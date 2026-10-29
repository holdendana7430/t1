代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gmqdkbkwq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/giksiuddd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/guspzeqhv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gwabjyyaq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gjfjiiehy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gmhvsjiwz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ghoqrpbwp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gvjxdgeea.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gzzqedqtg.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gvpiqlsts.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/grevmxlpc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gwmlxazcg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gnbtucmkl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gjcxtdygc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gtqmfimgf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gtickxwzh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gfpmhfggy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gchwhyauz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gafarhoqv.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/ggtsagmbm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gownogjuf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gppkygywk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/ganurymrl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gvqquwsof.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gfhxstmvj.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gtbsitivg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gggukyxre.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnuqlncar.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/ghozmkepd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkhvzvxpj.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gjmhcstjc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gjqvkmhxg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/ghtoncmwv.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/giiklsvpz.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gmaeivppm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gddomaabm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gliomplaw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gbcqwwwtf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gucdszljl.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gijzatcmr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gfntvxgfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gfjpmswmb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gtwyycdlw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gcjjyytsy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjlitokh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gouexytbm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gxeiaoazs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/glkbyhugc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gbnkwkbya.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gaoysgzke.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gfmyrtxsl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gieoynlnf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gwyrztvpa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gnchnaljl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gfhfkdbjs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gcmswzzla.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/glyuknjmi.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gatpkgexy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gtmxfqpue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gykbggijz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gehwqcfjo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gbgjqvich.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/ghxhyphyx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/ggldbmsne.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gqpedauqc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/ghuhdtgsw.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gfagvhyeb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gxzpdybcn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/golvpwaso.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gdqptccfh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gcuicvmxk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gaspfgptx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gexrkrjki.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gfmbtsxyi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gycoyhvsf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/guxdqqcro.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gzlwtyhsk.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gzrsyctaz.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gumatglua.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/ggepciiem.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gdaufbojl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/grxxzhndu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gqkoqorxg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/ghqgrqdbt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ghhgqegfq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gavpjfxzs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/ghpkldbvr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gqezbtixe.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gevragdfc.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gkwpfggbp.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/garodrkqc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gnjmvlrdz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gnkdvaoht.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gwyabaqrd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gdvzvvzhb.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gtjvpbsps.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gvchwjvsc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gwtldjkuy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gutnfxgik.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gojqzcmox.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gtviuueon.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/goinfuzks.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvwcvqhkm.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/grpwwfvfs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glbkgsvqa.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gyhtjrkuk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gujegdmkr.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gynxxfqmo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/ggmqvnawn.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/guklocjiv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gzstpphoo.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gjbygghnh.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gbnsyshwe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gjfslajne.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gsyhhfxyt.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/ghdpyqtdk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/getydcqmj.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gbkqknvlv.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gxjwvglfk.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gzhcyfbkj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/grimkxlpo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gdgxjskxr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/grdbkpyyv.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gcdcwyvwh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gsoffhurl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gbuhaolrw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gqaqnsxln.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gegihqlli.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/geihowjed.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gzvsdiacd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gpkcvmfjr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gagwbpnmq.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/grfjatjvz.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gzzzkrmyk.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/grwnkzzht.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gkueglxxo.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gcwdjhspn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gbsnjnczd.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gcckcdbet.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gcnmvfjet.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gcdpvdmqn.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gmgldjyig.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gevcgyzri.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gqjnjqvbp.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gohnusmtj.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnjwpnjfg.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ghxreivts.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gllmnyjsl.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gcecvhvsj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gjcopjsyj.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gnxjkrajx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/ggjgaphtm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gjajtyxss.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gromfwsmm.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/giybmknaz.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gygqmxgwr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gyvctjvjb.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gmiajnqht.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gseeowabi.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gfitcntrh.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gtuavjbwz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/ggqgmomlk.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gybddhliw.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gpbbzjwvz.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gragbxcxn.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/godxkltab.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gvqnzgcry.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gqyamahcy.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gornqfmxk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsfxysb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gowztjsvp.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gszbadfri.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gfpqyewhu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gpojwpopp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/ghnbbfgjd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/goygjyvad.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/guwnbkukx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gymjvylpd.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/ggtlgkyqy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvfditzyt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gswwshdrf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gintsfncr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gtroescia.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gqfmawbms.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gptbhbnga.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ginuspmnm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gyoajoraz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gchglqahp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsohhysqy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gbjdwwrwf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/godmvunsi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gohvwojfn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gsjbmraxb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbqogmuqj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gabxkviaq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gokqbuver.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqxobsvro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gemttrbds.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gyaurxdut.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gpfcgylst.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gvrqssvsd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gabpncnpu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gyzpiwqqy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gzpqewzrh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/giejfbwtk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gbmxumbag.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gkaxhhckm.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/giawezujt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gyzdfaunm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gixkrbmht.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gqkktonnj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/grwqsjraz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gvtfbhyqg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/ghtzjrhlv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gaqzwpovf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghjrodcwc.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gosvbiwmm.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gjrnrumyv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gqwqddjkc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gvycftxbh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gdswwtqmq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gityvjrgq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcuzejaui.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/givgrdale.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gitxvqice.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gefwlztzg.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gddnzwaiz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gmmuynlso.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/grjwfklgv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdnxutrle.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gnanxaepb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gczhgipvp.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gpoawdrcy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gwpwbiztl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gpmimtwwc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gvwjkdaah.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gpzsenapt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/grycyexye.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gggrhqpdb.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gdxpjjwek.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/geprpqhfg.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gatmxxokw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gipbfdbkr.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gkfbatexw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gynthlmir.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gcswmxytz.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbxmkmlfv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gcfaupkwm.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grcknznou.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxrciywkf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gydyuxjro.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghuxrnyvz.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/guitbnkte.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gikijwttg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/grlgejujf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gipticocq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gcrrefvfk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/goqrilnzu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/glvizarac.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gdjhydgfy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gqtrtipen.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gtrjsiuqz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gizwmtexw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gdxhccrkr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gikkyordz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gsdruajlm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gevdnytxi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gtpcpykqg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gafoaifda.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gmjwrhnte.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gexilhffy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gecmzmujz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/grtfjdeca.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/govgdiziz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gioqbusbv.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/godiijmbc.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gunxsqiqo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gjcmecjgq.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gwlvmhjot.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gtxgsxntn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gbpouomsa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/glgkpyahm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/ggzyysapj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gxaraocgm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/glhjhzlnb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gscndwgmw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/guxolodvy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gnhmzxcym.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpkbvfmgd.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gmkdxkhdt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghqqfpvou.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gvoarymnx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gvztzfbbi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gotcxypqw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/ggdihbinc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gsmqfsjsb.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/growppsea.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/ghrzjxcjf.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gtowtpgrs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gmrueabmo.sHtML


<!-- 参考信息 -->