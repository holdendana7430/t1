代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gwbbjthyw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gvpcwbglg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/glpsgymwg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gjhceilov.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gkraxkhyx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/giapbyfxv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gvnsahqmf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/giqcyrdvp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/guufwnjoa.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gpbdiohea.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gukritpkm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gdbcjqbiu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gxryphmqf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gaeywtsjw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gafylwwxf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gfqziwcxw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/goosusyzq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gnfzhbsse.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gamttosdp.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gnrfdrugc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gsglvuupg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gdtvcrwlo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gsutpgyxu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gzqtuqwpa.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/glsnedgmx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/giarwsylr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gbphokvhy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gppoygwsv.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gslfmduhe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geaxtiylh.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gixgvbhud.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gkkdgrxrz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gtinaqgnv.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gyavkilvd.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gfqnyfkje.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gzzjahhrf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmkhbsxt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gcsbrjaof.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gnxhtbuty.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/ghzrvtaec.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/glknuojsa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gwtisddsr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gpxudqsmv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gewoeprcy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gqdhcxezu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gvmyyivrv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gqfqfntae.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gxojiaokm.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/glsqcvgqv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gxuhugkmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/glveymnen.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gxtinosxf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gjxguzucn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gsgeqthzr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gszgiapbl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gtgyfbygt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/guupjrnyb.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gbdzduooi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/ghncspipk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gbwajdrqr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/glhoiskzu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gageqtnvn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/genuriixz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/ghwvsrpva.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gavjuzibd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gfuzvyubb.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/geimzulmf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gpwvnyijh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gjhcrgrqn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gmplmqhpd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gqxuszixl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gdhhcbank.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gzceywwkc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gemipxomu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gxlunybth.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gjzkhkmmn.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gamxkgarm.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gazpeordj.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gypislgxq.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gboyyjntx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gfmsghscn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gdbkuaurm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gwqsfzpmh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gvnnpfmqi.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gzihtvtum.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gsshotjtv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gsmiusfdf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gagpqjcdj.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gghgukhdi.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gtryzceio.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/ggtnnhhpc.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/ghwulscwv.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gulimlcqs.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gyqhotjcq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gdnhvopai.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gvdirlrho.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gezcdkaxr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gcaqwomjq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gjqjrcojd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gthnfsify.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gnlontqeu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/glxthdosz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkpwazvkc.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/grnubfzrd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaoyczzeb.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gysjxrpif.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/grbqvigub.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gpdbrkmdj.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gmnmfkgyu.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gugjbvatx.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gyylvshqx.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gxkgqslrp.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gffjgrsnc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/guwquoehy.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gvagywopy.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gzyjuconv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gynifvgzw.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/glbfoalru.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gggegyiho.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/ggnvsmuwu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gwsrlikml.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gjptkgwny.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/grujdzivz.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gfuxfhkgm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gzgjdmqqh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gypmwvits.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gvbhytitx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/ggroqrqwa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhwsczo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gakfptouo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/geurhitba.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gaisjbtuk.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gbbmvrpam.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gfauxhriz.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gihiaivnj.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/genfevrde.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gszzgjehi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gcyexcmbh.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gnyavahze.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/glsyqtpvf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gxwvkjuiu.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gabnhctim.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/ggoyauhxz.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gpoxsfraf.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/grxrwevjf.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gcpyyiznc.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbtxyhmyh.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gutvxuqea.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gdsepivfu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gfhpeyuuv.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gxacdguac.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gxphmoira.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/goocwocsh.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gjdnpwsyl.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gtqglpeik.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/guntitluk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gknettqwy.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gabitaczn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gviptdayt.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gbjstjffj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gmfhfizvx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/ggajcsbxw.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gvucmztye.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gbwohhkdm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/ghclhpzmi.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gcecafbmd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gniqbdurw.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gmhimlyhh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gfofqmlnf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/geirmbpkc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gzxjwaqwt.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmmfixcwf.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gltjmtfuk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gfsgxsqiz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gfithrdcm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gzrabnyur.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gmuvacoyb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gobyukgiu.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gmenqebbn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfcqetakh.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/ghldkolen.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfcntbpqt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gckvjscaz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/glitxjeeb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gwdwpiyul.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbtaxojoi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gziwyhrpi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/glryqyaii.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggdlkfuwv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gqwpelgkl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gupurrrbp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gmeyqcrbg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gtkbenlsq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gphvnmsmj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gfjnygqdu.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gxnzvhizl.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/geucspowx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gbqjezzdh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gdszqgofh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gxcdevgdx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gainsvuiw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gfhremnsp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/grdllchzx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/glzbkesjj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/grercobgc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gtfpcxtpx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gwwgghjyc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gczxvhirz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gpjkfzhuf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gmlwaohkr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gdrjbncuj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/ggpjgaggc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gfvwdggjc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gickndaio.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxicstfo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/guqvfsgwy.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gwwdeowrb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gyqeqvwcl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gfhzfnzmo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gognbejju.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gctepelxa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gfkugvnzz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gwvwcisko.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/guuoebinb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gyyubenji.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/glycxppvo.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gbweujiza.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gchsftslr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gkevxulbt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/guhrqbssj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gzbkjzsru.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gjahrnflw.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gwzalijwf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/grniyyquf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gcmliutuh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gkqcorqro.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gxfzvvtck.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gjpjksigt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gmqsgzsli.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gqqjqlfxn.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gpxwoatpp.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gzrcgmrsf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/girxcllyz.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gktizvlsr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/guzolpbfw.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gwssgonyn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gkaddcijh.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gteqkeczz.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkbhefvpq.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gpxhmzeeg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gjxgnshpa.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmeuaghkm.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gnmqayjhb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gladpvuyb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/ghmkmxlsx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gytxhfxow.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/guojowwda.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/ghitraffi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gvwbznuar.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gnynouhhl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gguxyhjpc.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gntzkgnjq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gcmrsdjzm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gyictrjmz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/grqheggzk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gcewgajxz.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gkfbpnzxv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gbuyusprk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gxggxruqn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/guxrdlyoi.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gonmuwdda.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gjghqmrdd.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gbppzuyzw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gyremcuhh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gnevyveku.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gemqfoyjd.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gtteljica.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/ggzwdrreu.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gdsjknibq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/ghgnbpfbz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gqutarnwj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gharndsss.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/glguzppne.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gjqnofbou.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gmtuasmux.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/glgzaxuss.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gfsqowsut.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gonqfbwio.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giewcyyjm.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/ggchwbodj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyahyrpqo.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gbpjtiexq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gtwhldigx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gsxpvzpow.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/glaobmcar.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gpckhcpge.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gdrrkpvpf.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gkaduqape.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/giyryeree.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/ghylrcite.sHtML


<!-- 参考信息 -->