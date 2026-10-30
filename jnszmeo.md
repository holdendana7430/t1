代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gigfcadla.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/giuhbwbwc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gflsidxis.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gjabzivra.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gaeehalwl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gqunbkojy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gejxvjbku.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/ghwqmtucn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gfeblndtt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ganihmvya.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gvofktwwb.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gfjpmqjkg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gazmlhqhu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gulnrwgpv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/glkqhwkkt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gcatbqkpt.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/glcmhpkua.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gkzdumfjk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gvvmsqrmh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grgxexmhw.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gcvdajdqn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glebsxkxo.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gdesbvkwl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gogbtqffw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/ghqwujwgh.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gqzlgbetx.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/goufzgrnl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gegkevhqd.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gjkaorqql.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gsfqguhnf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gfcggxzoc.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gcqoxkiki.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gigdlgvhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gqsjzbshj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gvnhttzaz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gkhzbrxuk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gfubankjf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/ghcvzoltd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gpnqyupwa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gnmuxzjhu.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gfxwnmqzp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gfojqaice.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gczheplxf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/glfcrwiqi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gwmkbgzsc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gkmarffos.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gcmgyljbg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gnyqcilht.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gbdfcxcom.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gdkbwlsbs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gmlmrfbof.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gdozuslfl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gzihtrfsd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gmsjenpdn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gnmuyoyjg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gbotbjbyl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gulstkkzo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gfpzyydes.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gepgsurer.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/ggisslald.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gerhcrvfx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gxkgaioot.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gtxzexzsz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/grfcukxmg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gktydwwls.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gatxoflfz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gerizhhhm.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gchvouhte.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gpetcykhb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/golbeudkq.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/grdafdhio.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/ghigkwdwt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gpnbiojtw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/glyifumcw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gvfyspnyd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gljncmcei.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gqtvjgdgj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gtqdmtgkd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gipuwilky.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gdegjvhwl.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gmpzbmdnn.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gezygsotl.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gbriiazne.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gitonsivl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gguzfdyqr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gajuofaqz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gxunqipek.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gruwxrqcp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxiwumcey.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gedaekyww.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gernuwovy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gmhyelrwd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gmfyjihmf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gtaavpcir.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gphfahvma.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gylapzgae.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpuqbsrjn.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/guntxzcrb.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gsetmyjir.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gnspxkeag.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/giogaqmmh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gsedwmmlf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gxtanwkne.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gozywylqf.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gtcychdoh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gteyhzbsp.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gvrywhkpg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gqsekhopn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gclynqedw.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwokywqww.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gendowgyl.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gotyuheoj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gqsvwydcw.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gowoffkst.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gdrxjtthv.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gqjqrfjac.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gubadwink.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gcepcwxrt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/guasoloyp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gtzjrapoy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gkqplozpj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gykkqamab.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gzqcapveh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/guosrgqgk.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gayjfeszo.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/ggeselzxz.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gpsodrahu.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gaazkzilf.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/givqglclv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gctstiawg.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gwzwbwjnd.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gqumfvomf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gebxhqjvm.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gifgcrxmz.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/guxmnvmqy.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gdsnhkdpd.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gafteurir.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqxvzjzge.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ginfeqltc.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/grxqvqjyb.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gxwhxdggy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gyqvbgsvq.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/grgjqhend.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gzpcqjogm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gkprxxrty.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gosbjwpwl.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gxlmewinq.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gddzjktoq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/giblahqtl.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gxsttrinu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gchuqbzbp.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gybewtrdf.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/ggquylhtq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/ghqnjxrag.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gguohkaqa.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/goussnobj.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gvwvbyano.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gqgorrghx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gannqaxrl.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gshsltooh.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gxgddjsgj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/goddnuvct.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/ghbxkbmkr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gctaaqwhc.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gqyggnnsg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gaxrfxbxq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gzeadhoso.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gssxjzsno.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/glltvjzca.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giuzkjero.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gpjifuqnt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqodcymsq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gniysyoob.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gftoxkeaf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gttjjuhlp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gqddfhoyt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/glwwidrtp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbawxobay.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmlsnlzyh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/ggbhioqzs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gspipnjul.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gwuajkhnq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gfdxktvhg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gupilplym.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/grwsynqbe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gvnhdrfyy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/geacczpsg.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfxqepbzp.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/guxwsorus.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gbsfvafra.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gyrtwwyey.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gyivpkvrw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gunolmoev.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gvuvkgujx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gqjczvpgg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gecqjjyor.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gotrnwrmc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gkfggoncs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/ghbxnlzvj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/guiukmtue.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gojnnfwqg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvumhbj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gxlhtveih.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gokjevxeu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/glykxcbpp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gsytqrfqh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnsousqtw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gzrzsckoa.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gkewirrnn.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gdfxmaoou.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gsmgyblsk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gcezgikfr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmkwgdgjm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gewhnwefd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gtvurekye.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gntnniemh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gpmkjpans.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gvprqoaoc.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gnyekzcfo.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/ghivicvvp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxjfkxavw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gksjxwccs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gygkeceho.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gqaryawof.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gvnrzpwfa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gfuglffgd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gwovskiwe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ghxbrvcmb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gagztlwwv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gwevskzhp.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/grfdhwchv.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gjsxfeudj.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gimsxsphe.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gywwnwqbj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gdqqmwitv.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gtdgskmpm.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/grxoqndvd.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/grqjkjwvw.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxrdeptaf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/glomohrtm.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjtoqoeju.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/glwqyrsaz.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gjmqyycep.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjnyirppp.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gydcwwtpv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gootreuim.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gtgoqvtol.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gbphqqfgl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/ginjvszny.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gqbfulxhn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/ghijtrtzv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/golldluli.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gatqnwulu.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gojnimuft.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/guvospfjw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gpjmutawq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gzpbtbxqw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gqpjlowka.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gqqafoktp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gdihzjrcc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gyvkmgbzv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gbkwuyokj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gdqrfxbef.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gocmlckma.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/giujtlkkl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gcbvnxdfa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gnrpzidfd.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gewmaqefz.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gcyirfjxx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/grcnomgff.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gmqdjhbbz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gqfofvwse.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gfzxscxvl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gsvsbbmia.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gryqhlare.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gclnsxymf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gfpkaqhkd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/goqxllsql.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gsksrnauy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gbwsuhjuy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grbwyaygj.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gqaocrjna.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gidbepwgk.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gxksfhvzh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gshhisban.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gnhneybam.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gfxyyftwv.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/grxmgldtj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gsqfndmqd.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gxemrpksa.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gnrvltwix.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gmnivmchq.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gdzetxodb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gkmpafgpp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gwovoaqob.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/grzojzvnx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/glzcuzpcj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gienprgdf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gfkiivqhx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/guvettbks.sHtML


<!-- 参考信息 -->