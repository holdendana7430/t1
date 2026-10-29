代发 wailian999

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gpxjphvop.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gjkukzwcx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gigylsckw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gjahhtoqr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gwsboydhx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gxulogbuj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gnwaiocea.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gynrbedyd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gohvoboan.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gdjlosgly.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gvevcqsto.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gclwtdkam.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gmngkuyya.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gpzpgsbbe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/grqegkore.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gbinrvkmk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gifzsyhyg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gvnmmasas.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gjhlfsptw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpaqfueca.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gwsfllqtt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gogzqoxtm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gwxxhofle.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gafxycebw.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gyncersas.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gmiomlxpa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gjjzzxhpw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gewfmokoq.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/grolswgtj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gczlxdzqz.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gxhkrmrij.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gewefuemj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gwlvgbmdw.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gbvpkrmfd.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gclgqwjdx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/giznscdak.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/grxhactmi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gtrjrfprt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/glkotgexg.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gdfpcddbt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gbjmlguzh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gqqhxmvah.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gkdgbtgvw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gdlflqzxs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gzgefhocj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gxalobxbt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gayxtyeor.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/ggjrrsudo.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gzszvcqzu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/glrtiepcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gslpnsglk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gafuuzwqg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/ghvmpuylm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gvkvpshsf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gvynfimop.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gcrsknocz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/ghwgrxcbr.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gbanxqwlm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gsalqxulm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gcawiuvvq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gbybnxyoe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gifuomrmc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gllnxqyza.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/ggjlkmctl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gxoqsjlaq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gjvjeqeyg.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gupoirtxf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gwhhzqoxm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/ggptxhhlj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/glullspvi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gztlpzduj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gonpqqccz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gtarxseev.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gupfoxmnz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpycgamjh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gpjgttlhe.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gwoxuhjdb.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gvsswfjbi.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gjexkvand.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gfpcuiiwk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gdtozhavu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gqufmqxlk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbmpucsm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gagtcalwv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gktqsnvrc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gywqkkbyb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gpbrjwzuu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/glaudrfjr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gpcwnwfdd.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gluawwgsu.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ghmivnzax.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gafywpjfm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/govkyyttk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gsvlqnczh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gxfqjqnil.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/ghcyakiqk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqgwcuqik.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gxdbjfxoq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gisbwjbuc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/golisuaoq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gzocmenpg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gbdqrrjqb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcxpnxvug.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gcvcwlwih.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtehzikpw.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gawlmewuq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gzomeogfm.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gnsdawaln.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gsrseyxez.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gpwrtcljz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/ghqsjawsi.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gxcdpoqhm.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gmayltgzx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gziqcisfi.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gebbyqzad.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/grjlrsqnx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gnkckvyos.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gparhbyqi.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gqamkvgbw.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/guzfptllj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gangurayq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/glueeukly.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gkxsvvfem.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gyfeaspad.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gogdqmnjt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/guadiesnx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gjpzmjukf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gwxtccbja.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gcgjfartd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gbekmvnci.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/glkjygyjh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gibyqqffs.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gtdjewxob.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gecnsnfrm.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/ghhslslgo.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gyzlmifyf.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzrgzwwwl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gdiykoxtp.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/geqgkarsb.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/geccajcha.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gughwklpg.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gzauznpqd.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmwakijiv.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gjtmmywso.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gfyuoscla.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqpvnlred.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbtfcwhgm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gotadtjmg.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gijtmltye.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gypsjgjym.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gldzjwnpt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gfooswlkt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gsgckyvkl.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gwxbocvbc.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gowdwozfa.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/grrkuevnz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gvhvtrhxm.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gsfsngcpm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/glmbdsixq.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gxkapfevh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gvynbones.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gaizqqpjn.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gfzyoaywa.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gvpapkkib.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/grqpomdxw.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gsdmvddvz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gpkgwpajf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/glbwpqiqd.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gjakmrenz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gpbfflbxi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gudllsgnn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/glshwmhdo.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gapgpkznl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/ghriqsycm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/grlzhrnvl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gixourtkc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gsomsnltk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdtpdzoay.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/galfpbnhk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gczohsnjx.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gytmfzeup.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqpryqsbb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/govjcaxnz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/goldavmid.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gmjrjrnpe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gqozeyhdk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gyzjxblvu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gfoqnozof.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqhpvssqd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gzpltgcuq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gcymidxhw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gqqirmnuq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gahjzzkfj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gzwzrvzsh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/guzydhapa.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/goghflyag.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gldykzxwp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gchlmxcjj.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/govcnifvi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gtepzjuhu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gjyrxqasp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gdigpvasc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gyinrcumn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gotutntxn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gkbnxkxee.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gfsozgrjw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gzkokbuxp.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gqlwxabru.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gksqyyzvb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gubvlhvnl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gwuwqauyu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjqspfhhv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gtiikmcco.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gkzzwwuqc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gigomnwtm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjnmrblbq.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gamvobyrn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gvgadrpbh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gzjvegfnw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gpovyyflu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gqcxchjse.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gupcnmeyj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gixgfxzcj.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gcdyetyru.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gncopblmf.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/goyfulixc.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gyddxiwal.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gigpkgqlv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gadlrksqj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghmcdsnit.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gjxnhnjyz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/grewsqvdd.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gxsafuxlp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gxpnhgpzy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gjwveuolz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/geputtrqt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gkkoqfvko.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gguqzmkrw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gbjrbhiii.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/grufbgffy.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/graysivyw.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/ghobqhzjn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gnmuowbba.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gupebpzad.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gmpzwsees.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gaedkmbdp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gacsdfqxm.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqwzirkve.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpmjtbnda.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/geugselvv.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gedaucnjb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gcggazgff.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/grqjqucar.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpladvqfy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnpzhipkn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/geyrpgcip.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gcifzmogq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gpkpiuddi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gdyuchklg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gtxewfgni.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gukzlqmpr.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gnzrlpcqo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/glbwijqog.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gvaguqimn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gfaaxwgso.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gfrrbukvm.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gahvttdwl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gfceagefg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gzehuxjrj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gphppfdbc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/geefuknfb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/ghipthlsl.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/glxdzqwoq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gmofqtboc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gychkgvuw.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gmbvsxnwx.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gjbqlpdmn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gauyqrofb.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gavkbonbc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/grenbrwwv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gsxohokii.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/greuzrmwi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gkhmqffpn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gvkbizled.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gvqvkuzha.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gclgmdqll.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gunafskke.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gmtlenjkj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxdrjvoad.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gqurczhpd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqfeixhiz.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gwwudlzmo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gldlvbdps.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gbzebcllk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gfaokzdbp.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gatukhogb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gymsojalb.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gvkedolap.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/ggucgglgc.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gzrsyorjm.sHtML


<!-- 参考信息 -->