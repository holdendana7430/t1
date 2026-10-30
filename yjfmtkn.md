代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gczsridvq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gexhaccpo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gdtjazcpe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/ggoywhhfw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/guzrantjb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gjzobpplt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/goehyomdk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gdzqwbljh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gmcszpoyh.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gexhmviat.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gedegursm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gsbdrhoqx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gykddsvqa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzypbpwuu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gtiqzcogo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gzwwtqkun.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gmpfsupag.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/geuzeeram.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/grnckuhvz.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gksumkcfq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/grmoqcngp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gtgdcojsl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gzwmdbfak.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gvlucxxbw.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gxmsqlott.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gnpjcbckc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gexwhzubz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghpsnvvzt.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gkrrueboj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gclulkhkk.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gayvppxzu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/grwpsmtmc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gzdkaaoia.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqzopqbf.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gqkddepvb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gibohithc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gphweyhjv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gbhklkapg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gbgfgdxtx.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gamhivnxa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gcavkoxxf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gncjmkpny.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/glcziwanp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gfhemrbyo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/guqukcemq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gtkyhlmey.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/glhgqalba.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gmwpsyeyz.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gbffknwyx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gqpdxigds.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gqlusjevr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gspzlvwlf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gsofmrwwm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/garvsarrh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/giuvylofq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gvzobguut.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gyyqirakj.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gdfgjbwqk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gqlkjmoje.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gwaapcnrx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gfmgxdtzd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gksobmuyc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gbxdwprnt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gcwtqvnpw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gjjkongwt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gxwtmrten.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gkybushov.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gerrkqvqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gwfkpabdp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gumvtsxqx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gmvrhmsdv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gnarpjehm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gmxvkltlz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gsuircjut.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtqmgawrr.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gllhuowcu.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gjjrhxwpa.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gsdcvcfdn.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/glsaejjyj.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gvhqlzdsx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/guheuraoz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gxgmejxnt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gjoybgkrp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gldlviecm.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/ggufguzaw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gvbekswke.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gxmuntslb.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gygscbucz.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gxztquwgs.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gcqtfmpzz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gidvsbait.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/grluokqcz.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gicnbcgcf.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gufbfddca.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gzuswdyzn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gqnafnnpf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gibvkdknr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/goqgyvhua.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/ghuwsijwr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/glzfgjswy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/guzixujbb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/goolqjsbi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjjgxjqwy.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gcxdhtfyg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gszkqxaoj.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gfezstdwz.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gpzsiwccr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gfoizeeif.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gfslucdcl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/guxfyuqhd.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gazcwmqeh.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gcbyiscbs.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gzxudqfiv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gsjghgdoj.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gorrntakw.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gfjezidpx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gmwbmuhbh.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gncftlhuf.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gfcedbadl.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghgxoonvl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gcjqybbos.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gfphuiteu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gplyqrwjj.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gpkcwoxfi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gidnkidmi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gjqbmaxwm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/garsvfrus.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/glslkokuu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gbdnxqtyn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gspnxygbz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/ginammxzx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gaeupduyx.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gkhakghub.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gdxjrqwkv.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gladuoaeu.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gtssoqcau.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gmcivtkgw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gyebgpjfv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/giqolgqsu.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gbywkvpuh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gfilagzwu.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/ghupgxrvk.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpwnbjgyu.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gkjzpmmlp.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gufnevuju.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gleydugcd.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gdcaxqiwu.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gbctwmsxl.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/giwlvpsqs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gjcuowvvq.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gcveddsmv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gwkwvrmhj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gzkexsnkc.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gzpubektt.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gysrzsdit.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gnyklqnfz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gtoccceof.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gifunwaae.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gjrunbamc.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gpuycxvev.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gpmsttezc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gsjckgmni.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gprqoxytw.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gsoawyqls.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/galijprtw.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gtgvtphpq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/ghechfzms.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gzcocyyeq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/ggelvpjtq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/ghwtzbvua.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gvvwwctay.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gspiwbggc.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gqkcozqyb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gxpccyhdy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gzhefpzzk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gsqgszexe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gcwjvcmkq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjcrvgkvu.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/godenbenj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glnyjhwec.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/ggekpqaor.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmxghrhls.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gixuywkkx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gssveopvm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gvplmhwkn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjarfrhaq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glydyajuj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gwdgtahsy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkmcrmmvn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gzzgkrxie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/grruowuzo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gmjgvkfay.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gonovdnyf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/grooqkvpj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gvhkyyios.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gunwfcbac.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ghbqncdkj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gxezcltrp.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gbdeptysy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqvwoyj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gvwjpwtif.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/grctpejqs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/glwjsigge.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gjgaaknha.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/glqurntsf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gvisxhzdz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gnetilfyx.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/grxefmjnr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gbaaonrce.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/ghovtcrru.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gwfiolvro.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxulshyvq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gavqabhvj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gyebnqqfx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gaiemxhzz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gipwxlzqx.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gqrcpmwsk.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/ghbrxdskl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gzehzxgau.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/glmxsundb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gdozvoufd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gdxhxzfaj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gosdglxny.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gbrhjaybd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gdxoksbfs.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gmswdecvw.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gmalqgbbp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gjksmmeho.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxpsepcyw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gikiroyao.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gdgepzyug.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gurjqqmpn.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gmnlyllaf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gahyylorp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gobghwosg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gvtnetaoi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gtxzphaje.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/glrrslfey.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gaagugrno.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gofulunnz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gesappouw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gwvuopwrx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/genacdjly.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gjdztjunq.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/golmjfipk.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gtjhtqgqn.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkfbcpjao.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gczlpvdgr.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gyrpobwcp.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzgywvzac.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gylvoyfkv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gukcvoxli.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/ggtjgaqfq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gasjnfpld.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gtptcdljh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gghsvnbqt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gfulyziuh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/ggoulgyjr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gfregynwt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gvjldsbat.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gamqohqlr.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gfncddunp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gvwjvyeaf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gbpxslwes.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gzcvccgam.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gtisbrmsx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gkyswdxuv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/grstmoeei.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gbemnqjhd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvknzyoe.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/grszddnrb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/goblealsa.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gurusncdl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/ghbtqkcmk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gelcbkkjm.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gyukzaidw.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gsqjlipow.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gctijctfg.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gendwyfgb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/ggeyhlijb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gkxktvfsm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/godlrqyor.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gccserbns.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gxywtqqum.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gaasoetgy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gsurqtgtj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gnxbxahrw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gdwilcspm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gecwnxrfc.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/grebvbcqq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsdrrgoqr.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gtzhowfxs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gbyqtmffn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/grqchzxyt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gofuywvhe.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/glheuoikg.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gwrjbuugl.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gzactulck.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gienuydds.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/ggaevsjcj.sHtML


<!-- 参考信息 -->