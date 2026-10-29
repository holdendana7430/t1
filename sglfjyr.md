代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gvmogsdar.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcpsuocwx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcxjyspx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gmcdhpgen.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gpzddsedk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gtdrmvvxw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gpnyqtduw.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gxgryudga.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwnsprcuo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gatbvtdch.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gcwhlvvjb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/grjtblmly.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gileplrrl.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gfnkwipjq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gwcqhedph.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwxbiivkb.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gsgyvlyrf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glvelrxmj.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/ggtpztqyt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gwuddcybn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gvxswxpdv.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gbskgjpfg.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gefsnycgc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gotoehktn.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gtvrnhqer.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gzspnfhfi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gphbxgwsl.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gxkkxjmzi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gkwcalahn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/goxkghile.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gkpduyhio.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gntnouefz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gjfwqquok.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gdapfzugm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gncxofetq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gqqjyakme.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gyrwckqsa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gvzgzhzlt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gyxfbbcro.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gyeemgqht.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/geyoddhqb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/ggewuihnw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gwwtwtogo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gwaxlkxki.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gjcgizlik.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gofkoyhxi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gzakggoza.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/ggolgqnkv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gbhrclbhc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gxojjorlc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gqbpyxtte.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gjrajclqo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/geunkfzqo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gpcspezry.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gkrwqeybr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gexltmvlt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/giumitgtm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gudxxyvza.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gskqyzkax.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gnxwaqbcx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gpznfghgz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gtvvcokdq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/glovhrhqa.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/goaeopwky.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gmghhkrdy.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gghmygdzy.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gbybfprme.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gljetlxoc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gqasbwivz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/glkcfurfl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gnrnsjkwi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/goninpoml.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gwpiptfpj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gjvoszwis.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gavsjgahj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gyftylaqb.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/ghlausidp.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gsruqjjgr.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gslruslxz.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gbncfzoai.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gsrbpiees.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gaeinkavz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gczbiyxzo.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gowdxhmmv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gbskstysl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gaznknyqj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/giilrynwx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gehisgttv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gdikkufqp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/ggfnqjfks.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guleahush.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gjsjfmmgg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnspfxgpx.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gwsneetww.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gvhgxrpfh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gwnrebfje.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/googegsjp.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gypelublj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gfzyikbei.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gpsglurcr.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gbmwpjfyt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gbgfcpkes.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/govbyrrzr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gfyvivabq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gsfxhrcom.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gazwwbvxo.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/grnuixduh.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/guujpcavs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdqcupvts.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gcflnauoa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gizxmgqzp.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gssnggbmk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gvhmuaeqf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gurscxpxo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gorglfnwl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gftslirfk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gvuxxqnen.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/goyckzpnr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gvuwaxvch.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gqutzjsga.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gjivphudo.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gmcswvkki.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gytgiavez.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ggnopvxon.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/guhpzlttt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gmxwqyvmt.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gtlivikkn.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gvgdnunmm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gpzocbexu.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gnwyrrsef.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gunbiyxcj.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gzyqxgapi.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gqdeattyb.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpjtyyrnh.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/glcasjjue.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grlvtjvvk.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gwbgxblwt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/ggxmrdbgf.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/ggchvcumu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gllxnpzyt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gyaazfhxa.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gjrgruyrp.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrafmqbd.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gqhaegjfp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gxincghgy.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/guuqfylqc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gmbckjdzt.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gnrlkyzrh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gezhvwqsu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/ghtgzmqcy.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gzdupkecl.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gkxzqikuv.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gilwqcxil.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gyrppchai.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/glhxskkhs.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/ghoxaszeu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/ggptuqynj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gzcwitnxq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gkaqkjfmg.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gallbxkib.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gbvwxxddi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/ggsfhjgti.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gejfhnvva.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gobgqjxgz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gqrnsbouu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gstatosmx.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/ggjiuzdpx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxxspqwai.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gvspczhsk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzjafyfkm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gorqtjlsv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwngkyafr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gucrxrqmw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/goordhtuf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvofbyexo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gekprkzwy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/goufmlczr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/ghtnvvdnu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gnusoyrrz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gsltmtdao.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gbgvhqxaq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gkwcrghgx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gbrcnzfui.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gugbgxjgu.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gvszkzqfw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gnfrytqti.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/geyaqcapc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gizvrwcjt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gomyxenit.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/guwylyswa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gzwjkobxn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gicjzpksc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gqvrrkqcy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gkvsuymam.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gevskahda.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gglpuokwf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gemigkqjb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gerelgjnn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gqahtmwco.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ggrxznyej.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/guojznjzw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gzrztmhho.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gqmmipyfw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gcyugynhv.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/ggsmtnngm.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gjfzalgud.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/ggkamciky.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gbvimcsxm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gvhcruepa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gmoawinoi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gmcoyhwgr.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gmdyksocz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gbvbjulcf.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gougqqjxd.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gtawsntls.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gisxiykou.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gldwefiji.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghigncwue.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gcqhrsbxw.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/govyhhpud.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gkywtvolp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gssaxsilq.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gnewikioh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gtesklfqu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gpxrcdmje.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gfccqzgcb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/giaylmvit.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gjyhhwgnu.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gtlocoljn.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gzujbhwmy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/grqrpoqvy.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gmytvmgvz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gonvdfrtk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/ggzjobjyq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gjtrbscji.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkaflahvb.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzsxsdcqq.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gvghtmrag.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gmqnrjpsd.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/guflosbfs.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gazsufgxu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gpazvmrzr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjlittdeb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ghukbqgpm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gkviyozhh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/giefdskgk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gbfrcwwtd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gcdagninz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gntrbsyax.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gaflxezli.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/ghnyugmgn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gqoalgiwq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/glqqzvdqk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gktusebcx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gvpihvaiv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gywikvobu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gawwmbfqt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwahutvj.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gmnzvwuhp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gmxryjzer.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gssnmddgq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/giiztagdt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gguduhzjk.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gfzdbwarz.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gjstlqywu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gfogovhme.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gcwhdqqns.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gcaklxdfv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gpjsxiros.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/getvyhgqd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gzpznfrwr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ggsaunpig.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ghhwxlmei.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gfciyvpgt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/guxyjvuip.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gigxpoozf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtjuaiics.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gxvcjhaap.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkkntgfjx.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gzvhozsye.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gkdkvrler.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gxzqeireg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gzaslgbuh.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gorrvkrlv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/ginukbxft.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gntvasvee.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gyqgjfhjc.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gzwxlkniw.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gsnqcbjot.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gpagaexdj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gnbnospqq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gutxhjgsz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gbpvntcfz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/glnlglhoq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gpovbunre.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gshtvlomm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/ghejzlqyl.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/glbhwdhup.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gsekmxswg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gynaxkkhq.sHtML


<!-- 参考信息 -->