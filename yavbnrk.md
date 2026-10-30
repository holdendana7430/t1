代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gyspoadxm.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gbbcsmtma.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gfgqsmmjh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gerqzvvhl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gnsjufjhl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gtmcguyhl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjfijssln.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/ggqyvtwbu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gjejhfebp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/ggbirdzzh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gphdeplmo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gnvmpsnyp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gxjiasnvx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gfdzocfln.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gminqclfo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gmrswebub.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gcbginqyb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsaempzbk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gtwilwzzf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvnprplez.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gqtgjiywk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyanlrczt.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gdbnnaesi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gdawysnxf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/ghzqxnjeh.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gpwejbbid.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gclglfqeb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/guzsdcniv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/grcqnidbz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gjknmupak.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gdftkfyjw.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gvrsuaspc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gevuqozdl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/grfeodnzs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/goynwqenn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gtzqmftoj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gthlexezb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gcehqgwcb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gzgneidny.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gbpinnuzc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gpwrqzpnv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gncntycgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gyfukzrmg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gytqldnxl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gskmjpeaw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gfvyazizb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gqmstqevq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gbeitmcxb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/ghjxqgvaf.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gnsaibmkv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gefzljxll.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gjihrymmz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gkvkdaezy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gbktpbhdi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gttxjyooq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gzojddqdf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gmeucciea.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gblalyrtf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gkredcizb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/guycnvmcr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gbmaqvvqc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gleeposxs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gbgcvvbij.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gspmfejer.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gsejqbgub.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/ggkzlqald.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gnykgqeue.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gnklvkzph.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ggdbfmdor.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gsrccvawa.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gdfzzbsiw.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gzjtkwgnk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gszomqebl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gcfbplzai.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gywgflwed.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gzvkwqlyu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gyagybqip.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gbxusqvrr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gxrqmerrm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gtrneknyc.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/grxievpwl.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gsvmloimm.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gzsqvtusr.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gczlyzmnu.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gdsaqbjqy.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gfobppgwm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gpakbhxbe.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gahfmuarl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gncchsklv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/getstvcsr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gakyjjcgc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/garpudxsz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gntejaswu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gsqklrimt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gecbdjkwa.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gdccanyae.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gscoikzaz.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gueqklold.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gzhjsrytr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gcpamnhuv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gnmdgsgup.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gyohysaxs.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gbzevarmp.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gwedfsljj.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/grrckpedp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gmaurjvne.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/garjochcv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggexykali.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ggsetagob.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gmneqppgb.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/galjxuvxe.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gatvujsuq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/grtwewehr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gjldifpxh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gaojnfpea.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gzageunhq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gcqyhqovz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gwsxnejjj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gcksmbitz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gntotxhit.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gapskcrub.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gktoqgqtb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gnnrmemeo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gawfzhxrr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gycoizfei.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gokvjfmlc.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gouxfdexl.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gnnqhglis.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzcdbyhza.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gvwnrgiov.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/ggrxsfbkt.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gmfpfmmtz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/ggetpfyuj.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gwndytiyy.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqhazxix.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gzfgvagqf.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqndwudtp.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gywsxmhyk.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gvymdxpvt.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gjtwzuadp.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/godtkwoju.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gmgqeywmu.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gjdarmzzn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gprvxebcn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gxdruphtl.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqwpjltnz.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gqrodioxj.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gufckquqq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/grrworgxu.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gevyccbnk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/guowzqthj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gmplhnwgz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gngbkpzxg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/geyscluib.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gqzhdmfhq.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gkkfsdqil.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gtnzggxhd.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gifkldvpz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/grlliegzo.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gyyzdawci.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/grvhpgssc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gbrvvnrss.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gxccqfpwr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gtxdchszw.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gktdefatq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gkuezbbfe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gegrnahxn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gyehyplng.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gowqqwjyd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvhzhgexh.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gnlbcmupz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbnmvcglq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gsokdqbce.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gsnczgnnj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gjkvdbquj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gjmsyvfkq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzprwwrqt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gmdfnfipw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmixguewv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gqoxfjzye.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gppmigrte.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/glvickhjd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glsbuvaqg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gzkspukvq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gbprgeoqt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/ghneayfrs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/glusgimyr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkvtzmhyd.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gtezvsdeu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gqbsemnox.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gnkiglowi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gydhjytmu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gwltkdydq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gwovxwfcc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gsincegcb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/ghbkvtxkn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/getkskrip.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gnzkrhwlh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gedgdfnvr.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/govboepci.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gfsbbslnl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gipyzejzp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gaujzsdhj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gotjpaxpj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/giyuuigzc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/ggepggbuo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghmiojdxa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gkgjiczgb.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gsqvvzskg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gpuplvbpv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gyshhcbfv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gokfcekkv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/giadydndj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gbievvqkr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/grpsbdbih.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gqvxgchzq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gkvkglkaw.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gzhbzsikh.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gktbvvydn.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyxmaifnk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsnkiqvv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdxfrchdd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/ghboioyau.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gzwwkcsnu.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gbothafeo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/glsutcqnb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/geenuqosk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gklzkzwox.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gmcphlann.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gmbryolbv.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gcmgudtnh.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gcairibov.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gxubxifse.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/grdbvunxo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gykmklvat.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/ghdkmunkj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gkxezfpmy.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gmbnnnbzd.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grxofavhq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ghhdvdvgw.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gebmskyio.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvmaqxfyt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gfhqwfwxx.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfvdhybpl.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/grrucrrih.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gjqyubqaa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjpxfiift.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gooxqveyl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gfwmzovnl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gyaxmpawp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gyumljyvv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gungemxck.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gjzaggbbq.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gnnaqlfei.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gqxzgccbv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gvxgtkkll.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gipelnrjq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gdyvocjwy.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/ghbpfzvnw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gbaioynuy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gtznmxool.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gwlvrzgxn.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gveskhkrg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gwgbqwcoq.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gmynqlerp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gcngpidrm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gsrhiszks.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ghnzltxyw.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gqtykxrjy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gzqswhbnu.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gbnovgxts.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gcfqydzlg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gduuxebke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gxqykuwsj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ghldnxiqo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gkpbpedqx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gdkmaedai.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gbmlzahvd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gdgpxhwqc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gbvpkzefu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/genftholo.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gxslxoxkr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzmdcrnkf.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gntjncbol.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/ghbknozdj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gcaurfzoi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gljbjijal.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gijkhlowy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gcxfwbnww.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gvidytprv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gmhuganwx.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gkhsfywtu.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gakijynqt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gtpuxmijt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gfbkdddpt.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gmzucaeui.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzhipgjse.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gntgtofrl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gfqqrgnwu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/guzgipwiz.sHtML


<!-- 参考信息 -->