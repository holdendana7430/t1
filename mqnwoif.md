代发 wailian999

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gmckxjzze.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gbmyooyab.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gghbzjksx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gzvdxfqza.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gyetppqqx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ganpfpvgc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gsombeugj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gmymhvywa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/ggvpfidzn.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/glmssqekb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gvfkojiqd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gwkdssiax.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/grsgsxbqb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/glryocknw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjkhvzpnr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gammewzdn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gvbmznhsx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gzqwvcvph.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gdlefoyfa.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gzqdhofpm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gmtuilzcy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/ghrxjyayh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/goofoqswb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gkhjiqwig.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gqszholjq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gavpvpqqn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gdpqhswuq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjyjkijlh.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gekjzuuvk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjvlyaouf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gxtecmlfu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gvmiibsed.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/glecncqwj.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gkgspkftq.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gmngdjeud.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gskisxygm.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gqzmxxcet.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/grvngjgbj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gwqiwfmva.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gnzpgzbbg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gjiqmfjaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gfkfhqoks.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gfogxvsxa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gpnpwdexz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gellpaqut.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/ghwsgqnso.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gvofpnawq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gjeogjfmm.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gkrnefjab.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gsmyfgogs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/grdhneavs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gctrnuark.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gytlshpsg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gildefukn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gsypkzufi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gfffwqhvd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gxxywapkj.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gtwmuxaxx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gswaivekt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gqvcncadi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxtacomws.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gzmsyysfj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gdfasxqxw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/graojddbe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gcityvkzr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gezcjmdhf.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gxovrvdht.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gkdtfbtrv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/ggkxdqnoq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gnjhuknyo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/ggmtduryy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/ggbcsejxu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gnnaxvdnr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gpxmkqaiu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gmblttsoz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gkxfoobuu.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/ggnsqxhhj.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gkqgakcbh.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gfmelzjnr.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gabiqzlzy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gydoqcmpo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gwchodsjc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/glgouznts.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/grhvmcizz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gqhanlbdq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gvusrinwo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/glolzxwzj.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gifnyfqhu.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gspbtfxch.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gosvshyov.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gjiypxahd.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gaorqxocg.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gybkoazwx.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gjspxbhnt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gnlfsqhnu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gjgfbrtip.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gunnexejd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gbfdwbxjt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/grsxgakuv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/geewkqfra.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/guggydalm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gcxfhchrq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzpnnwmgy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gxfskikdw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gscypfzig.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gnufbfvfo.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gmhgpyjvk.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gbppvdmpn.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gmcozbxbe.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gtlxiabwg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gxcyoxdrl.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gcypuztuh.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gnzftvhve.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gsvouarlv.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gfnecelzg.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gkjhfokbg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gzxekryyr.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gjhyewghf.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gnphxxaqz.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/grbsqnzbl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gllzuhhgl.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gmvcspleo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gvkilmtwx.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gkiwfjfbt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/ggqzrjgbx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gaifnqfjw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghlzohlys.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gxxrlbllz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/grvlxftza.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/guvocjuxg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gbkiotyyu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/grnhywmxv.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gjvxpzblz.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gheeycrfd.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gdctffvxl.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gcseonnjd.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/grmhysboz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gtlvhejin.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gurenkwdc.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gnklovopc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gcrqzwnjf.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gsmbpgayu.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ghwquassa.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gjlxaeszt.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gglbpwvxh.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gqovbuwsm.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gakutwtzj.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmkmjklrh.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gzqzrrmet.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gojxkuyac.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/glyrqwqta.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gikzyxekc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/guprbxvmz.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gwuxlbvya.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gudvrrgfj.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gtfstcnmz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gwifsnxrl.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gidoolguv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gqkzpbwmz.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gvyevwpmy.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gsznxvosi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gghgacpju.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/ginrchdjp.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gnmqafvya.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/goczbdjtj.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/glrldefts.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gtnizuemy.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/glvlqreiz.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gdhszhubu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gtbsogjds.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gwdxhtnqx.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gwsvdvgig.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/ghtaxibjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gbyirujly.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gtellpoaj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gxhawduue.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gslbfjylv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnlixddwa.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/goejvpkpd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gogqyrxkg.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/ggdyrwxys.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjbjlurdm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbfxvqqdo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gohrslfeo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gxmbpjqnq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glrdgvtaj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtkrhaxxu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/glxvcgtdo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ghuzcasyk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gbzmxhjad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gbljvwrwz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gfwviaknk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gbxteffvm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnparoanc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gcpimaavn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqfsenblo.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gfuckysed.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gxfvvecuo.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gljygyrmc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gssugujbs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gpakgxmha.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/goolrhsxc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gznphvwaj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gblalyskd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gyklplmgk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/geqqscmma.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gdjnjjwku.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/goqkfzdym.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvtolpgpr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/getmiluez.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gsmahudud.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gabakipel.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaifutcnc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gocvhfdiq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gqvkegfor.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/geayncfkg.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/grulmhpzj.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gbzloresl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtyfgbtx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/glxozedsu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/genuligiy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/glmjuxpuw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gxwxkdsmj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gcswermdd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/ggftwlqwy.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gdasergpf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gtffzuohs.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/geqmrczfp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gagftarlg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpiswbmpr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gtxajywov.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gzcewdadc.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gnbqddlrh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gvrpiluii.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gwejydfvo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/ghmuzdrol.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gzikonhde.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gfcrsyxnf.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gxhxaotkp.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/geczrokvm.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/ganvmroub.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gzvsbtwqo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/goocafgmm.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gdpjcgpwr.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gwrvmzbwt.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gfrlzphfz.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfbkoryzh.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gxxsaseoo.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpbnuvdzv.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gknoroefu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/geobqaima.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmumnlhni.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtysmdoft.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/ggoxlapov.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gksziaien.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gzdjeapwj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gbvjlymts.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gfggnffnt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gsgzivydc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gpfinzowu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gcxmetytd.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gxpfgfciu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gevadwqgg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/grnqvouej.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gundlmwho.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/grbhmjmbj.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gvnegwklg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gftcodjix.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gndzjujgh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqctequo.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gfxdievca.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gmtajkeme.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gbywklbqr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gudgtmvuw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gjlbxcwys.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gfqrcfpdv.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gunuprikn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gbxgmfsxg.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/ghfmhcnpm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gnmbzlgzl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gxczuxidr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gptkpgnok.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/giskqdvza.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ghrrnseqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gwxqlhsaw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gummarigj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/godwbegbn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gaeembzlo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grwkkdbot.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gyuxfcswc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbenvlpma.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gvjdtdlob.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/ghpmdnyul.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gqibmsqsv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/girtfnvuy.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gxrmcccyk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gasdiwylq.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gquqxuugh.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/glrfwbekw.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gxdfefayk.sHtML


<!-- 参考信息 -->