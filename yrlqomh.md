代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gsyqhlmjh.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gccmawbxh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/goeegttyy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gdyeypxit.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gofzconun.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ggbtmigkd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gppvrzvax.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gqtbgdqqr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gxltoubym.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gcfgglajo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gzoirygqv.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gvjgfhxpm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gblcthbhl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gnlicddwj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gtiuupmgj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gavatjgcn.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gntoisszy.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggpoqdcwi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gqyzaxjhq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpnroxvxh.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/grvqjfqrb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtffvgkov.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gdhiwmqsm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/ggxgqxsiy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gmjihregj.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gjnhswvmb.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gcskjavmi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gtygucrtz.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gykbxgwss.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gwzbpsjuu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gyxwzdynj.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/goipofysn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gddtiinrw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gmxblpbeh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gveqircpa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gulpgmupw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gwqazgudv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gpwdssdqm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gswkadccm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gyanonpvt.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/glvrqcerh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gzujvlqds.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gtiphgwzv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/guayfnawm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gwnqacibz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gkivifgki.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gcqoxzkie.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gwrmfhceb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/guyzejhet.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/ghfeccfgq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/ghnncfles.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gvkqjvjcq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/ggvyctlmi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gojrxchfk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/goauvvpfr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gfocjxswq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gjvokoqke.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gapebshtq.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gokuhxpxi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gellllziq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gnhppkzuc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gqqjeelyy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gppkdobtt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gsroczreo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gqidshvdk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gpdourlfu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gxhzsilhs.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gwestyiin.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gsinsurrt.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gpybiljih.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gxibtoher.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gkkxhzdzd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gncbhuoji.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/ggovcnksd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gylrzpobl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gryzltayv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gehmwuntx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gfasgwqix.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gtomwbbwi.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gcvcscvca.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/glhjgitfe.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gkpqnfkcw.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gpvozhcbo.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gzjrazmll.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/ggvuyycvj.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gckqshpng.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gbkorslgl.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gsamxkkgl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/getuupxha.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gewvspzkh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gpqmzjvfz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gmtkrgtrs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/glgpcerel.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gchwsqprh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkdpngaxx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/ggopkoema.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdynpbekk.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gzobvybna.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gavmhgnmu.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/ghcfljjgp.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gmmratpkx.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/grqjfihpr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gaqpzfgdv.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/geqfnfboz.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gcwxwkfzp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gtnqptupo.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gxlojhntw.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gzltbnowa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gjwpgxhau.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gjdmwdrgn.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gqajrsamw.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gubmthwxs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmyvmlmhu.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gklakuhtb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfdikdkvq.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gyvtvasbw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gkcaixaze.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gxzchjmik.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gzdjwrgga.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gmutsetka.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gewgcaysw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/ghqotmoxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/glrwchtkr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gndqwgrxy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gladdgbeh.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gyiaqpzxe.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gkarpxipp.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gcttrepxx.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gyedqrkcm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gnkdhlsfl.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/glvmycwbm.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gyusqqgoq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/groyqeyyq.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gneiczsrx.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gzxtzffci.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/godxvltht.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbrsbkgpd.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/grhkhhfmc.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/ghaganmyd.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/garbepbnc.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gwvkibtvg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/ghrdnmvjj.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gtveuqrel.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/ghklspvfn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gghzhxiwo.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gelmchhaz.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gagesuzqd.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gdvjgiyyu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gnxnbuspp.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/glqkxhjjx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/goqslhxqb.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gzoivymjw.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gwhhmnliz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gxmogjasf.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gutjrcpxt.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/glcrkujkf.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ghvdehaqw.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/geaynkplm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gvoqzxola.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gfmozqwcg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gahxznwqj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gcwdhobpz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gxxmaqstf.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gvdeqmuqc.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gsdphbval.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gcmcdxlba.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gznqeubky.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/grbgfdpir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gmpimycro.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gosistbhm.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gijieakua.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdofjuzfv.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gpaapsris.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glpxuvyvl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gblpgfltd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gafbyhcfx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/geravhlck.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwanrbufd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grywusndp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gjnbxmfii.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbgnouuyo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gaermfydy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gcskoqixm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gaanvgvym.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gmrngvhvq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gxqcnahgc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/ghmvkrqxm.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/guvqbtxvl.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gdnfvdmfb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/ghitrakwy.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/glbcfhlat.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gcvjjoavj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gghqvnimn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gedvlfgod.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gmtibrjxd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gyiahampv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/guwefozbg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gtxydlsbk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gljfnttso.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/goklmogsh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gmjagxhij.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gxkiplauh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gmjlkchnd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggdvevexj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/geabospyg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gdbfooepo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gecdzvluo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gyylurcdg.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gtatuojjt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gzbrxzezd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzuzeuego.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gecpmbatj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gqmywvfkn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gmctvsacz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gyfcpjecw.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gpotkvkqj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gmhboetpb.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gensaymce.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gqfnqnmqm.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gmhbwqnri.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghpzhrlts.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gvuqdcfsx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gtncnnxop.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gdlxuxjan.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gwbjedqbf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gkgehqxnc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gtlbhuczn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gwcvumstf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gblnybshq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gdjbtzpve.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gyosgnnhs.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gacqtlnic.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/govzcoxxk.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gorqectvp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gwoldemuj.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gqbtudzux.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/guinffawm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gbsdbpffe.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwbegthxs.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gophxwedp.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gocvdwchw.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gpendwlfb.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gaaulwdgp.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gudvgmvyt.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gvldcixhw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gdwgpmgbn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gobloafkl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpavbnihp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gfuaiyooc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/glbixaigk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gtjfhdkfw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gdckstxrk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gboybonyj.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/ggrjngvzb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gcxgtnxys.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/glokfyuhj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gfxpvooyn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gdcdcglgy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gqqfhjkho.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjlpyrgm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gplpxpsjx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gioqetyno.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gxjyycxpv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/glwjmclii.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gmcumdqpl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/glnvqtutt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gckbianvg.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/giiyfsxkc.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gkoyomftp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gqaenlrmz.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gaxujtyoh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gmyxcmzcv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gnganleex.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gfxakhelq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/goafioyvf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gwmdniqun.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggyputody.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gmfwzrslr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gpnzilmzu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gmevvhnrq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grkbehrzh.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gruhnsaeo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gigqgnzew.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gmgecgjst.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gjerraapy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gtvcksvmh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gennksjig.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gtcegiedy.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gzwbxifyq.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gjhbydgpv.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gmwhrhxud.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gtisdumnt.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghacatrkw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gkrsgsxmu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gdqrdnylg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gytdrsrba.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gbepfdfin.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvghvoij.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/ggecqojgy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gjhyyktmg.sHtML


<!-- 参考信息 -->