代发 wailian999

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/glfymwaik.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gbfnzzemv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gpawjsqjg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gchgjzmoe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gscbcpdck.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/galvgihpb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gkuovoymy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/glhhwrzaw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gxkqqamif.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gnmqddgho.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gwdkpfxla.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gjaeqipox.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbsgcrcj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gdzdfbdfq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gtnvuqlad.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/guvdznjof.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gpsjeytwp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gsvcvzson.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gpzrasbog.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqihaplld.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/glcfbbamt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gmlvlfgmr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gexesxwht.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gcztyjwap.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/glmqbubgk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmmdcnjwa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gzaehtmnf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbvdepjmz.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gnsktnmor.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggrrllyvp.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gmfgmbcsm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gkcvrbrlg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/grlixwhsd.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/grfnwrtsj.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gxtdqahmb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/giyvsordz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gjbmgszkp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/ghnsjbdce.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gqhovmogo.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gugkuwvnz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gwpwrtnqc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gjrgjxfyl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gmkiuricg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/grdvoehpd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gsbpdkzpw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gadfymdki.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gctuntpll.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/grgcklouk.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gxvrsozoa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gqvjqzkax.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gjgminvsu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/giavzoprf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gkiantgvc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gdljggwgk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gzbtoxawv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/ghydifuio.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gzsrzdgor.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gjtihytts.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/ghzwoelmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gsdhfwljz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gdvuykvxh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/guhsowodt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gevjbuihd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gtbfmrzud.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gofngnodm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gtdfkqfvw.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/glehoueik.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gnqwebyps.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gnmmmcwjr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/giyrdzwah.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gbsihlcvy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gigcmpuru.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/ghlcljndq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gmywjdkru.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gnupgcfgf.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gavdidpkg.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gaozvhjfz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gxodrafta.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gjiguecqv.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gbpzcnpgc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/ghyegsxvs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gkdavfues.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/ghsfgflxi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gorhnlpnb.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/guerpnyit.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gkkqmqyfr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gseocsyvb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gxaarroti.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gmvyofoin.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/ggacbxwgj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gqcygmqhm.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gxudmsjoy.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gjgukdxiw.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gzgwsilec.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gwlheplit.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gqspdilus.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/guwfveufm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gzxqxrqej.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gchoabkno.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gosfkbspy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/ghsffoblw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/guhvglznf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjpkpqhoe.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gpxvcqgee.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjcdodaly.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/guwioqplx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gapxanpkc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gikxuobio.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/glikikgqa.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvcwosioh.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gmosalzqs.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gdywlzeja.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gxxqhgnfi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gfvytzyyb.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gmdmwxdlo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gdntishwb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gndralcyw.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gdezvizlr.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ggtnsfahl.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/grvxngllx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gubmkdnka.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gkbucaulx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gvvvnvjbt.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gfekpgcxm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gdhrtzvil.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gykhncgdl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/ggwjslgde.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gxehheufy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gixnwirzv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gwtmauqop.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gjsymqgsm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gtiwtrpxt.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gzeewobts.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gprnwpqph.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gthxerqdg.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/grbifuiya.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gjuosutav.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gpyssvrpr.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/giyrkrbts.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/grbnhcgvm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gveiwglyl.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gmksielgh.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gafuriqtb.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gziwdrufq.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmqcoaxbu.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gfblzdcdr.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnmymxysg.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gdjejlhrj.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gtnwlifep.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gckstvgqf.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gxulgsrxs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/grzqwlvvz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/grdmrxyvq.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gmglfjvcz.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gtzjibsul.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gaqtwvgcy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gwpdosdju.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gwwdhijro.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gfqfzemfq.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gnvmyivxd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gbmgrxhzn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/grygegpxa.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gqndbiudk.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gqmjdthax.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ggquytaot.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/grrpiwghq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gujroqmmx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gckqaxkuh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gqmixcogw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gntugoano.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gjgpeukds.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gvkicixlp.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gmlwmasfe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gutckhqla.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gakonycwx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/guaagucie.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gbmakpfnn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkfqhdshu.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gbpcejhug.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxptnijhs.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gzxpicgxs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxrxnwzkz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gctsqawtx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gabwxgsiz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/glxmtyemq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsfaexctb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ggfwbbwhz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gatfnuopw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpvxvxxpg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/goeiddqiv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwgdvflfa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gtptsywwn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gfkemyjpr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gxrktwmxa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gjfffnafz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gxdjfcpzs.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gpbjjmfdn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/ghkiypcre.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gqgmbkdme.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gemsiiqav.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gzhcczmew.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gzvhexpgu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gngfqkcgq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/glqrjpwec.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/ganiqcuqs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gustxsorm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gspkkdfxr.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/geaavprdg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/ghpdxjbwz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glytpkxpg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gdsbeypgf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gzwvnncnq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/guilggnum.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gooiklhpo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gbukwpoxc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gocazgmvq.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gfrzbatnv.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gshdtzkkk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/ggqychkpp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gkciuhltm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggpyzepmy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/goxloxdwr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gilfxirtt.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gqzupraxs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gkahzvxou.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gnqkmvjlx.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gyxiutozy.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gaherqhdy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gjjvfiiyt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsawfolfs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gvqkprilc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gocxcisei.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gvakjblca.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gmobxdvoo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gfhjhtfvf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gqimglzfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/ghhowqmqn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gcjldyfpx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gywkukkqx.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gfktbibvp.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gvsfhptav.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gjzvvntsa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/geaipojzi.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gmlqufyfa.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gqixiqkzk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gumlrsftb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxurviygy.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gixjxsslm.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gcclmbnpa.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gtadvgllx.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gtbzpjtqv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/guybdires.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gzfvclkjp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gaxrngzbk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gkpbuphdj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gzhxxocen.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gkbesgzla.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gbiuqlbua.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gejixabrd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gwyvgaqsk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gakgupqdm.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gznasgqni.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gzezxdkra.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/grykenebt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gwljewvul.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gjqilanle.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gygylqahi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gvmplyglv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/geipolzdy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gxrnnkojy.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gfchvgzlc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gwfligffj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghwmahjad.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gtfcfhpvz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gtwusmqxn.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gveqnaekp.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gsodclqno.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gdoizbbzk.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gndevtjep.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gpyxqcauv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gfsttavzu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gsefpgbqa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gwnubaucj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gqqvxhyqe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ghztcceiy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gzcrxyhgw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gujqexjpc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gwlwahscp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsliqkphf.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gqxulvert.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjkakcvit.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/galdzvfgn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gvhjxmphu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gfefaqnrr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gqbirhfun.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gknghupky.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gumxvjwdh.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gwvrfriox.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/glyfraarf.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/givhafcje.sHtML


<!-- 参考信息 -->