代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gjeqqshsd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gibsatxjf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gqebzcgtx.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gnfypbjik.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/grtrfiiiy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gobpgqkbd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gvlouugai.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/ghlqqfiyk.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gavintnkt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gqibyelsj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gihgctzdl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gvjgfrdka.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gzjxxcsmx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gqmkaaxuo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gzetqioca.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gdblxkzvy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gcmkslcxs.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gvckhbdng.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gzcuuezdv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/grpdesjvj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gedmteflf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gllzasmyt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gcwfkmkcd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/ghmbvzepx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gccvgwbpb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gxigauuth.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gvphrzcmc.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gnzrnfrnf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gabgeurmm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gimmraevp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gvhnxnjwr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gttyusjaf.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gnmkppjlv.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gcfgivlob.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gkisyrmzy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaflsosfh.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gfqttvamx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcrhxgazo.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/ggeofvfrh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/guwuklpom.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gmmysidbi.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gfhhroqhb.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/ghoqwqkhf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/glmzjydta.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gtwjjoclw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gmuhmclks.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gvvkprnfc.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gpipzbkez.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/guvrwnkgz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/ggfbgbsag.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gqqdleasr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gaobgnfdc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/glhnlrnfo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gnjndulew.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gnminmlyu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gxikzlsma.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gpkiremog.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/grptahsec.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/ggccedwcd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gaiuiujwh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gnxoqznbj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gcllwhvxa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gzbibfilk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/giqznnout.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gowujyvtp.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/ghoazzwsq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gyoelqpsu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gpdouimrh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gqpitlynv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/glhxttcfw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gojupvlyx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/goqfgybrg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gukuzqjxb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/glihlfgkr.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gmrwwtuwq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gsxsfdkds.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gtgxxrjef.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gdeywqkay.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/guqvbwteq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gdxtahdac.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gozloaklj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gduslulsr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/grahheaxi.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsywszkqz.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/guclgzypf.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gaysdscxm.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gqhunlnsh.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gdumxwibm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gzosuwkoq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gsmwzvakm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gqpeypcul.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/ggxfrrcew.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/goegafbwc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gkeeuetqj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gfdenetsj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/galdfqoce.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gdncxjzpu.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gqdindkis.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gceghnwgt.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gssfogdzo.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/giidmmyue.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gpxiezmkl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gsfvzrfvy.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gxmfdlbcz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gdngplikg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gstdkjufo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gcxlmejmu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gwzdxhhbz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gvqtgbbza.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gotjhksid.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvzmthwuk.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gyptsqgco.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtyevjlft.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gcsryfmzg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/guhvkiywg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gqirklati.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gagjrsaxf.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/glhpfosdr.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gmhowbcsm.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gmqqvoyoo.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gegsbsaqx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gkdjtjixz.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/ghutfqydg.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/ggbokucpf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/glctzvyfg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gwadavrdk.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gnvyxstjw.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gsztjfuli.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gxwwxzifl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/govikuiyt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gexgcacuy.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gyvqfscyh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gadehucpw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/grwthyqur.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gxobdahfk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gimytrhsb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gwwmfuzlj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gfgwhwcup.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/geuyesarf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gyefgipat.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gpvjrwfxe.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gbwlwtvzq.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gfgrbsrkp.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/glhcubsbs.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gknevgosv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gvywfrkbm.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gkldflrke.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gehdvvoyk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/ghdtqulyf.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/ggetgcuua.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcpxlrnkj.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gevgpmyic.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gzljlxepn.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggynkvhvy.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbebhdihq.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gufazclmi.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gfuuwylld.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gzlbywiyt.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gufafseud.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gmfjsacil.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gnhdoefui.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gcsydajec.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gazramvxi.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gkpqtqopr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/ghqpwfqmb.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gwymqfloe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gcucapebz.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gtkjocbdf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gquvnqblo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/grralvsjd.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gntvckclj.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gzrsdgziu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gwwwsvqeh.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/glkebkpnb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/golokohjf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gamgrgacn.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gaesqvpnm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gdlzfvalw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/glpvqjhxu.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gdvzxsfrw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gnmbqklqz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gvjfvueok.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gabvixvfs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gucklkpmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gxpbgglgp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gacsttdst.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gerqordvw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzusqjwmn.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gxltmyixk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gptarocdn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/guciqphdy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gahdrovar.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gbblgfoao.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzmndieae.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gehhyrvti.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/glucoqczf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glttrqhct.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gxwxpzatv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/grjedwzyd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyvzzocfj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gbmfmgzqg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gngdcieef.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gcainvwqi.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/grthylakc.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gyfukoohr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gcxvfplzr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/grghseevh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gjkjbbjjl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gxafrcliu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gwrzevaxb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gymijsjrj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/ghhhrqtzr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gkidzgeog.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gegajjvhr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gxmuubxru.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gqhyjfbhy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gnpotfjxy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gjbtwdvqz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gacjlhiwd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grlchtxph.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/grjbdajcs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gzaplrvgy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gcydqlvbp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmtpythms.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/garossmmp.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxqxzrdqw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gflrctalk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gremnwdxv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gqnklrunz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gqzxhcjtb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gemwsalbf.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gvbajmnwk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gxkkxkysl.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gjvhtomci.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gxynvmgsc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gietendog.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gaodfawgk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmhjqtdyf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gwfjvbftl.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gvmakpxwl.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gfspnvovl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gwgaeyksc.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gvauipycs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gbqfxqrbk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gqomlvmvy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gsysjsrro.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gesvshtgj.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gaenazdmh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gbckztyck.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gqkttggkp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gfwezsdio.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gfauqneec.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtwvznfbo.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/ggnnfzqqe.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvbxkzxrf.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gabftneqz.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grkkycgsv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gcmwaaxxg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gjsrveswf.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/guiwuzlqv.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/guyhejwwy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gddslvdsv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gskhwokqn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ggcpiroch.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gjlyxqkog.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gmjtjnxmy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/ghugtpvsa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gckeghiwu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gnbapmptl.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/genouvbut.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/ghsmdezwc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/goivqezwg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/ggmtjtlxv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/giwemfqzs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/ggwbfbscc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gekxayjlw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gebukmlwx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gdfciwofz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gmhqimvzs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gxdqramxt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gffqxvwzs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gtculqlyx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gkztxxhyh.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gqcrcjtcm.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gevlmovkk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gvoghbixw.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gogemmtrs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gwuwzxmuh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gqbamuwfe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gxqwjuohp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gxevcpzym.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gbcehdopj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/ghqwsmiqn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gbbxlyszj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gjmtotwlk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/ghzowsrui.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnhbeiell.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gvlujyyzr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcwyujvcb.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/grixdegpm.sHtML


<!-- 参考信息 -->