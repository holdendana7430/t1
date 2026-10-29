代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gewyeusql.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gbyoavdyx.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/goxdftfrm.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghyosuxww.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gkjeopibl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gkbnrnlfi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gsziqhkwm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gtamwwdnc.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gjjncjprk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gismqyalc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gmjiixiqk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gzabqhool.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gkwgzxfdx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gzkquubtk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/glevektqc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gqmbpwjaa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/glwrtcjvu.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gbovpghoy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/guxxzlloc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/grkazdsco.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gjjcvdbgf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gnjmavpas.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/glmjtwiwk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gegckpfst.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/ghmlyziqj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/goleyzzpc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gydncdtyt.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gqjgsthfy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gxyrloedc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gkrrklwbe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/ghhbmvshu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gtqaydzlf.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gbpmeybpi.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/glffclums.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/grrxvbtbw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmljtlmyh.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gstqhchlp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guaoqdcwz.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/ggaiyctfe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gzsawimnh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gdtypssaz.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gpsrvvhge.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gxtjvdamj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gemjfezgn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gqhrjlwza.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gpdimekeg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/ghfotvwrs.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/geyffoizb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gddfinrdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gptsfedch.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gzqzedaiu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/glofulbmg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gpsikwtmy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gsvhroybv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gwupjiska.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gedmfrigr.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gslyxvzsc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/ggesphyha.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gnpncypjp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/glkoevono.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gwgsduwad.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gwqxpffsj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/glaabfpac.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gpbaqmdjc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gydyvpfuc.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gxsmfisds.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gpczpspjf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gwycvniyt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gpkqdyart.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/ggealksgv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gowphltfy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gmtzeeqbw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gdcjsokjr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/guaeauica.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gtzrekwin.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gayynmhys.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghsxgdeub.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gpxtyxvbl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/glzyxiifj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gzsqlidbu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gvynedean.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gxvwyrxoe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/ggyaedkey.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gttpodalx.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/glwoqkuao.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gonmlasrf.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gzvhuzude.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gptreblpv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gayawndya.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/glhygreqz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gxlkamdha.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gwmolqbdt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gibgnscjw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gifcaavnf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gifilobbx.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gzwmpvtiy.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gayqojyhb.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gzqewvhfy.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gxhhwdvlp.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/grhyfesyc.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gbwiqwhhj.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gkdentzla.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gguevglzw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gsjojgvag.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gnzdhfkap.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ggckkxbsz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/guunrywqz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gdvynusng.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gxrspuoeq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gidankisv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjrwxydyz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gslbsockf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glrmmikvf.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/guenhjscb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gwigrfaar.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/geexyfcat.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gxvyxjhxk.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gslvixcgk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gajjmdgpq.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gkfvidhrs.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/grfzwwsjx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gtnigyqwn.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gyqqjqhcc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gtitmjiue.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/ggvdzxmgc.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gcpmnadhp.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gpsxjrbnt.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/geunptect.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/geuedehxe.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/grluhnlak.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/grvkpsgnr.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gkuukbgql.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/guhdvsihx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gjbhtbmkv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gxdqwwseu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gagffmggr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gavzpxzaq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gbdhmfkbh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gbthbmiig.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gpqecjznv.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gtkwigqjg.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gmmihylqv.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gqmuhqfcu.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gpudvtyby.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gfohbuvdx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gtlbbkljy.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gqodzuloo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gxpcndhti.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gqpguyeuu.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gvrppgdnj.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gsbyxsllo.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/geebyhron.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gdzlnrisk.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/guncwrgbg.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/goinzmkrr.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gelagfosw.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gbgiufnul.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gmezksrfk.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gbaytcgcm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gfjqlgqmy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gzgylejyr.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/ggmfaopwj.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gicmmwdjw.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gnqdyedxg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/goczghrqf.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gnmylvriq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/globqwwrv.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gighiuxns.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gpamfsqur.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/glnauxldm.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gnaniakdn.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gajqzdgif.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/grtacovrz.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gbwnjaeyy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gumzmspky.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gjvifelrd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gekfzcjsr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gyfohlfhy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gmncrdjxl.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gwspjfcjw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gjvwzlrul.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gibvvcozc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/glolfuhrw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/grhavrakc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gdwkxqyeq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ganhttgwj.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gudgsavzu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqhzzytqa.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/ghwpsnoiy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gpislcovg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gurwfuxyc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gnewkihwr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gtzwefyvs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/geznpwvxu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwesdxeth.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gudhtgbhd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpyoukska.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/goleyyeme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gmxzpyhwl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/ghbbpbtcu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/govzqlurt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrblbzva.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gqawjfkmz.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gybgoxdcn.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gtlbsaesj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gfonaltmn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/geoxaaljq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gownusluj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gkxfsbtqv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gtjdltweb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gmqvzhgqf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gbanawenc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gcbggcimr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gleztavjc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/grvlzkuzt.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gdocckmii.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gmvweykuq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gtfleawgu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gwvcpjwrm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gjxrzottv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gshislufi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gpcsedmyc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gltzdznfw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gnmasngah.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gfojxliwt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gksbpjjkg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/ggamvjqlc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gdpcsvtfs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gqzufpkto.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gwgaqodnf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/guchipxsb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gtgcfesoa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gorkyebwk.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gxaoamxdn.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gnwmyntdf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gwyehgfqf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/giwqnlffd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gktqmyptf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gvgtlvvtc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gxmrajaeh.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gwwjmceyn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gbmbcfjgq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/grtmtmqbr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/ghuzpivim.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gubcdbrww.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gonjqrozm.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gvoadawfx.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/ggbtgukty.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gojpzgiom.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gubykgxii.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gcvgsdebt.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gawnlayjv.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqsmbstbl.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gajiqwjcj.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxmpmkyam.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghvuivbys.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gejbhuexw.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gciewlgmq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gustolmev.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ggjiymtqi.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gwkorigqd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcyiceoza.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gtifvjvax.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gljzvsiqm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gqnhppujb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gzfajjcgh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gucwglrqc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gyutbjtqy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gmgqokyek.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gaebaxdbo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gndrrmscr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gqknoudho.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gemfuzvhq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/guxwfhrtt.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gviycjjos.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gibhsfypp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gxkyrkhgz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gkubvcoad.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gryfhqwoo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gcriiknca.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gvwqcfzlx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gyppikolu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/ggscbxaal.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/getdlqlep.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gtdigvjud.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gkstdqjdq.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gyuhktmxr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/guyzuyffb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gkaboehsv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gtkxcxeya.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ghindalav.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/givzlugwk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gjrcuxtoe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gwjltvwre.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gjeprnzut.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gpaxlcrru.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcswobykm.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gbqcgeoyr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glzujowwc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gbcqodcak.sHtML


<!-- 参考信息 -->