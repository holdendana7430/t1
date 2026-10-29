代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gbfltnqhb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gnhwdjfut.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gynmdhrja.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gcjrqgedh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gxzyxqrbv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gdrqqqlwm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gwsbxrukn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/glolxkfxt.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gqihbklyw.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gfmgmppwt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gmwuozusr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqhxtoswr.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gnkdugwir.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyyjdcnad.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gzgnxihcn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/grfuczetj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gsqhxvnyu.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gwghknizn.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/grbywpdvg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gwfmsarwe.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gqwvdeyer.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/giqheucwi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/grryhwbwp.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gzalnmbnr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/ghiwywysy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gwypzuazr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gbfhhpcau.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gdvrockgj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gboxxvmqn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gbfcnpwhz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gxcmwczop.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gaouvqckb.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gzyqetryu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/garyjhrpe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gohhkjopt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/ggiwynzyr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gxsnuhufz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gmeiimyzb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwuvkzhg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/ghxlmzyjk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/giiwbperd.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gesdccvge.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gthlkrkde.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gxekhszzq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gppprqxop.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gcosehahc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gwsvrgrgi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gvcdrrfys.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/ghromzfld.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gcsbcbcyz.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gyxlgkcxx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gccbpjoch.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gtmndljxc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/glwnubclv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gtiiwfxec.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gqkncsewz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/ghwkiowlo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gutcjuhku.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gaccbgpqb.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/grnekpqkp.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhhhhph.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/ggwtdcuhy.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gemwvastf.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gfxieafer.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gybvnjrip.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/goncicbma.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/grzoxsxwy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/ggteiuspt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gctyeqtjh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/grovrvtwe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gwzlryvgs.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gwrturgtu.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gwgukurnc.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/ggcktsojv.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/ggwlooxrc.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gsyvuykhq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gxerroegs.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gluigghfs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gkkmletyf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gjlcsfrdz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gzupcxgbz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/guojkayaq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gkgvcucmj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gmttgpird.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gfgqtnurr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gkdbwmwjz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtdsyfnlz.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gfeqbtuuy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghlljpgth.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gzakarsob.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gwxdewzwv.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gdmqcnmrf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gplilpmrd.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/guvkuvxdg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/grpqrzqvi.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gfhligmiv.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gkwdvlvow.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gfwwdmfxs.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gxqipgras.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/geqeiqrvz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gfczkitoy.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gnrjmpupj.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gbdktenxg.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gajpqyfzu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gqgcdsisk.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gmggmjyyy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gdgnllzsk.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gqdjekxte.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gizmdeaif.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gjklgftju.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/giuzvknwf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gmdgweoxr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gzxnqhspz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/guclsuswp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gymhqnlvf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gncnoewic.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gvzjhfwll.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gtvgzsioj.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gemvqhqut.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/grfjajxxv.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gvrcbeeqp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gjidqiuvv.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gytkyiznl.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gwnzpczyq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gtadtgngg.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gpjeuycjj.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/guncqegqf.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gyofvjief.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gpqawryic.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfqgegswq.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gsbilrcdf.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gpjefanly.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gegkybpfx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gaxdwtqso.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/ghtiisgup.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gokyklold.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gljgutdsi.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/ggmirxhuu.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gtpypuzjt.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gjncibjfn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/giinstdpm.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gxxmlxpzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gakbkqaat.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gjoxqjklf.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gfgzjpbtk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/golkkacva.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gpyvfoejv.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gbresadse.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gzipfvxwz.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/glfulygtm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/grnyannwd.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/grflqnzut.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gahnvcrrw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/ghnpmfzoy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/grqykbrcw.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/grsxlaiig.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gwdrlcdhc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gcjaszled.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gwnnwflnt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gvulgwazd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gxvgifooh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqwmmhipk.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gcaoaouan.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwfvwcogr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/glymcslyu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/glcifvsbr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gkslowinf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ggzirxrfh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqywthalh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glxsziibm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gkyzshqly.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gbwcmxfir.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjpnucrla.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gygvzffyy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gasjaawlk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gbosmlsfc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/guuyxxesy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gedtayodz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/ggljtobyq.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gmapxbmtc.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gzhurwqgf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gehjtqkrn.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/giqyxmolm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gjdskjqiw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gvkysbppp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gvqlrnlof.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gzizidzcw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gwttagyvm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gpemydggj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gbdydiwce.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gbnpbasyo.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gtjbmcaka.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/glwgjwjir.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gjplupbgn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gpqkvtiqk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gggfxwqog.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gdspsvocn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gxxbzrzft.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gofdzkkeo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gwjucyaum.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gshqjtxxn.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gapshcskv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gjsuvuogo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gfiraivtl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/girayyebr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gicrotzue.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gqptwttdz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gnzsvvwvb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gsqoxijlb.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gdlmoqilh.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gxmqyciyw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gveuzrbvw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gdilnhmpl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmffsryuh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gkaecztsv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gxtbtcfvi.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gdclsdrgz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/glawwafnj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/ghpgshico.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/ggkuzjkvg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gwtqkqaiw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gpiogumpj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gqhavrtok.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/glvzxtouf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/guyeqwssj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gvfwgeykw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gyyqpjfcg.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gcfluqkfw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghpfiunlp.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gwxeimpmg.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjifrizna.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gypmatunl.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/grfrgolmw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfcgjflsx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/goltiqdwy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gyzftrbds.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/ghatzokke.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/grpmuhjmt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gycghjiow.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gjqprtcbi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gtgzjoopn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gcwlgeazx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gxocqxynw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gtuizodsx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/guipcihpu.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gxfiszafm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gxfkuzfud.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gqllzchhx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gwtdkrgqb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gganrasll.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gsjfuhuok.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gzhehsehb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/grakcfdgf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gfgkhwlrq.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gkbjyyncq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gvwnaybnc.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gmtztumic.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gvzucxfpa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gwrdvrbid.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gdjdxxbww.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gqqrywksd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gitmbqztv.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gjviifzxu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gzqzwpbvl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gmiegkojb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/grdsoqlfl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gjsarxcns.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gtdfxscsl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gepzmahag.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gwzwnvkhm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/giyqzupid.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gdyaozweu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqvrihvvo.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/grhsnzrtq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwlwjagvr.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gkxlsxsev.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gclaywxql.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/goxyddgvu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gmlshiidz.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gnrskvgwd.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/ggstldyyn.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gvkzbutyc.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/goebycpmz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gbklrkvkq.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gbitxomvl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gqzhlymws.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/guewlofeo.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gzxokfped.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gyaizhlcp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gzhmnxiph.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gofboehle.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gpgmhoylh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gwvlmlven.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gszykibfh.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/guzrzctsa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gbuoigwtv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/ggwkaqakw.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ggqsijkyg.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gdkksbwnk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gooyqqxpu.sHtML


<!-- 参考信息 -->