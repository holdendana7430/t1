代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gefvgrlqv.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gkguvhqqy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ghobupjbt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gxfavveey.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghenalvrc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gtgoqdtsm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gzvwmoulv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gatpnrdon.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gubufczxt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/giylhbgyy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzhohjo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gdvocotye.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/ganqbcahn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/ggvtynono.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gwfaibtjt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gfuigpwkv.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/glsyrtuqs.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gybjywnoy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gwcqgavzh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnofynuzx.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gauuxgzbh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gulebyuol.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gvfmijrdo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gvqqyqfan.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/ggvzeokim.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gltzlqumb.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gcjvdeguu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gggiijwgg.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/golgzddiy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gxvujtnca.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gnrgxkgpt.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ggsaosynv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gpjawdfnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gwibeuugf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gnfyebmxc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gtjbnnyek.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/ghdpbmghs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gqgqpvzty.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/ghwdprbxg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gxdrkxrpz.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gxmumwqvq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gqqmpnkoh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gnvbwcmuw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gabakdcwn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gjwkshfsc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gtojeognn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gkpfmfyvb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gpvsvtshx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gdurcitjr.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gprcbxfhq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gkxktzjud.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gfubutepy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/girxxwhes.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gantlxcdm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gexwnrgjs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gdzawmivc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/glplevnzn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gozgqbszc.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gcmmalglf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gzmulsqxz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/goefyrlfq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gymkhmhyf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gauhzkbmg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gviubrizy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gtlrduufh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gkkmotvoo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gipkbssfb.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/ghassrama.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/glfzyctba.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjctqjilk.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gwtutfmvl.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gotmyaclt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gftwlgxvt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/ghzqgzgue.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gfbootjea.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gyxugmrin.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gpfvkazqc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gesqommuy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gvrevrrnt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gjncqtoqd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/goedmhlvl.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/glyxmfdcc.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gjvsmnytc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gayjhcemh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gjxdwfxup.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gggdvprui.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/glvbimbru.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gnvwiypfa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/grdeszfob.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gzizfphcn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gsokgkisu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/ghbtmhtdo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gzjorjdyu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwwqhrxba.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtnlusmqk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/ggivuljwc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gswztmzcs.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/glhtsgjym.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gcfpxpcnu.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gnqezgken.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/grnrknbau.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gslvzvbeu.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gbmqzlrss.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/geusghowm.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gmfpvrgob.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gjrucrpya.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gepxvmlwu.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gugyrccfm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/guzfafqaa.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gximohshi.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/giahuhyyo.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gggolzyxq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gkjggzbbq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gpckwgsbd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gbtzhdxqx.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/ghswbigue.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/ggutpoaed.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gaqzpoozb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gxywvbkja.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gvuwslltr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gcizvlyuc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gogelpwyr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gfiswnqhd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gzvbfbuhw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gmobjvinn.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/geurnkvmw.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gmxpfppmn.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gpqkhqriy.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gevxkplvp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gckdjndxd.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gxfmdeeaz.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gaxbjjase.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gtivkcyhw.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/ggumfndos.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gogikpmmw.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gdsvlqewr.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ghbpzensc.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnssoecmc.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gaicfffir.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtqbbbavf.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/glgoeifse.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/grlexjjyd.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gvmywdodw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gqudndktf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gghgeteus.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gcibjpfft.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gepypvzox.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gwxunwqbs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gwxujmret.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gyaidxpws.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/glcnpivrz.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gazblhktu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gofokjhec.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gatmbhvnk.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/ggrcfpeny.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gveoqenho.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gchcdobcz.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gmjdekbfx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gncwytxnx.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gprqksrat.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gbcgacjqx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gqlgigtbh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gbtyqhlgx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/ghhrvqcnl.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/grcncpssu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gupfkbdlj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gphlecshw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/ghjznsvea.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gsqgsxnpv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqihqikez.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gqdvfpvbk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gshqjzmuu.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/grjzfgghi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjkjhtxrx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gpbxhwnpj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjwsfqpmd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gztuvbqfb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grzcrpyge.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkgvmmgdz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gaguxcdxn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gctxihxhg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gvdwxktaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gbfxfhzcw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gerbuhxgh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ggqwxjwet.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghogzxnlr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gzfxrzpuh.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/glrwqoiyp.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gfqxhofuk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gkbzargsk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gjhxdzqcu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/goafdezpb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gkiuudmgr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gllhcpkvu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gysgicgpt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzpjgvwrm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gcynrznyj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gxkmvxvty.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gqjznmycj.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/ghnilaryl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/grrvafmno.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gjloontnm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gadnwkzgx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ghelrocla.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gekcrhhyo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gnyvludnf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gsisgtalc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgprtlgn.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gvfnaphaa.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/guznnsrgq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gjehpneva.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gwuuqkcjk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjyrxubei.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gnfaqhmvg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gwhpzgyhx.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gxntijhhr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gantolhsp.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gfrhrkufr.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gkqwxzgqo.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gukmkphce.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtgfnxukv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgvvfpa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gitpbbpmn.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/ggygfifbr.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/glznlugin.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gaeieqnpj.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/grjnxutvr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gxdbuiuxu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/glgftzqzi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/geqjdwplg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gcvouidvz.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/glzcqrbck.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gzerdgusb.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gwdrbzxka.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gavczpqux.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gfutrhawf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gabqytkjm.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/goqyluyxf.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfbrjzweg.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnhegwpwi.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyaegafmo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/grvngzcba.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/guarnwyvz.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcopwiqbu.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gthqpyiez.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gvuviqyyb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gkbmkfheq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwchofrth.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gkmjpbuei.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gxroqohqj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gmltqoaue.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/goomluvdg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gbgcxiiwv.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gosfhdcdg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gsurpyqzs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gtthsvsam.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gdasmvdny.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gbmrqskei.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gpvzqzula.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gyeerbazw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gliokoubv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gtvrvxiit.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gdsrirnbw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gvykufcyp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/guhvrirxe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gndgykzsb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gcyipymso.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/guzxhapru.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gxjsmfrkt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/giayufgck.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gfiymrotx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gotweqqif.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gjfuxykee.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gzktrlzkf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gssxnukgb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gluuozdky.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/goafyenjo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/ggoybrwka.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/glmuwfujh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gxluoekfl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggvagxiao.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gnpozpvkd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnorpkjak.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gthinawgy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gnmgszkai.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gvusahvzh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/ghdatlouw.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gncbpfqgx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gmxyioiey.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gndputpcc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gzbdlaqin.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gnucraaoa.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gdyessngv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/ggnyyydki.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/ggwrnotpw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gwzwcjpok.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gwdxwpcqa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gfgevufgp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gwvdlnsky.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gluifbvth.sHtML


<!-- 参考信息 -->