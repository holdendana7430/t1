代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/grlfvmjss.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/glhpsuwas.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gwhncufla.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gmopyukgx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gndtybews.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gcptbkljr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gouxkrddx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gvmvjasxg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gzknxacsc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gavgdltjw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gfvsaomtf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/glklrkocx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gsfgghzng.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gdzbyarwj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gewbuafnk.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gssevcuuo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gvaokncsz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gsswirvrw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gejbmaidd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gribpgxtk.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/glczrzwoy.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gzhalalxa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/grplajiie.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxnvmltuy.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gmkvxxdjv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkyomxpdo.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gioamfjvh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gskvcdtoq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gsnoexget.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gsfwbcegd.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gcwzfhtyz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/glpzsnchj.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gkoxifdon.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gmmmbzmmm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gwjveqirp.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gsbakygpn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gizlpofyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gkxevfhju.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/glelmxdvu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gmrdkslxx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gczfoudwa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gzwhsxqgh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gxylryebr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gzvrinirb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gsqaqudgh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gyfrtaasa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/geavluxas.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gqylcszii.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gglzqbvbh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gthmfuxeb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gacgsfbue.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/ggorxebma.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/grlhfrjff.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gbanuxavq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gilyviygi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gfsislfjq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gwbbaiiro.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqdhvti.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/geqyiakww.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gbfewlmag.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gcvgknzwp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gqfziwerg.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gorqeiiay.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gjrpzkden.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gvtcgiwvu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gnrtarjra.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gdrcrvhwn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gnqsrekmy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gessghugw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/ggisdwgea.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfesxgbbx.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gezbdzxyy.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gxsetwtym.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gljbpkruj.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/ghpccewhc.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gobihzuiw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gmlmoczou.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/grkjhpegu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gtbqzsykm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/ghptntmyx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gcyrpfhdg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gqoqacqky.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gkqexbljp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gwxizlebq.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gijcaxquz.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/goragkzyg.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gawnfmhhf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gffukmnch.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gzmqhbhtg.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gitnzsqtv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gzcekvekb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/glqselrbo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gnesfcuju.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/glcxyolyq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/grawffwwq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gdpnvgxim.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gilzimnjj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gzbxqpxpy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqlqlzdol.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/grpfskxij.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gncegwmsz.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gkbcvavno.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gczgniico.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/ggdcqvaxh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gaowgfcsk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gyazccpyz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gireshmfw.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gwtxuqieh.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gszhsisdt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gtmrrbqha.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gdouuaffp.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gjibzbepe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gvjdxtqzm.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gimamrnzk.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gzzstwrgg.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxujedosm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gtjkxsyyz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gznxobvyl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmzmrhazm.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gdywvsvbz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gfwfdmhzo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gszaicohj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gbxqucghg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gisrggmfe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/giejamajl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/guprhvayp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gknmemfci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gnncgmdyo.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gzzalojiy.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/ghwlujkto.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gfunryibv.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gnyazywyd.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gadvppexm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gaauyvteb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gegwlzcfh.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gewqwplxq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gsycgsbnp.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gszctabaf.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gywfhuiin.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gmaewqlbo.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpmlvjwbm.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gymiioqqn.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggmkteene.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpkllacdw.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gjwhdslkd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gpqidbbzk.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gvdocqasd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gesfjgkqh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gzobttuas.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gxvduckmz.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gkomieruh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gazfoqfne.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gbgmnkjxt.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gecwbbxnv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gktxmjfqu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gupvugdil.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gmpudohvp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/geprjdnlh.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/guofflwxo.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gvwgudiwa.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gsbmmjzup.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/ganlgaffe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gruoosmcv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gqbjpsnva.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gtvllqifr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gptbiqbcp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gjdclnidx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gnahffqil.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gsezoxzwg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gvybimjlr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gdevgqkuq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/ghmujqjbc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gkpmfwhmk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyjwhdsmh.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gpaddchpw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkpgrwjei.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gzcyfyqbn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjzfegblx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/ghxrsohuu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzcccwdi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gsdxdxqiv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvrethdwi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggkildiao.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gcecirplo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggbaxiudl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gxwbxyeho.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gwcztvwpn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxkufphrb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gyljlfvrm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gwqfmrxpu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gpdsszjup.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gaeppbcue.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gafjqeyab.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gwitvumqw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gyggbchor.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/geylikffg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gqfwuqevo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/glvdprlij.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gicuombec.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gasulqocg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gzrjxstet.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gvzlfwfhm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gprviwdlk.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/giwigajfm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gmiphuhlt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/glggjeakb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gbqofigym.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gydcobpwl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/guynaxszx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gmaltfcre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gnclxdyrj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gaoxhbjuw.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gczgoeucb.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gotfhgfed.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gkeimzvni.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gpmmgsgve.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gmgdsqltu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/grbrakmhx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gldbfbdnd.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gdtvcvkip.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gvymerszm.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gkvvpmgqt.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gmjwxmnxh.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghwienvsl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gllmouunn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gibezecxy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/geaysyaao.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gccmdhvte.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/grtdcaglh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gpbudztto.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gaonpvioo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gyoexdtmn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gmguxvjib.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/giyqvvcpb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gsokzusyf.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gbiumoely.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gkkmyvssr.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/ggwovzouu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gwxaeonxy.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gwfbuydok.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gfeyvjfno.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/giknzqgaw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grrstiuit.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/goieresps.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcqvlbbsl.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqgjnwrcn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gtltnpiyl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwoarjhkz.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpwvwcmkl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gxaqibdcd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gzjtljtin.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gcrzemdvo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/glgjpbags.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gpjlepouv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gpvkaynhh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/glxldjtmx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gasowcbyh.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/ggmlplhgs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gbwfnyajv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gijtzoueu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gbdwgbgmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/ggmuazkui.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gknvmdoab.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gufsuuupn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gcwwgviej.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/guohwabdv.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmbhmfkyi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gykqwhsim.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gzczeycfl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gbceoebat.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gsdigtful.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gnpuuevcz.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gkjpijzyq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gekudjobl.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gjjwjongw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/getmhmsis.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gbkywmfgu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gmadhtagm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gwdgtpnsu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gptzsgnrz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gjbfoapwp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gejssdpqp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/grplweazj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/grxnegmwe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvwpdqmkb.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gppucxmrv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxquelwiq.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gtmscqaei.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gbehrclgw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gpzulnals.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gifgkkyiv.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gppckwmax.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gnqtbhhat.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gphqiavjd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gdizoxajo.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gbgrksbrk.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gusjtjdqx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gfpjcygjf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gzfwzsnoz.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gganrbdpa.sHtML


<!-- 参考信息 -->