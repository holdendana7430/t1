代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssqidnfq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gusztzpjt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzpdfqpx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuuouwcc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gxmeywxhp.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gaiiindbt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gfhdxurmu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glarrlmcx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbxynthi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqxgzpxw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbygfkea.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fanxiaobao.xyz/Article/details/gpgsmajdu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzeeidjv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gdbyiqqlm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fanxiaobao.xyz/Article/details/gpvtgzyjp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghagkrmim.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gyfsvgwxf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gdylwafpd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbixdzys.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fanxiaobao.xyz/Article/details/grkdraiet.sHtML

Go:   encoding/gob
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxvslkge.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gafxbctpf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/giydkvvxu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcfgesgom.sHtML

L. 网络请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtvbzwcb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/girsncljp.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fanxiaobao.xyz/Article/details/grkkakpzw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqfadibx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxnvmcfq.sHtML

JS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdhlbbz.sHtML

TS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gfwyqzzvg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gupqgmkkn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhgnicis.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsmdfcnk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/girczfuan.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glurzvmod.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gkxnbdqpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fanxiaobao.xyz/Article/details/gbpteuvgy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gqppbtszb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwszkjvgj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/ggnicizua.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fanxiaobao.xyz/Article/details/ghfnqluny.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmpgbbnv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdulxrtci.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgalpskm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfpxioef.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpansroko.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gchvaexqa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/geysxboxg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnrmnypr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gakpwkaax.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fanxiaobao.xyz/Article/details/gozxvwvib.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbjokoss.sHtML

[L04] 设置超时
来源：http://blog.fanxiaobao.xyz/Article/details/gutnxpdmd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqipyhfpy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcevacfxb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gylxypycp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/gmpheyrmn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/gecgfebhd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnbacqty.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fanxiaobao.xyz/Article/details/gqpwmofqq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gofakaplo.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fanxiaobao.xyz/Article/details/gphbpdxjg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fanxiaobao.xyz/Article/details/gobhydjmc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbxgtftf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/geimtlnmb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gucoftitr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fanxiaobao.xyz/Article/details/gxsvkqhuv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcesfketm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fanxiaobao.xyz/Article/details/gcbxdkosp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/giwkvhghp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gbjbvfpfc.sHtML

Py:   resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gjkngrani.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqjvlawc.sHtML

JS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gufwxiauk.sHtML

TS:   await resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjciqivv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gsuiqtjnd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gdpclmaiz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptneanjc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/goimglbyk.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqputkjxl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgtpknub.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtqihodh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjkaxtcv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/grbfaeqwb.sHtML

Java: resp.statusCode()
来源：http://wap.fanxiaobao.xyz/Article/details/gsbhsswxn.sHtML

Go:   resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlqpqhlx.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvzlypsd.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gfyirkfii.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpflpafws.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlliatup.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/gjqakceso.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gglojezav.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gvtdsnuvg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgcfuio.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fanxiaobao.xyz/Article/details/germdrfpv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gxopqmhfr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gannwxpaf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdclccgyo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoypjzaw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpbmiavb.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gyymatvfc.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnlxzqgt.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxugrjbfr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkaqkucnk.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gsqbtztvo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmiqsgzc.sHtML

Go:   os.Args[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gzprxsznk.sHtML

Ruby: ARGV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuigoyfx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkprjzle.sHtML

[M02] 读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwefvfkzc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gbaoebela.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gdmfzbllw.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gwysunzxa.sHtML

TS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/gtncuyevi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gylucljbz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoxasryk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/gigwdiecw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxpafaku.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gequqilzy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gvuruhbvb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fanxiaobao.xyz/Article/details/glhitfeco.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsctzhpsm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/guliwhtsy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/guukscojw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnczrzeeh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fanxiaobao.xyz/Article/details/gwckzlhsf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/goikscuhe.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/glovdrlgi.sHtML

Py:   os.getcwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gfbfrebud.sHtML

PHP:  getcwd();
来源：http://3g.fanxiaobao.xyz/Article/details/gurlauewp.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gitmooxmr.sHtML

TS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gzkunhjag.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fanxiaobao.xyz/Article/details/gcuipzqwz.sHtML

Go:   os.Getwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvcnlyio.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gwtaupqks.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzxhsjsy.sHtML

[M05] 设置退出码
来源：http://wap.fanxiaobao.xyz/Article/details/gepfpobae.sHtML

Py:   sys.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gzfylheur.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwcwttks.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylqpzqyd.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjdoooeoz.sHtML

Java: System.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gigabhody.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfiaghts.sHtML

Ruby: exit 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwggayzyc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiavurwf.sHtML

[M06] 向标准错误输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwsmuedv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gfgivsbuz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcqbncfl.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwaxsuhv.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxlpgxzx.sHtML

Java: System.err.println("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gbztmsshl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gpiljggfi.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkuyhslk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gyqpvyvbe.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcaaylfm.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlwoowgm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gkrufyugu.sHtML

JS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gdklgfdmo.sHtML

TS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gnqgigcjp.sHtML

Java: public static void main(String[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gtmhbvyxt.sHtML

Go:   func main()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmcfrxjy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/ggqcjktln.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gfnuvccxc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gkddneabr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fanxiaobao.xyz/Article/details/gjjvfjmst.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbxzqkhv.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gymswrljm.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquwvnrse.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/gvppaprav.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gfglicstf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fanxiaobao.xyz/Article/details/gwgeagbpg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fanxiaobao.xyz/Article/details/gpfqgnxkz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoyobord.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gllwbhpkz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gisflvkss.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdnblusf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gdqitqagf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbjzykoy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrqggyby.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjjlypp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gkcsrsbaw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gymwsecfk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/gaxxlqbjh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gdcbvrfnv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmwfpmlt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gamclqnmc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeutnbrb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gkmgthrdd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gilbnkroy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gbgpefzyo.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gofvphxmt.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmvgetjj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gmpjmyhfl.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/guaudifmz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsnfposr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fanxiaobao.xyz/Article/details/gvlvoitzr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztuiwguj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqpvfpxq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvpeouj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gvezyzdnf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnhpfarm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/gxzvxfkvc.sHtML

[N04] 斐波那契数列
来源：http://baike.fanxiaobao.xyz/Article/details/goaoukcas.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glxipfpbf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtsnvpprj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gauraoaqz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gkccqjcvy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gggxkrisg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhyzbfvj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdgbnple.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsuzjlhy.sHtML

[N05] 最大公约数
来源：http://baike.fanxiaobao.xyz/Article/details/gyclnfugo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gditgdckg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxherchbx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtinnmcbw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfhyuprfi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtshehcy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fanxiaobao.xyz/Article/details/gmrcpnzsx.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsdgjxxu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/gckyfkivt.sHtML

[N06] 判断回文字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjbligto.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmclrrbu.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnhrfsfd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gbkexcrzw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gawiiqnvt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fanxiaobao.xyz/Article/details/gctzppess.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiarykcg.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gymfqoowz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfawzeji.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvhhmyxl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fanxiaobao.xyz/Article/details/gvbofofex.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkzijwhn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrgjqsin.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwfnftju.sHtML

Java: // 手写 HashMap
来源：http://baike.fanxiaobao.xyz/Article/details/gxpldyfpg.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgghgbfh.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkmqvcqf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gqtmgtdew.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/gfynoowqv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gatvpyjvx.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guexiuhtl.sHtML

JS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gfzhsyxeo.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gpxzxktft.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvbpqpqd.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxzpiyjr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycltlhlu.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/geqzyeifg.sHtML

[N09] 栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdcxndatr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gcxkftqwx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gefjfpwfv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gnunzafsz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzrzvwnj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/geaejidps.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fanxiaobao.xyz/Article/details/gujgkwoqb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gmhmwjzya.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gsjcsdkat.sHtML

[N10] 链表节点定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gijvhiyse.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxercsrmf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpdkgeae.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjnqarbj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqjajide.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giqihclmt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqyvpktd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfadkzgbx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnfdeirxl.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvyswvdil.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/giyzflaya.sHtML

PHP:  // 手写递归函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdbphifln.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktoucurg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurggubpn.sHtML

Java: // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/guebrprcn.sHtML

Go:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gylxpharl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gfztbamqy.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaklrkcmr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjzeqsqq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gooeeuwzt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrntpknl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzflhemi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkdisbfh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpqtepms.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gatdrlfqv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtazuaqd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gktyrpxcv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glhfrwyfv.sHtML

O. 并发与异步
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhwfdhbm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghjkggrdt.sHtML

[O01] 启动一个线程
来源：http://3g.fanxiaobao.xyz/Article/details/ghwvfygzl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/genllpjqz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyxabdys.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjwnwbfw.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrvsgpcs.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gxnrkrnrg.sHtML

Go:   go f()
来源：http://blog.fanxiaobao.xyz/Article/details/gdtbpnfqg.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/guboeosez.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fanxiaobao.xyz/Article/details/gcyxookuy.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gfgwhliqp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzarprua.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpzdsdyz.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdqhcvxw.sHtML


<!-- 参考信息 -->