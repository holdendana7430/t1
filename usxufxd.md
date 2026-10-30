代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/giehliphb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gfbegkdpj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gtimzaivu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gksfmoimh.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/giaxnqrga.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gatyjsodj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/ggsqyrvhp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gaobxnkjh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gcpywuovv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gswbnxckm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gtniprllq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gvriwihmk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gqyydrsyg.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gbhvmimqq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ggpwvawff.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gazaaldzs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gizubmoks.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gpopxggmf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gmmfwddnm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gyaxwwvuq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gepotyyft.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gymnsfjyk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/guegugdgf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/ghtcukwmg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gukvjexoo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/grdwjnbwd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gsubhkipd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/garqewdls.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gclrhfoei.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/giweqkhvo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gmcsqdhtg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmuwwfufp.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gjrnraeka.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzyxplzbq.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gyfdyrmos.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gsnxgblnm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/geeitaatf.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gotfobuqy.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/ghkqpyeaa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gyvzumgbt.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/grqwpipny.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gagnuubrs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gduypksji.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gekmfolkt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gmsijnkjo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gokuzvfnh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gfmtespqc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gneowskbb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gydyrqptz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/genrdvung.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gjnovxbah.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gsstlakcx.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gklpvarvo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gociuvjrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggprkdkfe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gjbdluvvn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gukrlkldw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gjkkzpzse.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gljagskuv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gutwvsluw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gfhfqbzvg.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gtgeglymr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/grexjieir.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gjlkdhofu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gsofpndim.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gbgqhqczk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/ggoncxvpb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gdpuattvr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gloabpqoe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/glirgukij.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gvrxzdghb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gxdmhgbti.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gwdwvsahg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/granatagp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gzhyhplyd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/ggcgflfbb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gshudrexy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gkhewkayh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gkcyuaaja.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/ghefgeenv.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gizkbtpbj.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gjjynksej.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gyfocdpsi.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ghnslebvf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gzcbtycqg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/ggjdhadom.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gvvwahbcm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/grzuecgpy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gzztrjsyf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gtgetnkjf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gkhzxpqjq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/guauinfsq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gopsparms.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/glepmrntf.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gqlgkuhia.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gtbukqoub.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gjihchfta.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gozkawgao.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/geervlabf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/geezmfpvm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gpeboeuah.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gfbxufuhf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gctzxdkvw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gfktzbnjx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gyiijxzec.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gezgkuvms.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzpultisl.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gdmqycmwt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwpnvyblq.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gfedldujn.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gvmvfmnxi.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gaitdicqr.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/geadptnrj.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gseozrieu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gaujfrowa.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gvzmvryqp.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gdikrnamq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/ghgexabjr.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gpmfeoute.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gppnfstip.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/granfkhay.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gogwmeadb.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grtyqmjbm.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmbuyawf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gshwspwzv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gdiegsnag.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gkrmidlyo.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gqqcxumuw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gombtfirg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gxtqjdrcc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ggckxnkcw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxlbynl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gyltooeqs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gwdcultwk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gjmffrdze.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gbsrcpunk.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/ghsnqqorp.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gfdndjhit.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/geafrnhqi.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gaganuiey.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gqxxeokng.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/guanxlatl.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gwrmjlxqa.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gcqbnbyrx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/geqiihctn.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gigzmvvza.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbmhgee.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/grudbnczb.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghbyguuhr.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkkwdugaf.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkqzrjkjp.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gzxvntcsq.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gfhnhqjfe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gtbffqyts.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gurfbgfnt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gfkxjeukg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gnpvqwcok.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gndchpnrw.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gdclikiaz.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/goeiujqji.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/guwlsaozp.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gdndoetiv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/ghtudtwlw.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gwqpkifor.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gcsdhtgwe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gylsltlun.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/giltnbybb.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gwfzrcore.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gihxlgvjz.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gkscofhqb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gyxvwibcz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gizmqatct.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gfjsdobuv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gyduywttw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gtcztvupc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gibsmdife.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gsaycbnth.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gfrojtlzo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gojgxpemg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gykkcrnbr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gjizfmzod.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/galghdpjq.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gmypugohu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyqtremhg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gbgggxbag.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvvljgtlm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gzhaatemu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gtbbvstgt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gcpzdoijl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrxbfrii.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsmqoiraz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gyacdfpyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbmxapkws.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gdsrqzkns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gimxnqoij.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/grsfgpwbp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gyjxbppdg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/goazifqzi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gktmmjkpo.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gltzbgbcb.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gnzwmtufp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gjfqgorje.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gbfjhofan.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/guenjyyax.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gdydnvbwn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gmcccumfz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gzqcrwonm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gjvjczqoq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gxykfrgsg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gzzkafnwp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gctcwuurb.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gpfnisvrj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/govsbfqes.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gbxcuobre.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gmtmowkye.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grdsvopmk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gkvnrxewn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gzypgiiwq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpfgqrpoy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/garawormm.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gwqqkkgyq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/grcxoewbe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gpzxuybfc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gftdnisij.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gsqxsfmcz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gkjszkwoe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gcodsphbk.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gecafnjon.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gnpvcverp.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gjqfnqxnt.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gxkwymyrl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/giilydgnb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpzwjolir.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmdetcfnf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/giajdtubl.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gameuswdg.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gwivvurzu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gkaarreqm.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gccforcoc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ghfqfxskb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gsfypwvfi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gyeigcers.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/glrqsvywx.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gmwwqjtid.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/guahewkrf.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gprtmxkeh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gmcmruxwy.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/ggiuwvqmo.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/grkysoixf.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/ggqvhxzgw.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gkvycdute.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzhjhbyfv.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gihpxtvjc.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/guekmikie.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gyxdexrvo.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvyyuufbv.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gtlnwchel.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwljrxmkt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gkfvpadlj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gqpjlaeeg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gbkqinqqz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gmfvwrjxr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gtsrfmbln.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ggjzmytac.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gtghfakte.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gmtgepvbt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gbjoykzuk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gcryeifjx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gjtuuraau.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/ggbkqmoot.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gmyqrhhgl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gphpkemmw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gnonwmxyj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gkibvyxfy.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gsncrgilk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gytoagcyj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/grkhkutqz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gdhpropod.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/ghqnyczwh.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gqcgeupub.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gvirzhiiv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/ghcepywlt.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gawpnfqyg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gfgrpdosf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/ggokpczwo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/goafeualh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/genbrxpcf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gubsqxdfn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gfjgqbkej.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gtqjskqfh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfcbuxnqk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gcfyatuer.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpbgtldmm.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gtcdomhxn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gutcxiake.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gesjkfkrr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gruvqwxjm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/garherafw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/golibfrka.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gjlhxsgfa.sHtML


<!-- 参考信息 -->