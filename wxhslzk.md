代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gegyfsvgx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gmehniink.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuijitox.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gsavpxogz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyffltvpu.sHtML

[K07] 进制转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqiwanhr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gcanxvgwt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyiciwhe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkodgqrs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqufrykxt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/grmjkcyxl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjgaybom.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqmrbluu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gexlvtbcv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fanxiaobao.xyz/Article/details/gfwozgpxu.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gnmzrewpd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gvsqspwuf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gpyvcenrm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjcnscpw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppkocsrg.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/guogetuar.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbydpmffx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gwbxgovwa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/geyznxzvs.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhiapfrl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gilxonarn.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fanxiaobao.xyz/Article/details/glizdmvly.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fanxiaobao.xyz/Article/details/gxhuehkjn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqvblauj.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gtccdcevs.sHtML

TS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gnluuyeft.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fanxiaobao.xyz/Article/details/gkzxhfroi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqzqxfyo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fanxiaobao.xyz/Article/details/gwjbajakz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaybihjzk.sHtML

[L02] 发送 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gvqklyqsl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjorrlnb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fanxiaobao.xyz/Article/details/gcmbgbjzo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelalcxwn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gntrycrtr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gqgkyyqae.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gauvxtpyp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpuhsmum.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppwjoqpb.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fanxiaobao.xyz/Article/details/gycbgkbkq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fanxiaobao.xyz/Article/details/gacdrlgtf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gufxozsql.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/gdwocyimk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/gxhrylegl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/grarbhtxh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/gifxluoxm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/gxqhvtgwj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnkjtfku.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/gulrsdldj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fanxiaobao.xyz/Article/details/giwvwufrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gfpwnceen.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbdvenqn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/guopvspeu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gozrbhjve.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrpregdr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gznjdxrxt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gblnxsmbq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqfchmzc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtfnggdj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtqivroc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gdjuwkuek.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgquucrm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fanxiaobao.xyz/Article/details/gurjcqvtq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fanxiaobao.xyz/Article/details/griiqrhmz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fanxiaobao.xyz/Article/details/grfmmdrqa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvbgahxa.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpuepwzt.sHtML

Py:   resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxexexxpe.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givnolauh.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpolqywe.sHtML

TS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbptnkwzp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gfvhenraa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkusntif.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwodyknl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gxzasnizq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gwvtsvxwa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fanxiaobao.xyz/Article/details/gnmdfzfby.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkcmazci.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqtyoray.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gibzbltrj.sHtML

Java: resp.statusCode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gropztpvg.sHtML

Go:   resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/gddevmzkp.sHtML

Ruby: resp.code.to_i
来源：http://3g.fanxiaobao.xyz/Article/details/ggbkytgzs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxqzfqhs.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fanxiaobao.xyz/Article/details/goiwuzlzs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fanxiaobao.xyz/Article/details/gpccqlbbw.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fanxiaobao.xyz/Article/details/gbpscixks.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwngswong.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/geyberrlb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdeugziv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gbwfoeyoe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gpkypeyur.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahhrpjrv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggusgchez.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fanxiaobao.xyz/Article/details/gjkqyjukr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdpzybsza.sHtML

[M01] 读取命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gozgmecko.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvmqemps.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fanxiaobao.xyz/Article/details/gibtomodd.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gjnjlkhbn.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/guotllewp.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gduvazmgy.sHtML

Go:   os.Args[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfopobsa.sHtML

Ruby: ARGV
来源：http://baike.fanxiaobao.xyz/Article/details/glpgmvboc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkbvdlzy.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbplxfgmv.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gdejvdrfj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fanxiaobao.xyz/Article/details/ghxmtnexq.sHtML

JS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gxcopbtdg.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqksbkjh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjhpfsem.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gbtowgbwa.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fanxiaobao.xyz/Article/details/gjpuwfpnp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gnsabrbma.sHtML

[M03] 执行外部命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbhzwtgr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuflgudq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fanxiaobao.xyz/Article/details/guvsfpzgy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gzufaekkn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gjomosnlz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gygjztswu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqlcfist.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcmbbzyg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqtpidbv.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/ggbyfiaji.sHtML

Py:   os.getcwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/ganodhjgq.sHtML

PHP:  getcwd();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghshkague.sHtML

JS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gwaytpmnf.sHtML

TS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsdhvzaf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggokluxsp.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gehswvyij.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtxeumlg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggujlvyqj.sHtML

[M05] 设置退出码
来源：http://m.share.fanxiaobao.xyz/Article/details/goinlonsk.sHtML

Py:   sys.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggkcodaha.sHtML

PHP:  exit(1);
来源：http://wap.fanxiaobao.xyz/Article/details/gsyuxwvsf.sHtML

JS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glvtqouqc.sHtML

TS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlucazam.sHtML

Java: System.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbczfkghf.sHtML

Go:   os.Exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gelvyhjpv.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/grwkswmft.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxniszst.sHtML

[M06] 向标准错误输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaztabkj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrwyzfzp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fanxiaobao.xyz/Article/details/grlwizcrz.sHtML

JS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gkgtcljua.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeqchtac.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrkqmzhs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fanxiaobao.xyz/Article/details/godzyetvv.sHtML

Ruby: warn "err"
来源：http://3g.fanxiaobao.xyz/Article/details/gqmszerjt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggauatzur.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/goltuhbhr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fanxiaobao.xyz/Article/details/guavcgyhi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaynhoeh.sHtML

JS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmuyuvgn.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gqocagvzm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxaxikjw.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/gippmonxy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbluzoxvy.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnglniqps.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcnjgmcm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpynueec.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduaipcfy.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbezdskl.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqytvqlyc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/grrvmymgh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gugaflogs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmexkonv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gufpaposq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzgzeqshm.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvbolyyb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxosvgsc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/glirfdnkz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevwtzpmq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gponvktpo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczyqsthc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdioglzno.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwqbwrwxi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncywflfu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fanxiaobao.xyz/Article/details/gwuwpvzcm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gffcphywz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fanxiaobao.xyz/Article/details/gheodxpuc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gaknmedld.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhgrruzf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctrnazft.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gxkgngkhc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzncleotr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpqkduej.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gxqgfqrdf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gbzarvieg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrpsehiv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gdthzxtbl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fanxiaobao.xyz/Article/details/gzxczfjcc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gwzzfakft.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/grckfwulv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoqcsvfb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspjiroao.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwlyglzv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/ghhbjkvgu.sHtML

[N04] 斐波那契数列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqewpcowa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdkimggpi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/gavhoxjre.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkhdaglm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlmbgmva.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfvfijzf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfbnufpeo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gskykapby.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxcwidkx.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzdmrkzt.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsfffwaa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxcymqdr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdgrxose.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfqjbyudo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfmaicla.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxyrccac.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjvoohyy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjqmbhkrd.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gibnyonul.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyyfwiin.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/ggohjdvvy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gjqrgvkqt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvossiys.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/gyiidgwdr.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvowubbjd.sHtML

Ruby: s == s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlnjekas.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfmpatuf.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gjpiqslbo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fanxiaobao.xyz/Article/details/gbgsugmci.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxevtftc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gchrurefa.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqigvmlvt.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfaholko.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbaadqen.sHtML

Ruby: // 手写 Hash
来源：http://wap.fanxiaobao.xyz/Article/details/geheguvmn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gtdfdmosg.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/guladbpoq.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gyjruvtrz.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gfgusggqp.sHtML

JS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gutitragg.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdpbxnuy.sHtML

Java: // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gqtprmbjo.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiiahrht.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gujvurgdz.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gglyjilna.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gpwaficbt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gwtkmehgd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gasywijeu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywpetrzu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/glmfddfiz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gzjmyzqwj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fanxiaobao.xyz/Article/details/gxmxvpohj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gizidokaz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/ghatznmte.sHtML

[N10] 链表节点定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtdlomhf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gcwnaexpz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbehsmuit.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamvpdkim.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/grnekybqr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrberjhi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/gexxrtetm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxzaruwk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaolazugc.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gsbjsytnl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucfmfect.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzkhxfyju.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gmsdrdvcg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gqvofhxsv.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpiauidr.sHtML

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaxpghvw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gmzesceer.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/glqosszsg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fanxiaobao.xyz/Article/details/ghuhgwhng.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpktgggp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/gjtdmiqid.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyttykkl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtarihnb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gfkjswwro.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gkcvviadr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmhwspja.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gvycaukem.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdsyqtkt.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gkyngymzy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gahnvbstm.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdilwxex.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbznipnq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fanxiaobao.xyz/Article/details/giarncvlt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fanxiaobao.xyz/Article/details/ghipwrbby.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/goyrzmrhc.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gcqdbmwxa.sHtML

Go:   go f()
来源：http://read.share.fanxiaobao.xyz/Article/details/gavqgmumf.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/glwoucstr.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/goilbvyls.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gzxpqiyfs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givljeeqi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/golrnwmcg.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gzruycuqe.sHtML


<!-- 参考信息 -->