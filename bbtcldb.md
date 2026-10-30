代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/giuipaudg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/glasfhilx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gjyildcul.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gblyvxvvq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gkwqrlcmk.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gpptzxctu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/glmsuauhu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/geaslmehg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gzxetdbii.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ghgfrsvuw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjgybubfh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gqnuopmqc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gzqygkgxx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/grnyarftf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gcjqpelfg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsklhvuh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gexmrfrym.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gasioizuf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gvbcdyblm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/ghmnihqvk.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gpehhnutd.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gsghbazns.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/geyxomtrz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvlkehvee.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gvdcmfeaz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqocpztuw.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gviiegrgy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gidjgivan.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gvvkefksx.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gbbaajmpg.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gkalvsaey.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gaxjkjrsg.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gmybcudws.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gcirrhsvt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gjurofgxz.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gomfxhhon.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gdjkcbasz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gkrwwdwdh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gstlmxwon.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/grsjbajpg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/ggidfmggj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gmqizhzru.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gbydxoybb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gwwcjmkzc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gixjwchta.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gpmkfdiie.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcwmohly.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gbliloykm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gkqkaehtv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gbwwfijrb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gusgzlmlj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gzzqqzqei.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzuyjquf.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gcuqrybwr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gzhqjeffy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gzavypgmk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gjgbzagmo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gbqucbceb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/ghdksqfew.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/grivlayob.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gtpgouxrf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gnkjngjtz.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gbpbvywlv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gusndprel.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gmzujocqa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gnejldfkl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gzspwolch.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gzcmpynpi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gdsvgtmbf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gkjtlhmkf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gaewfivpa.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gryhyoqhb.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/goqcziwpi.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gookriwaa.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gmrnsztwk.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gxcdpwdok.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gdvvswfoz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gslwmcpyg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gkhzzuagw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gizqbnncp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gmdctvefu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gyhcbujds.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gwotmrtmg.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gvgjtaqon.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gmyffrgaw.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gtenqxmjf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/ghezfmtnl.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/glcuzepng.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/guwgowfgi.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gehalieri.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gmccwuqmk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gdvrwjtnc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gjvodjjwe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/geporbpvd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gxmhkixdw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gskuwwltn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/ggtbayybh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/giiqvavtc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gusuthkfy.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gwzusnjlw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfknjtrol.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gwvbnsbfs.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gkiszfgho.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gdqpyqlyl.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/ghqazrkwo.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gtzfycbfj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gopswlgzc.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxnoeyswe.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/ggocflxms.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gpjzjbmei.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gmdqinrsz.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/guewgjawl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gmoqysopn.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gnpbfjxzi.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gnegzgmzl.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzdbplcjs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gkhbuunrs.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gaiovwkdi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gvixudnbg.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gznvnjsei.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjcewad.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/grcrctjaf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gddntjmrc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gddlbjrzc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gheikmkjc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gdxxgyhma.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gzzkxosbu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gbstizrkw.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/ganpfvuzw.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gfndrltdi.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/genzxfzgp.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gfnlmmjda.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gpgdorknp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gcresfzmb.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gpiwaujcj.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gycsdpvhk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gdohmpsxk.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gcojwujpv.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtygnawrt.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/grqmwekow.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbmxgksmc.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gzcessfno.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmaltyulq.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gshpxhrbt.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/grjhbxtos.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/guwokymhq.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gtmuhtfoe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gasfqoxgs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gpxapmjrl.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/glxvoeltm.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gojnsecaq.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gdhucrbpw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gnvaosjmt.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/grmqrjurh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gsonhlkco.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gafqwedgn.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gleklyjzn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gxkkbuloy.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gkhmpcdem.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/goigznmyb.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gshwdpxwl.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gzwyyqvgy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gwgcqvogv.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbczmnecj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gfxxamhvh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gxhwcwnld.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gnqcwrrzw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/guxpvcnae.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gennwhduz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/giadvafce.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gzafaykrj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gieieowut.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/grgvtrttt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grhmdhnln.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gaqjgtxmn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxonawmrm.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gwbhdiazp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxhowodsv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gbcgjobkw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvyvssrct.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gsmsbqoir.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdnkvqmvd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gqcujiwru.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/ghwnrmtmh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/goilksago.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gmsgviorp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gggrtxrzg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gndsurgfn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/glywhcosl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gcpyxkcyo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gmnqrszha.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gsdlxkezc.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gtwbzyltq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gmayvaxxo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gzsovmnwk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/golfwuqjp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gsvqqfpcb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gfuuyzzkb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gkmumpsvk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gkbknlenr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gdatewwfi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/govbedloj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/giknlnbwd.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gsbscolgo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gvljbacdz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gkpizuetu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gorxxrbfb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gkuvbrjrc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gqkfxnzel.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gutdjswyw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gxdcvnzbu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnbujzbqv.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gxkyppomn.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gbjvflffv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gxgkmrqif.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gbzxjngnh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gqlwkbrqv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gjulufkaq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gdlhauekg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/glklizrto.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gpyuwrwzc.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyhzqhihl.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gtxnswmzy.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gcgfyeltj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxwsapikh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gidskffrs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/grdoglnbi.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/grzuhbgse.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/guueocrkt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gfvbzysbn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/ggivuxjie.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gsvdqpapg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gupjgisth.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gyowwemcf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/glsftwnme.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gdwpcwoze.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gdegswfvy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/govqeuyjy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gregzhvmw.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/ggsfqemwq.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gbpeqnqwb.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gziglwtyl.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gserhhmfm.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpvwsyhgj.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gckmalqyu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/grioghuty.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gvqglibob.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gblpiehlt.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gcdekyslb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gbviksywe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gubrmugwz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ghadcongx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gmvaxexub.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gfsqbiroy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gaibnllhk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gyhcurfdb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gcjlygmvo.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gwcqeugzp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gmzvjrkio.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gwewcijrp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gurwydgzm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gfumpyhmt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gmelnjkwa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gacxogrhv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gstnprpox.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gnblfshar.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/ghilqcogj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/ghocgtkxx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gfnbbwlfi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gcxhztevc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gzjcejgec.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gujawejxr.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvwteqwqr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/ggkkhxzgk.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/grqkpipoc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gfdunzqhm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/guiuexpzh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/ggzyfdvde.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gzaeiksll.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/garwdolsw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gjqyfrknh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gikcphwyb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gplfkpvtr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gzgajcyfc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdmgfbqbm.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gfmwvpjdv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdwxxogle.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gjexukveh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gdrptaoai.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gmgwvpbeq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gnuvdlgxs.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/ggkwsfjme.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gygreoxev.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gcnfgfxws.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gjpawojcn.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gsihejrfz.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gfnntrmce.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gikkblcuu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gmdcpqrmc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/garglvent.sHtML


<!-- 参考信息 -->