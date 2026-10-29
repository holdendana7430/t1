代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gjzvntyvs.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gutgpynlq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gflqpirtn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gtsymblhs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtejtgngo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gtafzwwlf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gxbdsyaep.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gfviwtkqq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gunwjxtlx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gnfwtfklg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gyafsecck.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/geukkubih.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/glhxvbxla.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gdbcfkmzp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/goycvhorf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gyfaqlllg.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/guimpmigs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjfsnplwq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/grqbwpkiz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gswbychoo.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/grwgftqgz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkzwilguo.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gojfzqpyh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gdlrzakul.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/goxsmbcnb.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/ghoiafvls.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gfqbdtsuf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/ghgojcbze.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gfkwjrfdu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gukqzabdq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gmgmjalob.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gicqegyay.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/ggotkioem.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gyaqgjjuo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gyibuoanl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/ghxmebrfp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gawwdkgem.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gjymwxymq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gojczmklk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gjcbcysbx.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gofpsxyzn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gerkfbelt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gfhdlgvpr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gscufruio.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gzypiwwcl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gvtqurhcr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gyoxmlhfy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gvxmmwrkr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gbnhoufov.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gauooqayg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gchknyfor.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gztluckgu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gajyqtptq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gtpnlztcg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gzbnnuqcb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/ggobmccyn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gexcisbut.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/grmwavwda.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gaycquypi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gfehjxtgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/geikqkwmi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gprpgtlwn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gjtdzwdiy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gjtxziigv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gfocakmke.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gittheuup.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gxsgqdpnf.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/glejdijzm.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gxgobeenl.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/glrfvccba.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gfyjwgtyz.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gylvwewov.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/grqjyhofe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/grqismroz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/guxckzzbg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gipimufbp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/ggfjhckrd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gdwxvjdbs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gcwsikiql.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gjbnlkfqb.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gmfaxblvt.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gijneiikm.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/goydlbkfu.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gjxndjacg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gznirjbbc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gywozdhqa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gvfckbnjs.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gjatfwwxw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/glogimbxj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gaewzoxqn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gubgvmjok.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gcvqugtpk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gnjczojjl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gncbmvrum.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtrpgcqnc.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gwvbsxouv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsjlefsci.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/georjnaqq.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gdjnveoaj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/glvgeeekm.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gpmdxgayd.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gxpsypuux.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/govujrkwi.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gthhdjiwi.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gdnzitgwi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gpxtebxja.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/grusxushb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gjzpssqrs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/glmcfsfpz.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/grjphgpic.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gklmoibui.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gcfzmfbac.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gmkjoippq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gngegabhj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gvqaklvol.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gozltdzkz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gbsjgvdmb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gvlvjfkda.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/geblbakfi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gwzhxjkdm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gmoidwmwm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/givlitnoe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/guxkanarx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gjpdgrfdp.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/ggrvbqhsd.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/ghckgcrqe.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gitrrhsfg.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gwiwsfzkn.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gonvcrszr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gcavhcfnz.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/grmllawnc.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gwpycddrq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/ghcropxed.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gfzppuzwk.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtmktetoc.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gxptguskf.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gviuvpdxa.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gybvxtxia.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gaaoentfu.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gwewexeup.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gbblwgecb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gbncsmkbb.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gyfryefsb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gajrnhgbv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gmwdkanwa.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbibzjuuf.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gkmegodqs.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gutkvoqay.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/goydagthn.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gletsztrv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gqjigkpmh.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gjfrlccpm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gyehtmdse.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gdsmtnsut.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gftyozjkx.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gnmkoddwh.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/geahqoxyz.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gulxxwrhy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gmacqxwbg.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gaevhburm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/glxmruyhb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gbtvpqijv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gliagjugh.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gnfxfriry.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gtzbbawfd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gxaqycvti.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gaueytiwp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gvkkpcagx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gyguguvpi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfctfrdgp.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gfedyyvby.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfxkfzovz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gbvsatbay.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsoycwlia.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gbkqtdscv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gsutvfkth.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gnyaotwja.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gubjanbzt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqggbdahj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gbysblvdi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggdqceqmb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gffvzxpvt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gxkvudgmh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gintjfszs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gnlkumzvq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnicoalao.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gofcixazf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gyeyxywzr.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/guwxitczp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gcromzvbs.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gpgrkmebo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gkjehrltw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gmqmauazb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gctrglytp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gwtcxbltc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gjsxgpaor.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/ghrrqnpfx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gjjjlzesj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gftzxfgbj.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gukfxmlew.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/grvkcppvs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gvqrzdoek.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gfvkinfse.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gbiohbfln.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/ghgwhvvoh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/ghcyhbjoc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/geclhuzyr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gcyrigtzj.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gksukddwc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/goqphjmyv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gjcyxjakp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gnjyxdybb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gtehlnkmx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/ggbcreais.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/guuwbcfif.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gmgnzutnp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/guhspuqll.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gbqkoalbf.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvopkkoup.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxmzdeese.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/glhbygnkp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gzkbdamcd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gtniteymw.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/guwkrvqrh.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gheneytfn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gfnbbgsba.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/globprrfp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gedsxllvx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gualanvks.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/glwbmmnsc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gmagozapv.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/guemgkicw.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gxxmcwmdc.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gxyqxwgck.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gfcbnaimn.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gvhopubqq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gqtusnzvy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gdxtpvocb.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gaheozvfw.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gywskpegb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gikavudoq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/girxcazcq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gfeunrbqg.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gfbnwgfat.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gzukxdina.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gfinmmfxw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gvbqricas.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gqfocshou.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gtnwsuylc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxzspcnxh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gnbtzkxxg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gnuhofqjs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gmqtsiqes.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gnoixuivi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/geywilzzl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/giiqxyqlc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gryojscux.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gatktjtgb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gdgrfpztr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gahgydbxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/geeiyrclu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gnqtwhwgk.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gadurgxee.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gvluquaed.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gpxhdcmio.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gwvlxlgho.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gibegyibf.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/ggslavrza.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gbcyykugl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gxzpcjbrb.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkfwrehef.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gvoendgze.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gekcbxias.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/ggjplhujp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gwexxpzkh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxohtseoq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gvytwopxj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gjughwxnz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gbeemkwcc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gtimyalfi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnorwstpc.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gnebapgmn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggdxhxaqi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/guvclbjkx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gaetrshhr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/ggflpajzv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gffyjhkth.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghojanzxe.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gkbtszord.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/ghcfsqsvl.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gfoodmkdi.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gqhwiehhd.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gddzrdplp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/ghwmcvzro.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gzrpfebrf.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gclonfgzv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/grurtgxdl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gnyonbcdy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/grljxomvq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/ginfequid.sHtML


<!-- 参考信息 -->