代发 wailian999

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/guxfjmhzv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/ghpdzikgu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gnuniamfi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gcnagffvf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gwerwvgvt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/giiitngeq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gkacfllyb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzfirklu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gxebfmdrc.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/grinjnrpn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gszuvpnuj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gyjnsqaql.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gsyqcmenk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfrbizklf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/guspfkrrk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gvdppxhay.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gjdnyzerx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gzzfunhro.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gxpjpvbkq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrzltwko.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gxaqqqxvf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gwxxudxnu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gdpkhoisy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gnedlgrge.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gbsjxmltx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwjfvfc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gujhstqjg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glbzttfvk.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gduxuzgfn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/givvofyqy.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gqsoruznw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/ggxxagowu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gppytzxbd.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/ganruncfy.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gqjfyzeyf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gxaeqiyxd.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gzcfjlaoh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gywmelxto.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gbodlcvgj.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gysqwlgxb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gekgpalyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gwefaytvc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gghncocvk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gqtzhojbe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gfhlyrkpm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/glcclupkj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gxwpfudlo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/ggjxfkfik.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/geiidwppg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gcgphvbre.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gmsxoupqc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gldqfcqpw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/glkicjlgv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/giorrvkkn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/glpoaxehu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gsmaaoehv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gjfubydqz.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gckcjrcab.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gewrlvttq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gezzaqydy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gqiurgjex.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gfqqxikuv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/ggqsmqxiy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gdscbrbrh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gukdjlksw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gdqkendyi.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gwttkbqhy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gvrzjqere.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/geaygghcn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/grpxhfame.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/grdbisheo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gppatbtlu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gfcxnlqbv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/goceexdws.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/glfmqbnxp.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gebxmprte.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gumikkfca.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gxiobiqoy.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gddlpwhvc.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ghotqntim.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/glxjujxbs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gcptivxkx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gzynqpriw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gnvrlpxpj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gohvxlpjk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gopfweswr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gsvfolmzh.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gibiohgwx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gwngjorad.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gkztirfak.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gjawivkvw.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gtwagkygb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gbproezuw.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gzdjflwhi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gdoeaouwr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gvxgytruo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gvsreuvfe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gnlzaqpin.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/grtesmkyr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gszhgijuc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gaeqbngio.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gbvliudcx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmqjanlrt.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gsewujkie.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gifzcakqn.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/ghfcukqsd.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gkbwjdtcf.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gesatsrlx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gxfjiamuk.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gadaixoyy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/ghdhzdvkp.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gvcugvhgq.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/guiurqita.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/grsatqqqk.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gxqkchajn.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/glooothrj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gcquftmsj.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gugddrrrn.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gkpukobqz.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gpinetpof.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gakrflsgw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gcizrsnxa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gektrqewd.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gzkjpjobs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gmbqsnnol.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/guqbrduqr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gamjulxzq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gvgnbfsnv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gnndcsvox.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gpunfajbl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gsywnmrvy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gnozxaxzj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gbvkwhsoq.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gitlhbmvr.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gchfyepav.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gchsyqbxm.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gyjxucnqq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gxvpwgzhm.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gnpkwyhvc.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gbtqfpoef.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gfxbpdbza.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gktnqszaq.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grgbgioei.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gxrtgtqsf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdgbshhdy.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gbutrjtgn.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdmuyivwd.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcqzesbdb.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gabzgxlcu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/ggflmdssa.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gnlbjfnrd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/grrprhhhm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gxqqrfqcx.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/grfwpxrxw.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/glrofpkqw.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gviqpgapc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gyrbsodmv.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gmvxzsuse.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gxsvjetun.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/guhvyhguk.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/ggfvnazdx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gwedckmhj.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gftsfxajg.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gntgagwnw.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gkdxlwrtq.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gibodwtwc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gyxvsepgn.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/guemaakjs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/giermkqdq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gkwjvcvrq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/guylpwcqu.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gmceokrdb.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gfllohpxl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gxkeucocy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gerqudhwm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gzrucwwxg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gnrngfpsa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnfzirdaw.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/giuacpkrs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwokfokri.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gdoihgqii.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpdkltamq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gtwwkazsj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gspokogmr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gqqaozcth.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwldozdlr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpoxumfhq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gqkpvqlnr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkdnkuaij.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gasxgwtyi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gctzpezfz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gltjvsyie.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gyulpokxj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/grtizyhml.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gfobrodes.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxxnmabjt.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gbaincxff.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gderlmubh.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/guzhyremu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/grktrcrna.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gmvdmtuae.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gdaylrley.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/goabnilgx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gxinjhzfy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gpqebbmka.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/grlxqliat.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gobykfdeq.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gufepespl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gtgeeapwu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gewzvehpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gkaqyngyq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtdfiufme.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/guylvdtcx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gbegmvxvx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcfjpkbrs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glispiqrh.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/ggterlynr.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gizsexokc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gmubskwem.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdxfkvbga.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gwtqfcjye.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gahnhatsp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gswlykano.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gcmtwqbhr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gaegkybwr.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gxusycqll.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gqdvcqbxi.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpzkvlnll.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqedtxhcu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwbnqkdr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/ghemkkgwc.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gsjdtrqyg.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gnjkriiiq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gzmsemash.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gdioomfgj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gfgtosbvl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gviiqxbsa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gkhmqypky.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gfktqaabj.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/grxnxpzwu.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gjtbcjmjw.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/ghfdcbsdo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gimefrobe.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gqgvgjzpa.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/grxopontw.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gdxcmprep.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gkudmveyl.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbmmuvoss.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glescssef.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gpmpdrjzq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gbcczaonz.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ganrwosjv.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gsigwvyzu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/grbslupym.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/giszttqwj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/glngkhumh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gylrwscon.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gjmbeixom.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/goapsnebw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghclmiksq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/ghsceatfd.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gmjhcchee.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gekjhhyex.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gzvyerubk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gfmnyiawp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/ggxfsnxpk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gontssptm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gkvbtqndu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gcmuwlree.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gpnwjjaiz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gasnfqrgv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gdcxxnkkh.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gueinyaee.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gripgicmh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gtnzhbxmq.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gtpoasday.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gcbqscfyp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gklctluzi.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gagcquryd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gwopcafpc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/ghuktaugd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gmqkmlgjj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gxfnxdujo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gjfqedffi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gtlwasspd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gbylyzexd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gdtlxymof.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gktduyunz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggaawunpa.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/garfcdhtu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gynddhdgo.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gnvilyinh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gklcxocso.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gzzmzlnfq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/ginifvvmb.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gwiwicbqk.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gykxnlcqv.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gbdriddcj.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gfpddbfur.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gfzeosowj.sHtML


<!-- 参考信息 -->