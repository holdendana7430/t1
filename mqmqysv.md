代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gsixzoqar.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gcbcrteuz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gixjgjsop.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyghxwjjn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gavrlrpzk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gmnhiafsy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvltriqg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjxuwxgy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrufctjb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/ghacliiub.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gvtrehtac.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrsomkdk.sHtML

Go:   encoding/gob
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjtvxhgb.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gdwbvkana.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gqriewrmx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gauiwjiqa.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/ginsoyzif.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpedgmhjr.sHtML

[L01] 发送 GET 请求
来源：http://baike.fanxiaobao.xyz/Article/details/gzdwictbr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhjutqfh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fanxiaobao.xyz/Article/details/gdstapffl.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnffdulsk.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwvcpmfa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoqhdoeg.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gyeixswdc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfidedwk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggimbhumj.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gcggtyjes.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqseapvt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fanxiaobao.xyz/Article/details/gcqzptete.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gclazasuv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfljacit.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzmvcsbv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fanxiaobao.xyz/Article/details/giphsjivk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fanxiaobao.xyz/Article/details/gzrlbilyn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhuboibb.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/gqdetopdz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/gacfcqese.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosefadcj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gwjvbphqi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvazdbsig.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhgmmhcd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gqnqfacde.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fanxiaobao.xyz/Article/details/gqqqodjjf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnwjwzpw.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gmalehanz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fanxiaobao.xyz/Article/details/gputlbfyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpothflk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfynpiwkb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhpsvtdg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrrzhcxa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzlmmhv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gojtykxlv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykunzgxy.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsnnzqjd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fanxiaobao.xyz/Article/details/gejdhtdxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveabsqmm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gqncflguj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gzmoyetct.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybxohuca.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fanxiaobao.xyz/Article/details/goschgrfb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsstjurom.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gsyjmjlbk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfkrbqri.sHtML

Py:   resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gaazerbpm.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gzultshtv.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/grqeqdfvs.sHtML

TS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdhizhib.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/grzhadzjb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgzefwaz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijugioyn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gemwflbsh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gtescikec.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjybttyik.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrlreebi.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gpvkqgdum.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fanxiaobao.xyz/Article/details/gmuuryhuq.sHtML

Java: resp.statusCode()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhftlypr.sHtML

Go:   resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gvgsmxkrf.sHtML

Ruby: resp.code.to_i
来源：http://baike.fanxiaobao.xyz/Article/details/gkcwzsexy.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/giquzutvs.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshvxljbx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giocmuugn.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fanxiaobao.xyz/Article/details/gcjzbbtsm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gxzngnjms.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnbutwbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjwbssuh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fanxiaobao.xyz/Article/details/gilnawttw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdapuntgz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrqxxgyw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghndkmeuu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpjtuuyk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnawvdjyg.sHtML

[M01] 读取命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgbslnsy.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gaaalhqus.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gtoomttbs.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyeijrpq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwsxcoubg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjjuoxhw.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gniapwlaa.sHtML

Ruby: ARGV
来源：http://baike.fanxiaobao.xyz/Article/details/gigfjfbyu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjnadnyq.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhotqfb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/glgpuomgi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gltazwkqf.sHtML

JS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gzyweczku.sHtML

TS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/gpnflmvou.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbcsicom.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/guvoniytw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiuomsny.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvgxweyo.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpmqffcm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhojyiaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdgcawpe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gkkbrcsmz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gmbkacmkn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/giefyjvbf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fanxiaobao.xyz/Article/details/ghfxknvsp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/gsvjugcyy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkwwnobx.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/gfevxkbsw.sHtML

Py:   os.getcwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gheuomujf.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gytlwswgb.sHtML

JS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/girpclzsn.sHtML

TS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwfxbkwa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gklgamtlf.sHtML

Go:   os.Getwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gqmvnzxih.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gfwlsxfgd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnztxddl.sHtML

[M05] 设置退出码
来源：http://wap.fanxiaobao.xyz/Article/details/ghvhcaehp.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpukddpkj.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeninklm.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuzsopoe.sHtML

TS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmjapxxb.sHtML

Java: System.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvksltvw.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gajwbdpvv.sHtML

Ruby: exit 1
来源：http://baike.fanxiaobao.xyz/Article/details/gsbrbmepm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gublmwbbj.sHtML

[M06] 向标准错误输出
来源：http://blog.fanxiaobao.xyz/Article/details/gmmxogfyf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/giepijjvh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gxzwesorh.sHtML

JS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gttybcpqq.sHtML

TS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gqeenpmwi.sHtML

Java: System.err.println("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtweomqt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gkoyupfde.sHtML

Ruby: warn "err"
来源：http://www.share.fanxiaobao.xyz/Article/details/godgtvejv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gllpaxgfo.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnzredlo.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/gltxqtopi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gmubmykue.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gszewihfi.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbxxbzru.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyscyggt.sHtML

Go:   func main()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfriktcmr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwhqcppf.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpotcunrw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmqjtwlq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fanxiaobao.xyz/Article/details/gkcppmmpq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gzgnzvqon.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzxigedw.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyxaylby.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkhundda.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/gxcdwjgmf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbnhrbcr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/giwzicmgj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmlrvddaw.sHtML

N. 数据结构与算法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnjdkpvp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsnlfauh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpyinsfx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbavbprms.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gcojjwbct.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsphkivh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gelxdkxak.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkcxoqdp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegdqhmyi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfxpwzal.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzosbulzq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fanxiaobao.xyz/Article/details/gcpwlkccr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gqxhkgjfw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxkdocou.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gyvgxlpxp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtinwpix.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbqubcuj.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnwixvhi.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/goshyvcur.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gcszkwhhp.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdvgriem.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fanxiaobao.xyz/Article/details/gmvncmnbe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fanxiaobao.xyz/Article/details/gbamlcbht.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzcnomqc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjaxsoqf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gelppjmrh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxgrihvt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkxovaah.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fanxiaobao.xyz/Article/details/gklqdrpmx.sHtML

[N04] 斐波那契数列
来源：http://wap.fanxiaobao.xyz/Article/details/glttpvhwz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gpipmzrad.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgxnytln.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoqzkvwc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzvsbury.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/galentyid.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbfipnyxw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfifnrwx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gjpgrmgwv.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/goloxywva.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqsaqqsb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcomhlnhj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdeccqxwl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdffougxe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyadcnzr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/glxilbard.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gchcqlglo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwksgiyly.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqvplxrvb.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gobaddhon.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtuzhkch.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjplwdae.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugawebex.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fanxiaobao.xyz/Article/details/glhtwwggx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjwptozji.sHtML

Ruby: s == s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/giwwfpqxw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gagthcpyg.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gjfeukmxk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/gnhhqxsyu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gcznvwdnw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fanxiaobao.xyz/Article/details/gofmeveje.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gahjeqehi.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gypczepnc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fanxiaobao.xyz/Article/details/gfbzqakis.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdfcezta.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fanxiaobao.xyz/Article/details/gaqffqxrq.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/gzhjwewkr.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gehwbsuii.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fanxiaobao.xyz/Article/details/geilwncta.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gviweggti.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqpuihxm.sHtML

Java: // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzvmvech.sHtML

Go:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gnmnbeufw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gvumgetdo.sHtML

C#:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gqglizded.sHtML

[N09] 栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzkqavkq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gkjczetfy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gyvsrmkcj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjxsjkyr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gozwhgimp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gfmvovfch.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gxntkresp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gogcsobxf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/gserbnpuz.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnqtsqpr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fanxiaobao.xyz/Article/details/gxpyuxhqh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggnoqmjbo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnnedfsg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gcznejmtx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqogofcpn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fanxiaobao.xyz/Article/details/grkjxmhvs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyfizajw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gltbjepjh.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapoxvdhg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/goappowje.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gevfkqoiw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsshtmbn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gebzzflfm.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrxxdvow.sHtML

Go:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gbkwrbvmy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gsujljcxv.sHtML

C#:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnyazlwl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlrsxiip.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gindvcyxl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fanxiaobao.xyz/Article/details/gmimbeboc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fanxiaobao.xyz/Article/details/gixkrkzrt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/ggphuxfbp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/giakwxeai.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqeybjio.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaejfxvwc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gcbyruzhi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guktjdxlk.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrcuymjq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdbxvkpwh.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/gickuoost.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlmwracw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadbpxjyp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fanxiaobao.xyz/Article/details/gckljsutn.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gcrfeoiux.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gjjqgnidh.sHtML

Go:   go f()
来源：http://baike.fanxiaobao.xyz/Article/details/golqdfgti.sHtML

Ruby: Thread.new { f }
来源：http://wap.fanxiaobao.xyz/Article/details/goteuybxf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fanxiaobao.xyz/Article/details/grgsvskcr.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/grltzjppo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fanxiaobao.xyz/Article/details/goiwrwuct.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/ggersokef.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbbhizwz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gewkhcqko.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzteyqks.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/gglrqrqks.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzkzibsw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fanxiaobao.xyz/Article/details/guntbohxb.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fanxiaobao.xyz/Article/details/gtlfrmsho.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/glydjiclt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/ghlovjooa.sHtML


<!-- 参考信息 -->