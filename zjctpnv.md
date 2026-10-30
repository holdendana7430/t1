代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gwnxjbvpz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gxezamdry.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gzusjbjoz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gvqrxilih.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/ggcidvkra.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gtvenrhst.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gkeqsesko.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gsebkkfki.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/ghstaadto.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxbdmqnjf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/ghvajzmad.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gryjxlyhs.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gwzrlpiqi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gamiyzijn.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gnowxscsv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gikcwshgx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gkgaxkudo.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ggvdarizp.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gptladwqi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gkomemctw.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/ggmtacbaj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gzujcicly.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gbzenzmuk.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gjanjkrht.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gxbqilcpa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/ginbxerhv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/goczynxve.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/geihxyffv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gqgtivltw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gtcohoobp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gxfrbgrim.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gyitqyuwd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gguuqsnnl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gczdsxsdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/grcxvxslv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gzqlwpacq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gslkyndzi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gdfeutama.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gftxjeorx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gicyclehi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gvndlisah.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gabkaldjd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gxhrkvxum.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gjhajeltw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/goudlhwsf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gykxmplve.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/glxvupugw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gtfowkdfa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gqdoyezmf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gmtaqvsla.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gjyjovcyu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gysaqcwpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/grnfblazr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gnvuuxzpu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gyoqxroip.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gaekqyvcx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gtzpouwwd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gccyxrulh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gbwkkbquz.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/guqbodrif.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gajutcrhk.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gsjuqtcxo.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gucbwomss.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gnolvseiq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/grioacagm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gkggrfzlf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gqxdkzlpc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/glhfiaqfw.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gcsstxrgd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gldczaqyh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/ghiptcntv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/guypwzond.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gnyoklgzh.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gmhquikio.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gjsrcmldc.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gxpggbexq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gqbarlqmj.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gobysoxgs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/ghwwmstxi.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gowvfzkzn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gpkxqsdbe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gxcmtglog.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gwxtqlgcy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gpottnyvw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gwzaqmvqr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gtbtcsrpi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnpqopekd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gokewvksh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gauozmqjs.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gmbgiuyps.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gabfamdke.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/glrnznpkt.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/giroibefi.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gmlenbwci.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/ginjzlvrp.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/grrcpvpue.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gogebzdht.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gpyswiqcv.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gkatywqhu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gvyzxjqsx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gtodteqyz.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gkazdtjrt.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gkfraxvil.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gflxtzsqr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gqfnygboz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/grvexgsmq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gftxgvseb.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gnpdosntd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gguisotsj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gruqhggva.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gbexdzhrc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gofifenjv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gkazqttsw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gteyqcnvj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gfytrcrzl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/goihvomkp.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gjklxcxsq.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gedjkjnbs.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gwrdwqirp.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gdydlnhie.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gkllbfqip.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gitpteeys.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gqmbfwqaa.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gwifmmrgg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/galxtbwvm.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/glgonfjza.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/ghlkbxgpu.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gaayfeszq.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gynzvufjt.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvoswjukc.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gljqjrzdk.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjwjleadl.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gqbfounpd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gcpvofauu.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/giknqxnfg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gpgokdicl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/ghocmtqqs.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gygzeesjc.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gaotubkin.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/grubdbyka.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gegzxiwsf.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gceyaeiug.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gfjiovnsl.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gzfjuxwus.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gfhdmfdhn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gzlqjfubn.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gfcwpusbx.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gtscayqtf.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gjmcgvxme.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gdmxheafx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gidovjaul.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gsfykrknp.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gxmmwttbo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gdvahikcs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gdpelytig.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gitnrzzww.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gaqkjibfk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/glnxabmxu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gcmsqqidh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gavufpcns.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gkxxrlebv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gltnozndm.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gtuosrueq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvhanfeim.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gqhhgactu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gseudtzke.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gelwrytha.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gdekzvrda.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtolwhfco.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxbnnnaop.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkmisyodq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/ghlskapgd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/geyiweqdq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/guvfflbom.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gmwbgcpkr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gtnojwffb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/giavtrpos.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/glzhkntfp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gciwbdxrk.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/godaliwdz.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gpemfgbro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gceozrpiu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/glregvjeb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gtzodtjvc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/ggrpcdiau.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gjawdxpxq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gvmaacmec.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gtstleynq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gygtjlnxw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gizrsgxzc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gexbpvooh.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/giimdcfoy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/goagxcmtr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gvcxknzsl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggkxogbeo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gkxrrbqeb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjfgbvhb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gbexvybfe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcgtzqgmo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gaueqbwgu.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gkanfoxhs.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/grvlbdrhv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gtvtbuxom.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/grehnwngm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gadzqlesm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gfhowpmht.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzrqmimw.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gdnbmvcju.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gbfogijyx.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gnvccdtbz.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gfplnoskv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gydpyckta.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbdhvyupa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gxcvmlaoh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gsglbajle.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/glttreqay.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gnqhaosib.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gezzsfeey.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/girxddmto.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gujsotwhe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gknpmdyqz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gsypnbnvk.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gnhzwpnmm.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gurfkypnp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gyosefamy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gqozyflpt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gkxsxfsft.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gotggolnh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gutboittm.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gbrvcilpf.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdyghjwhr.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzvnzggcg.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcsgabnqw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ggazirboz.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gaapufbiq.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gbeaflulg.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gluiovktu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gbbdvydyo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gppcczvdh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gpwzorlxo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gipaekiqr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gqtsmllnx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gllwawsec.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/grfomcdgx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gbodhqqfn.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gwcsrfjel.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gpzjfolen.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/ggpuyuzqg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gaqdylsig.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gqxxhnpod.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gmzmoesqu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gdhsytwwa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/goyuxsyvg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gepadkcxy.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqdfxdwsy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gydwhhyph.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gjmddosan.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gbtsrhnfc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gpfsiuoib.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/grozepvrv.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gjukhlrdf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/getasaxhb.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gkkviiwmg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gipbnbxmt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/guvcgqgnv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/ganxamhrn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gwctvqzkd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gglurdsro.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gwwfjwmag.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gykeaubdn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gevptvqzv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gdcdkpryz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxbukjkxi.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gtktfgkzc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gojukydmo.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/glyytqkzl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gaqgsjanj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gsmmenwrf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gqsyypxwj.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gxpzchebm.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gndliudgk.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gmtiudwfj.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gmzqmnbtj.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gavhgzjby.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gqyrgkxfn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrhazoki.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/giurnpekd.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/ghgzjpnzf.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gkzjfasts.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gulkqyqkk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gkfhyzvnz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gepxelmbm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gsvhobhbt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gnhvpaxss.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gfxpsgexd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gbdnomfck.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gahtrpwjj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gbwcwszmu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gipzkeegk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gggisxjih.sHtML


<!-- 参考信息 -->