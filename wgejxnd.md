代发 wailian999

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gzyqqffrb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gatezimro.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gfikgsffr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gocebxlfw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/grllvmewy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/ggdwfqsqa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/glozgpqup.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gmvsxlxai.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghkdhtagj.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gtdqcalys.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ghivoclyb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gxctaqmyg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gzmmtniir.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gjtvjcfjt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/glnudloop.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gushgwoao.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gjtzluezt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gpbbqnpgr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gupkqgyre.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/ghxcnmung.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggnalmwry.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/ggziangzx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gwtdbantg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gopvvpmtk.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gwhjawrdt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gsmbvibsx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gddnwfbef.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmpepqvbn.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gijsnetci.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsjgvgoch.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/grcizrhcr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gweqrludp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gggvsdidg.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gxjlvgbxl.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/ghmpsjitg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gbttteviw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gomcszgmx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gaymcgzrh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gjgylnarr.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/guirkccxz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gdieqiqpf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gqqmqwjem.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gpjythiho.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gnfcyiiis.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gyttqpokn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gbrsjxjrd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gjyevwabi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gkdyhderw.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gaitapnim.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/grfbiqplk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gzjonerwq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/grygzpwfp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gkwdlcczr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gbuemjczp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gvecjtozt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gdnjdkxqu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gfhddrjdy.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/grkccpnab.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gwymtxprz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gggwifjrj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gyduuiivm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gwzzwbmzc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gfmdcwkyy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gaynrhnim.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gbseqtjhi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gghlrlhqw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gtnqhtaxx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gibxxhfdx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gvkhnnpdf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gujeqtvqq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gtgpxlpot.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gmoqksoqp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gsbaamtbe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gaqhcjkgi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/grxfvaupp.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gfkynlean.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gesiittas.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gujdvcdrk.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gujeuozpj.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gidobazqy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gnrpjahjl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/grzuhpibh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/guurqvbzz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gyxigvhgj.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gkcxsuqlw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gtnmliubt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gmozzvcrq.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gtncsyweh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/grsqcnxrv.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gfcrkmrjm.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/ggadvpvvi.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gyrccspuc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gpaygtflt.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gdpjvizzi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gjmgjmvgr.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gfzgznioe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnmavcu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gwrrhhimq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gftlzyomr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/guvfsrtte.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gdwecaurl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfooigazj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbroemwyd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gutxsccjy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkprxcanj.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gjgndfeti.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gcvardwlc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/grtnfkgnc.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gufmqjhuv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gohwuecns.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/ggxgmtvnu.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gdlkdqvxk.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gcqctyuxc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gzbnuzqxt.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gaqbcydoo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gtrqadnlp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ggcwlieab.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/grenptrvi.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gugbhoxsd.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcqxinstz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gihialash.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/glffwcdnx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gnhycvzaf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gyasdybeq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/glyfjpyus.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gcukkmloe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gupsntsol.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/ghwqaidwp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gtqcucsei.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gbcgjgxad.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gwtrwught.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gncqiyrxf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gsiuwdffc.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/glhpdnddw.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gjtcsizva.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gssevflju.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxnwzrhya.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gcgqktbpb.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gnwofkito.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gcgzeqbec.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/ggdnxzcnz.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gflbetipx.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gyobsdkxi.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ghvnpvpjg.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ggfiuycyn.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gfgoghxvr.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gfnmhooae.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/ghhhaaspz.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gwmmjrczf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gkngbwqbg.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gsbenitrf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gozxwspia.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/grjvqrhic.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gboginbbd.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/grmpbyowe.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gdovjwhxm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gmvqhevoa.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/giskaoswi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gznmfeshw.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gxhmihebd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gekmfixdg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gqwjwoxud.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gaubmtgmy.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gyvqclsnk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/glgrtfiqd.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gcxzazqub.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gemqrgwrd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gxvelgarx.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gnxgpiqtt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gqfflnfwp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gmfprzfhk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gsnkzhoza.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/ggvhevshb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gwdsiwfoy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gwstowmkm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/ghsrxejna.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gfwwbwwjo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtbkzhlml.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gzspaulfo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbbmaybov.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gvbepfeab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gtzyabifj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/ghqpjxenk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gwuvyeaam.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gvfeubrcz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggxkmnzir.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/glzsxfuza.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/geaxxzzuv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvqrcrpvl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/ggzrkzxhv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gtkxgpzpj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/geimjxmqa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gwyiahmjs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gmiqgmcrl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/ggrgrtwtz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gneteybgq.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/ggwpjapqr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gcohtyzrz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gzffpvwrm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gqzmlubqv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gwzgssitx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gbylthucg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gdoqapwax.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gsrnoceiv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/guihbpgiq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gcmewpgay.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gypdvpgjl.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gtafluyzx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gghorftsw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/ggrellive.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gubkmmknw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gtpjtnafm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gicvexclb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gyumvynmc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/geshzhcbl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gxrqozsiy.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/ggneevwew.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gjviqnvpa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/ghordcqaw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gyzyjzslt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gjwqikftb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gpjausyvj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gsmmeixtv.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gktqmhmpv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/ghvupkdgm.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gktnhfhue.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gbkubbqkp.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gllszhofu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ggowbmjfq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzvgeqceo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/glmbvatwf.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gpsgmmrkg.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjtnrbkxl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gfvpuiirn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gmaaamdbn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gaoppcbuy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/ganzqltpa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gadsmpoki.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gzjicecdi.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gyzpuspte.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gwrthdstf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gemvynkmq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gwshwgkfj.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/ghqmgoprz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gyjpxubse.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/grmublhkc.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gidgliwsa.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzlhgctuh.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gtvzqunpk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbsyfttpz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gizmxpohh.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gubobwras.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gwykjwubp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gpyjbvbwo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gajovdpgp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gesmwvdvi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gwovkupqt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/grxqujeex.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gqkovcwcl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxanwqeow.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gagztrxff.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gldznyqns.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gqdpploan.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gozfsaegi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gkkgrlrpj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gahjlqfyp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gvrpinzki.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/ggwgxsurg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gmsejlfud.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gzlkmbypx.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/guvfyoych.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gbijpxqbs.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gticuaoct.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gifhigvva.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gunegbzxn.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxljjrpiy.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gtrdohqce.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gtjivyyyv.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gqpbjzuol.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gpjxfnsri.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gmqbfpsuq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/grvqenzoz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/grmeyhkyx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gucpgotcq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gxnuafarj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdoycjpv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gzexyufjd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gdunismej.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvslzwudv.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/garvbtqpl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbtpvqnis.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gxvytwwbf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gfqfwaifw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/glgijojsg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gndsfecjr.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gqyzkppjm.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gqsfbaqci.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/guhfnbkgp.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gygtwrzki.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/giytmswzx.sHtML


<!-- 参考信息 -->