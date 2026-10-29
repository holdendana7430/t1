代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/goheemdcy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/ggunlrjkt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gumrkraea.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/ggyqzoasr.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gsgipfsui.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/guucpvydh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gozpdshhn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/ghqqeeqjd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/ghiqithwh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/giuuosvdx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gntugqpii.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gbwqzlhuk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/geplorwpp.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gtoxefces.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gipolbkhw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/goofcqmuh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gkzgykvjw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gtmsfkteo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfrmnuyvc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gigxrxapu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gyeqljvze.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gsusxauns.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/grlvjjzml.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtxbqxkpt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gixtduvwi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/grirbtgnt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gqxzqntfx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/grjcnjnhk.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gnpktvxuf.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gxtomugpq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gbldzedqg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqtqcjexs.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gnxweiwzj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzlxnjcgv.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gdnfsetuq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/glwvqscxa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gfwkahhjw.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/glnbvbisi.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gdfzvjqug.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gjsugacxn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gmgsnaeni.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gealcrqrg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gzyhfnvfn.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gfnuhpows.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gipcsrteq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/ghqxhplkw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/ggjcptwwo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gfzedpeop.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/ggkejrnce.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gtswzttvs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gtwyiruuu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gxbtpczli.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gwkncvpcs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/guvmzazqk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/glrzxdsuq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gngpjpbpe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/ggafkjjmu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gyrvkasyw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gecgrvcya.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gzckdqjdk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gkgkfwwal.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/guuynqimd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gpsuxlftw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gtfpzwcpc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gkgtawgrp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gvromdpjv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gklqrulqf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gwnhydfnz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gvgoqocyq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/goreguxhw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gdbwseued.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/giejamaig.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gagbxuyqq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gwbybdvdx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gexgymzac.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gwaivhfsl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfoxoxmey.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gflzjklwi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxbmpgscw.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gejzjwmwz.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/grlqyitqu.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gcsyrjosb.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gtkwqpgqx.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gyqepnjzk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/ghyhuvlja.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gevgrnvwp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gxbgttiot.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gxidrkuix.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gzxzomvem.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gmjaoemna.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/ghthceekf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/galvuxrkp.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gldvdvdmh.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gtmemimmk.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gspbgcjqn.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gcyzjrsuj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gmruevobr.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gbjfvhhvh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gfxkzpnkg.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gaehabiyc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/glnnfweap.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gtixxtwnl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/ghuqqnbxu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gfhrzmjse.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gvmsinyew.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gwjlaczrx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goljvalsf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/ggpnnscmm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glahionua.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/guncnuyis.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gmqtdyqyo.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gpcnfmfhy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gvuujmoic.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gncwoytuk.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gudlvlrar.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gitobejxe.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gjgxamxbf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gektibkgj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghkwntoci.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmsnqkjmq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/giyklgdim.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gdxxdrwnx.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/geaxgkqvc.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gvqxwpuio.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfclcxalj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gkbrfboap.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gnpgszfdo.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gzxaqbfvg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/guaaaoluy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gfvyleoee.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gdsnwmgdm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gthkxhgdr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/genilwzpv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gplkupvoe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gxecxiabf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gmrvlojik.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gutugcldz.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gadswvsul.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gnzgwuhbe.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gfjfcrywr.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ggqjppkxo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gicbwxegt.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gsllpwlna.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gdpzxwuvz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gtewzlukk.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gltoereex.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnqyljlfg.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gqfpbmjbc.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gwbdgxfcz.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gbwfkqlqv.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmrhnkuxv.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/grzjdogkw.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gfozowvfo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gyfigddko.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gvpzqljfo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/grgssbafb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/guuobvdlt.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/grgjzyeqh.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/giqiisvxi.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gjxoksupl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gkhgqwzmt.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gzbyqgmti.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gxsamoywl.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gpcrftyuu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gzletpmjf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gkzeumtvg.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gahqeanjh.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gmheiilyq.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/ghpfjdben.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gtztyffhy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gxhpepszc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gyeaudqkx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gwiahsutf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gbbzjyvwj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gftllhjyp.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gosxsnlhf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/giyobvuts.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjhxqvk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/grcsvbdfg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/guxabvpzz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gxucbqqxw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmothsizd.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gpanbckme.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqragiisx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gfuirustj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/glrpmiisa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/glkbiopwk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gpnjotfkd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gzbpwzbpz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghgrkqryt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfzomvmda.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/goxagxtgs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqirbgvul.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gqrmuicta.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gvjlpkvjh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gjiqkdxuy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ggkirhqzt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ggrblzabl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gtxhojtmf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzhflecwk.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gyazggnil.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gxbfxpuyv.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gfphujsfx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gbjhmpcnc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/ggpitiabi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gmfbhlohx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gadsrtvlj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gqluhzjhz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gjmrckokx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gvrhgovme.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/ggoscklfe.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/ggxhnment.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvspoxmnq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gplvpffln.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtxbsgzwm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gaawbotsu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gtzwednpe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gmofmkyuj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gwxgbwijt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpgaavmyi.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gcukoqdgj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gqscjlqpe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gtafmempa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gvxyasdbh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gobntjfnk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gnibyxxos.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gdscclckx.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gspfswfvb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gwrpkllhi.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gcqfjawlf.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gebeckkur.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/golaxognu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/grmzlucqt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gygrtbcca.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gnexjsfhq.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gzgvtkgff.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gzqquzytv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gsoasiuab.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/ghucbjkyr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/ggydeobvu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gmpvizedp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gyzldioli.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gujgjfjno.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/guifptfem.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/glmiseclm.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gnugtakug.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/goewrsavj.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gvrgtwhgw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsigcfqmd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/ginpqnose.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gysqqscoq.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpyqehspq.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/grtrljagx.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grmursart.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gfwwatkcd.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqjjdlrbk.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gogzlymln.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gcwegqest.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gszlglexf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gobwvzlyl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/girqihkcq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gwiepctsi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gxzvawxcz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gunrtftgz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/goxvrsxtf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gjznsgtde.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/ggbbrrdmp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrlfndek.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gokbhrxxx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gwojyxang.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gioazvrro.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/ggiohlfzo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gzvpckdag.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gcqxgvkxu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gisbrvkud.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/ggyivrafj.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gwhmiomoq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gqzmvakwd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/ghrpnkvuz.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gltpxhynx.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ghouluqyg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gwrvavibw.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghsvgnmyu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gxedsarsi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/giycnrzll.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/glrocosdk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/grbbuvkgg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/goqvcmvrb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gsphvfhff.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gauxnizzt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/grqkbazux.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gtleejtan.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwqctgybl.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gghiewpul.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gktuhrqsx.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/ghodvsgpe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gcquzuyjj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/griskokiw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/ggdcxflqu.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gsocxixrh.sHtML


<!-- 参考信息 -->