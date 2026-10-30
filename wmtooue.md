代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gnylvqdct.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gosvclhnj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gmlnigegl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/guwjdsnkh.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gdcwwwtwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gfldprvxi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/ggspebkgm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gmtiiqfiy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gobdqycly.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/glqqucdzr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gizltrupf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/grijelohg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/glwafnnta.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/ganxyalrg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gqpkqtygi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gfveajoht.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gfelxzund.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gludqlmpg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gpwsqdaby.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gmvvmdywc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/goqytelfe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gafqjpjui.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/ggdzpxrhl.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gsrualcvl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gnnnkhtpr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/ghrabfqcv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gmefxvkyw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/goicmqmkr.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gzdwjtomx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gypavgyzp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gztselopl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghmrruncg.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gsgcgyzgz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glyefppsx.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gtwlfdcka.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gzoezixxs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gzvyobcha.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/grwnpewtw.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gxbjuiozb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gvmltoprs.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gusrxlliy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gvwcpdiuw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gwqluxmca.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gpkoioagm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gzgvdunvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/grbckmdkb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gfyfheshr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gbndojfzb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gdxuptuut.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gkhnbzbfh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gzphjiqhm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gfngqpaij.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/givjbtfay.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gtwcwbbuz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gbhijbgmc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gyegrxkjc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/guvdwpnfo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gtcznldpq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gaglyforz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gmtgnlgqw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gjapisoiv.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gblgsnpjd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gnlcwrpwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gpdknsplx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gbgojmmgm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gqvnjxued.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/ggiflwgqz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/ghsxekvke.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gyeycxxmo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gfxuwrdpt.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gyoovcqxg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gnweivoid.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gysvespet.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gjhdhyrpj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gsqzmgavb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gynjjetgd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gtceqawvb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gkbuzajvd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkewgofjh.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/ggvwlbafm.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/geyopgrri.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gtdgwlska.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gtfmrwnlh.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gtketxqyq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gjjnurfjv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gadhjkbde.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gmksrsrks.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gumxpcqid.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/grcfhbvla.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gppvxyfpi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gcjakdlla.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/ggigzxmsf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gzquvwsoe.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/glozuyczr.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gsfeiyorn.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gineivlzs.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gpauhykua.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gtswqlblt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gxpfomxcl.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gxuexuanj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gytvbmiaf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gcgitkteg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gxllfdsvg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/geilcpdoc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gslwpvkfl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdnyszkkp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdinbbuap.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gowdmbkeq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giuoiaguv.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/glogtbxhq.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/glwgbotid.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gigizcjxs.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gzqphzvsr.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gvobugaon.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gppzwowql.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gfdigfxkh.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gsmtabthk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gwoxuncpn.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gnzsllvsp.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gqlyyavqf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/grkolccvq.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gfnmjbzal.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ggvzgdfwa.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gsoplynnq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqgigghix.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gsflqsepc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gynplrnmd.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gqigrzlwi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gefyfhhwm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gfgaoxkzx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gexenwayg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/grdnlgjal.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gizsvlnxo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gsvanlrss.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/grwlrynsz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gpvmillgz.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnrcasvoh.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gdlzmixeh.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gkkdmzkgl.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gbpsrhafd.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/giuyduvyo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gzruavyri.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gesoxyxic.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gzmqidysw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/ggtkextqr.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gytopohms.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/goyzjvtcw.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/glfbbfbyt.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfecgmhan.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gcgxztudi.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gntebyfsv.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjvjennku.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/ggynzdatf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gkyrhsepa.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gnlqmaojs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gsswmebpc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gswgueysl.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gcdtpftau.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gkfchxcrj.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/glvkwyitb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/guzihuikm.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gtvlydhwk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gcjrprhrx.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gfvrreija.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gcezqoexy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gdumbbxob.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/ghqavbufm.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gkswkygcl.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gumewgjkm.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gdoczvpuz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gancvejnk.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/glfhcnsbm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/ggwuolqqr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gdnwnhjos.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gjvemhter.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gubnbujyz.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gpfccreda.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gvufxwegs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gyfjoxxjz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gytozircy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gjbbmqcdl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gohbhnoaq.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gyfyoqkwq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gemxgdyyl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gmshibhvq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcjkflgfv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/goebmdqoh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gjhsrcyiv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gzmxgoftg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtaupmeee.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwkfqtsic.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gmensrfwu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/geneacqqu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/glrboknae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gnmlwcxli.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gtwftnxzk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/ggenhvqqw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/ghdgzbciw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gjnudhqio.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gbxcldjcm.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gnvzzazah.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/glcrrwvio.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gmmpamtwg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gjvjjdrvv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gnjygfqln.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gjkcengvk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gzzpmckzi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gtvgabhvt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/grciprilq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/glvzmviil.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gksyrhcny.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gpfiavjik.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gnengreyr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gnyyfrhic.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmdrrdhlb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gwgwdlkyv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gcmqkvijc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gndjtaxyy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwyrtneny.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gnxuwqxyn.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gacqjxgrg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gnwungxfz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gkimvthpz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gmxdenwoo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gmwofjofv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gbbqeeohl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gparxyedb.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gxpkapble.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/grpnmvdlg.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/ghybmohfo.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gycjdsfqp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/ggydbryzj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gxenqglus.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gengnzjfx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gudwgbdwk.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gwyarrosk.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/goapuijze.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gudrjiliw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gzbuhcwmh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/govdhnrvl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gknjwgkhl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwhvuhpc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/ggecenydo.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gbtcfbbrn.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gpjnlincd.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gvpduanwk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/guiyiiuap.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/grczmzcna.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/guwxuoyyx.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gnenxbrry.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gmfovmzsr.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gugodzrqf.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/getxrizsy.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gaumibozj.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gxetvcxgz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gggvhbgyl.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gkiijpwkw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/guzyrjvhs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gzpkyxuda.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gdepqbasu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/glaexgyll.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gglbkqwsa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gcuqabsom.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdctnozfj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gmkbpgbjc.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gyxrdrohg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gvhhbngzi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gvyilwatc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gvhilkudg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfskujcc.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gfwgzhfoq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gbpqiwqgh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gmjqunrgi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gzerqouyo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gzzupeanm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gfxdzayxq.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gumcbzvrv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gtipjgkis.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggacmgzar.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gjncynwvs.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gchchjenv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/ghrskttmd.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gtlwrejfs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gcpkviswy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gzoajemmp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gwyakuhtl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gehzfkvil.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gatctjcei.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gladtqmfi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/ghibuajpq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gljkqhhad.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gsxyshkyj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqhsavyzu.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gamtnnmoz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guvakmliy.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/ggwtxkscl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gtavwltsz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gqajkmvqf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gcdqtofuc.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gwjacipas.sHtML


<!-- 参考信息 -->