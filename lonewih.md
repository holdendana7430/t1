代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/goajsmyms.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/glawyuucm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfznekwx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdbrimq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguxtincp.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwbuzow.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gifuduror.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbvmaetd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxlukefa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfpghdbc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghonzoxwb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjswskth.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssiiabla.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gcnxjfakr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fanxiaobao.xyz/Article/details/gjrraexjp.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/grujiphee.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gohlsxean.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/ggssprsnb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/ghombcolz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnpkdjxh.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/gvgdzajur.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/guhokoobt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/ggydchqxy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gldjpamku.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/geatbvwbm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwahpbxsv.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoctifzm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gfivttzez.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fanxiaobao.xyz/Article/details/gdobrusto.sHtML

JS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgnocrnl.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepwugsto.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fanxiaobao.xyz/Article/details/gympeofqr.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gbifuuxhf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gishzvljg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gujfjwcfx.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjipuews.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/ggnfiijrz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyfjkdnp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjytgysaq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gshdrpgec.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gpxffucwp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fanxiaobao.xyz/Article/details/gshgtxvvg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxhvulsm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxthmggok.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkguarrm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fanxiaobao.xyz/Article/details/gzshnjjqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdamdibx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gbtpdyxrl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwrobeir.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkudekhg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gulxciiww.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscyfehnp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gbaifntpy.sHtML

[L04] 设置超时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxsgfbok.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpedommt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gospgdarn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gjwmuxyyb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfmejdea.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gbqbqrmnf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnckoozni.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpxabjjm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gakkgggqh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjwdqnja.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gencgkunq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/glsqboxdl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gmzwntdch.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbayeigj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtxvglv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfjcwrin.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfgmhtbq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucltvilf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gwalbmjpp.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoovnwdm.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gquargzim.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/glrljwxks.sHtML

TS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghswpwxti.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/glhzktiny.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fanxiaobao.xyz/Article/details/glndjhlbh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbpatmxb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpafwjshg.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/guzexuugg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fanxiaobao.xyz/Article/details/glpzhcpxv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gstsszwpk.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqmkzzgy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gizvowyrs.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrwulddh.sHtML

Go:   resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwnittic.sHtML

Ruby: resp.code.to_i
来源：http://wap.fanxiaobao.xyz/Article/details/ggrlpnrmi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxooinxq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaspogjsv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fanxiaobao.xyz/Article/details/guaewlzqe.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/godlgmfzh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrfhkhdk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gwznvtuzw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlceejqw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/glfvhrdwl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcidyyjqj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gafmurbag.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgbekcap.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gcloyadcb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grjpoennz.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcknpppch.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqaefexw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fanxiaobao.xyz/Article/details/gfgxzduxr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxsybmtmb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpnudnnbd.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvvadqlg.sHtML

Go:   os.Args[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/ghhqsjhwd.sHtML

Ruby: ARGV
来源：http://wap.fanxiaobao.xyz/Article/details/gbhqqyzkl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqtsrkfn.sHtML

[M02] 读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmcmbljky.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziicqdof.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/ggkttzimy.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnjxaotg.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gmsellmuo.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geidsagea.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbeyygcm.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/grbfncamv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmozejzj.sHtML

[M03] 执行外部命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gskcmlfkg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fanxiaobao.xyz/Article/details/ghkefdyxd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmhcojjb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaqcrmzp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/ghirwdzcw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqwxflwc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhxkgjau.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fanxiaobao.xyz/Article/details/glqwjgbzf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fanxiaobao.xyz/Article/details/goksrhewr.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/ghjazuong.sHtML

Py:   os.getcwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdululse.sHtML

PHP:  getcwd();
来源：http://read.share.fanxiaobao.xyz/Article/details/gecghctfl.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/guuqbppln.sHtML

TS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxhxllkq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gdgrpwprn.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkmrrcmk.sHtML

Ruby: Dir.pwd
来源：http://blog.fanxiaobao.xyz/Article/details/ggyvvybmr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fanxiaobao.xyz/Article/details/gayjauypy.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndwpwqy.sHtML

Py:   sys.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghhhfaxaq.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gjwovkgsj.sHtML

JS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwougxsfu.sHtML

TS:   process.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaknhfle.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbckzykh.sHtML

Go:   os.Exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbzwulso.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmuhgpfv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fanxiaobao.xyz/Article/details/gxerutfbz.sHtML

[M06] 向标准错误输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjzycdqb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazkmvric.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/glcfkuerb.sHtML

JS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/glqfdqyik.sHtML

TS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpeuqkac.sHtML

Java: System.err.println("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwnbqqcq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gpxiseolp.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/grjltycwx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoacjgqo.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/gzemmfcyl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjsmtptd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgpevavp.sHtML

JS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzcnrldn.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gutgktklb.sHtML

Java: public static void main(String[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gnrqafkbj.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/gitgeycfr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfqourro.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/glprifdzt.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gzrobqkof.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fanxiaobao.xyz/Article/details/gplmqudvm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fanxiaobao.xyz/Article/details/grfttsfrp.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gqxqpnhfm.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpelizib.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjywvyqsh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/gasucwxav.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fanxiaobao.xyz/Article/details/gejzpmkbq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fanxiaobao.xyz/Article/details/gphinggwc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcbhhmzb.sHtML

N. 数据结构与算法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknfcryri.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkozuyrnw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxhcjgla.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmfbxzbro.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbekutbqc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwtkyigz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwosyaerz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/grzewkufx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/giwnesnqb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gknnpvktz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyjqtlrc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fanxiaobao.xyz/Article/details/gkmbogqbt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzshvyidc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhuavjun.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfcqqvtr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrykjkfr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdwxsmxr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gijaelnme.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbdvzaxg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoltnnal.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gdfyuibjj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fanxiaobao.xyz/Article/details/ghigzpqvm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/gjecnhmgd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmzgxley.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvcukmkj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gacpzxsmw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhqhzsbc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fanxiaobao.xyz/Article/details/gbqtpphqc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fanxiaobao.xyz/Article/details/gjksfzkpy.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpugyeop.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grhkcajxn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsedxxeb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvghcojr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjipwmrny.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/gygilacsl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfsqtnws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjupprxm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadruchud.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggydextub.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gigkfffcn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glazgprcz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghxtopchc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjkottus.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gftmywpeq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/gqxdrmehl.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmnhlaeg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfxfhhhjr.sHtML

[N06] 判断回文字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gssxyppzr.sHtML

Py:   s == s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gdxunhqog.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmsrtvvo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtljxxqp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/ghexhvbxv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fanxiaobao.xyz/Article/details/gvlunddck.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gyxctjeao.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqotccif.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gudpqbsvv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoutxdzg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoejnlcs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvenxcgsh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkmvhpvp.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fanxiaobao.xyz/Article/details/gxnbdwvng.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbdiozym.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkzffruo.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrocofgl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebuaeyjg.sHtML

[N08] 生成全排列
来源：http://wap.fanxiaobao.xyz/Article/details/gxenowxcr.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/glokdxvtx.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqqluagd.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/ghezfjnys.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrshdref.sHtML

Java: // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gksdqmhch.sHtML

Go:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gqsroyvdt.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gdouakgjr.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpheugkt.sHtML

[N09] 栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gwihhhcta.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxplpbmc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghktfwoxa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpmrsiyc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/gslhjliil.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gystqwvqi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbujtkie.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gzimiitod.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwmmsvkm.sHtML

[N10] 链表节点定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmgswwob.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fanxiaobao.xyz/Article/details/gbdbjphpb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpujeckhm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gnzykdnvq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gaqunlztb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghiowtzjs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fanxiaobao.xyz/Article/details/gwabwsbok.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdmipdwy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvxytsex.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gndgwuemq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fanxiaobao.xyz/Article/details/gtniekzxn.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glylfqpka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glakqqvbl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gmrpnkmvi.sHtML

Java: // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gdinkacoe.sHtML

Go:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gxczdzxkk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/grgqzkqoa.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gtapuvzxd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvknpavcu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbzgkfmw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/gwzqqotpw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gojumxlma.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gczfflimx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gnsoennkt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gwunnbbon.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gilrtqdge.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gvurhmtst.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemqpzeq.sHtML

O. 并发与异步
来源：http://3g.fanxiaobao.xyz/Article/details/gtmhzaehv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghagauxsg.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtjyhmyh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gehpymvqf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fanxiaobao.xyz/Article/details/gbhcryfyi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fanxiaobao.xyz/Article/details/gganfizku.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gafkidtag.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gdopfapsp.sHtML

Go:   go f()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwfoyipu.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhxyphzw.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijxmzyen.sHtML

[O02] 使用线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwfinfxz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbvgapio.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/gsycojcgd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/glwjovcsi.sHtML


<!-- 参考信息 -->