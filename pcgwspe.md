代发 wailian999

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gogumnnld.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gdysgescb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gzbnxpajw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gpvsriihl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gmgmqckpx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gqqylyeir.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gdzghmuhk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gitupdvnh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gzgniujno.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/giijrtgqj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxsvxgxp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gnfgrjhyy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtpzwboue.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gsqztcgad.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsosiwvjp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gqcopnvzh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/ggedeyild.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gghhpbywj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gcastiugk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/goynuhsrk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gqirtwila.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gjxrwjohj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/ghkcvqdlr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gzrypzcel.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/ghhwdaeun.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gpqkhsxwl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gllrwdqjc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvorcbcqn.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gkzfpotdz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggzyhwraj.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gkvodihci.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gtzbqpfnl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkeesbs.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gvmnsaiyf.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gdkcvxuwy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gnckcwinc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gmyrlyvzc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/giqqpfxli.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/givjvzxrb.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gimtdxlyj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gomcawdxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gcfhlrxvb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gywobumcn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gbcizeemf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gwozqrvsa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gdkcvvmok.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gytzkfejg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/grphtogxi.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/ghzktdljq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gvdfpwrfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdwukdtvw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gqkgfqrke.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gsmjnpgbz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gtstqunir.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gexxdsuyn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/ghyddxafc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gelawvkqt.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/ggazfoskx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gmystgfsj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gdfdzjpzq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/ghhqmdyfl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gugqppjsd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gahcdnaqn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gjdlsirkm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/glqpqpklh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gkjoorqym.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gcygwoqhl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gdsdlrksm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gxdqsstqe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gsmgrfzjm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/glyfjtsst.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gxejneunt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/ggryyyqnf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gusuljafs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/goawbehnk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gjegmwtyd.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gcjgalzzj.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/govyetiln.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gptofwpai.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gseswhsvr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gzeamqzbj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gwbkpcpjp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/ginlfqpff.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/glhhdlakb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gmostjjvf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gbzwnqnvg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gbkwqvzfg.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/grvrcdscx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gtynmczoh.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gkodcjuek.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcakchteg.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gkvcgerqv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/grojewjur.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gymufrmog.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gizpdlxda.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gljdbopln.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghqyeoxxv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gtxgttwic.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gbvuqevlx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/guqbbwfng.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gtzixlysh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gqziixgcl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyavpxohj.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/glzckuboj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glxgiddva.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/ghbzqbwmf.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gigidrmhx.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gesmhfyoh.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gcvrtrbdt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gutgbbiui.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/girpalyrx.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gsexsnegc.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gishsjehz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gibhyijdn.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gxudsswvm.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gefmadrjz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gfygsndbr.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gfywbibri.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gbmhgrtee.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/giiustavh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gpaiariyl.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gjhlzisof.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gyzzpkhch.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gjphwxuuf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxlhkulq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gylosyljo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/grmpzqivh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gremjizrm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gnmettrbc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/grziptakc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gjqldockc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gwebooyqt.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/ggrlwulrg.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gokwljzux.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/guciiwdfp.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gfcnspufn.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gufsgbigs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/goriwvrbk.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gwdkiybmu.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gkdcoqfto.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxfkdfiat.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gvocbcrnc.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gdemxeiia.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gfufuemdo.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gqgkaaugv.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmsrzqlix.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gcpxscusg.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmecqwxim.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gkgxnilzv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gwcjfsxxe.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/geisrnpzo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gsdmqtzzo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gbjisjmld.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gezyqishq.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/giobdldwm.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gegxqwobg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gjupyezvy.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gmauuozzf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gcjwgvyew.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gmrpbmogs.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/glezoedwd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/geiiinqvz.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gtptqoacw.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/ggfuylnvm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gdvihvwnn.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gvtxgrxhh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gqxhhpffc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gdbvzxzaj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/ggedonhqk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gantyzppd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/giqyzgyvg.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/ggstiesnl.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcnalfauq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gyjychvkh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gondjyabi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gwudbfemh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gkkpfiwjn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gubbwkwqk.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gtqtfweon.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guwjxszzg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gjbervuvy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqbzrzfvc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxkdponcm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/guyokgfam.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/guhwrdvhl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gzrwppeaa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gapozokjc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gryenxtas.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtryrixxo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gjjtytanv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ghlqxokbe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/galpzylhk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gvwyischo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gdhdyrsln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gyczxhmzw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gasjcvzyr.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gaoggswoi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gospagrev.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/grqxafmcs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gjvsfnbsl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gozooizop.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gbipddcze.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gyyoyckdz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gkvxfwsfb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gbptvbnyy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/ggmkswxyl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/guyhaeors.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gnhfirebz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gkfsivfaz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gjodlbpwm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvcxsksmh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gpxitljlm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gktmdtocd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gvqhajtqa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gjxbmcvoa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gpwacsdrw.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gbihpzbwg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/goqxwzfvu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gmpfmznvm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gzkrmwnlb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gugaqoxqp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gahttkuln.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/guyvznosu.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gclqbfzjo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/grwmzgrre.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gpczprkcc.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gmqxhnmlr.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gdhffkqcf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfifyvwbb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdcylbjhp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gukgfeoxc.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gewuemdfu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gjfejmqbe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/grjyxyski.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gzrxxotzd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gmsvwujmi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gtwkoipgh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/glyhehidm.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gzxmhfctk.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gekvlxtzr.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/ghetbdgwt.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gupqxcdju.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gvswqcqkl.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gkbkgvtea.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gazyabamo.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gwxoiuddv.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gsikyluvr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gksgzwyzd.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gvetmjhlu.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxekdarec.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gvckbrlxr.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gsjgdodfp.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpjpffpyq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gyzrslmct.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gmessjxxx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbpsdiubs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gwhcvblct.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gztkrltly.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gaqaytzhj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/grntluhrs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gcswlevnq.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gquowllbr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gmadqccsr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/grzhohtwe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gfveixbur.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gnalncocm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gryfskafc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gghtruvil.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/ghvfqjyov.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gqdpyttrb.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gndjkjksl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/grirajkkc.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gbzuaxeuq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gfwyqgxsr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gjkcqnbih.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gymjvkctc.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gxogvohru.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gbktgbbmi.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gqpfumdaq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gfffqivce.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gragwvksa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gwmpqjzdm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/grxjfvmbv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gvxhwdvwt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gmbkyxkhc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gsufeoask.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gqfecrbfi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gftshyekt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gftbfmacu.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gziyluzae.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbyuaggkt.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/guixrnxvo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/geqcvjpjx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/geetelgma.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gziqhblxm.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gvgkiqxmn.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/grjjtiemi.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/ggrijjuvk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/guopgvefu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gkhpipuxk.sHtML


<!-- 参考信息 -->