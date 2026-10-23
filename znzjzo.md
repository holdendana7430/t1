代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bwipdvhc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3onrbectc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3oikblqoi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lobnbena.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uonuwouh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3eszhdakv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ayriwwts.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gdpobxdi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uoezwwaj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3edbzblql.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3odghvapb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ysbhnmvh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3aydctyfy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fklcsaiz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ozepuebe.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bapwcqjx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rtagvkpd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qltuomkp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ytbillih.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3gewsluzd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3pqfwaqvw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3klzvrahz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tmhhxkya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slziavff.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bmnzzmsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbajldcq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ydcvhash.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3clswmpis.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3mistqelt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dajhgzyq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3scylzdky.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3owsitzvs.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fvetmgln.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3yyajveqq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ziudbdld.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pmmwfmwg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vzfqfhed.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3oykhigpd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rxxpyghw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tisorifq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uxqjsiyf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xzfevftx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ztjqerct.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rbkvgjii.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qrkmxnsv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3aplptblc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aqgsqxbs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3yzgmtnym.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uyfpfjbx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vthzryhu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ubnnveks.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3jamietyz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xizsoekk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hdcxwokf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3teclbgke.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gisupzki.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wozdlgxh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ybwuwyjv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vsefpiep.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3weqhcgvh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ksvusyey.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dolflndl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3eeetdyfz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qhdlrgjl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3svnevpxa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wuiimlft.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ceyjanon.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3soznhjsl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lsocpwrc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ayqqfpch.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cerliqlr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3upanfvah.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bivcsftf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cecadxlj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pjwgxlst.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xwtotjla.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fujqjuuz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jafhjwwg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bpvkwenj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3dsgqapml.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ktdygwec.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vsorabtv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ztilfjrq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3etvpuhtm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qhczxcsi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3acizhjza.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fzfnjtxs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ispvfkuf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tjthkjtg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qtdqanih.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pmtatdwt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hstydici.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wjdwzkvb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tqwpeatb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mdwkavfo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3skcxyxzl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qwamrfew.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zfjonlbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrqhtueu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gzqmxojx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szcizcpf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3stdzfynl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3teuamcsr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bdnosvlm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aybmrsbp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojthygrm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vmetkray.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ncmttuie.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3oqlcjcxw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rvmblhrx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bpkdpozq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xdiapxxh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gahccbou.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ouxmaflr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3haqitkqb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cucxrkxh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wmuhkrmc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3azkiugxp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3srcxpsxb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3grrtbaxj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3shnapxzr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lfviwbig.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lfkkvztc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lhuywpvq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hfngzigp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fhzivgvl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lyuznrym.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nnmmbjpa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zojdrwka.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xodbyols.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3icjekuxb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rxymwjhd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3spcvztsp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jojhwvez.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qwmmbkoo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3acfamucg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gcbyagxw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ymnufaee.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kceiexqz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qkyracua.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdfkmpuk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kctyueah.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sjkzcoag.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfdkegic.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wcwqfgth.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tytqsghy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tozuvscj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hjtbfclo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iihkuwgo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dkpzyngs.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hwabewic.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3meqvsclc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3cczohngz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hcrjzfoa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tgjzbbtb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3trhxwgql.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qqyayssr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uvhmnacf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bnpudekd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rxfnjejv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cckqovfx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cpbzxdts.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cqiauisp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3atfeuxwl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3unpvvqag.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3viiteohq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3btlahgae.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nbfuwsyd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hjopcvkk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ubhckalr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lyrzwnhh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3mxqawwlo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rotxcqpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qveocqew.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3tckiqcmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyulvkel.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bimsbakh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umgbdsug.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xfkmuenv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fqfhybxu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gnypxtim.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uppulokl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwgrgobz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vdnolvio.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkwsacj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xfjdfkkf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ndikdhiv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wicgeota.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3txxbswbr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ljlzwcap.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ekqghzvt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3syyqonhy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jfjsilpt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gjioopby.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ahkyqsam.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wbfmhapp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jqxjxdvo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wkpzjoui.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3znlaftai.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xvkdjouh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3avcgnzaj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3eqcbsgqo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3onvvumrr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3iinsykfi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wnltjbxs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3osjfevqg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cpocymmg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dhoipxjy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dlhpycdz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3krbqrczr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikikrkvb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mpwtudth.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3quaoidea.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3boeurpcr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mrvjibuv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahetovmi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkkdpavd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3nngkytah.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nyrxiibo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iqmuhtdt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3buqpgbxn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qhsshiay.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3npxgoglq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ppcxnyyv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ebbswqqs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jabnpjbu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fuhcmwmg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hustlrwv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lagmgkcs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ffxedltx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3celfoytz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xwjjovwq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mlefbhcp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ezxsofcs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qymlnopb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3anintrwy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3uegbqcwv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yxlosdxj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vgxdbfxm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bhsvjoqz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtpnqbgq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cwijudgr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cpkvjhzk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nmlxipgg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wrcxtovy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmehtgwx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nbzrsaou.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uxcckkat.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bzrycqfm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rowphxwc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ukbxyles.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3muzmfggq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fqxmkntg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nrmhcyho.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3amidriqb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yvayauax.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3crokwldk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gfdzfvuh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3eocmqnxa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxktyafj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzeeqty.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3haouhheq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmconulo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3nbivsnmt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fexnxnhy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjuifpdp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3smnvhhrs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3znydhcav.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3aepftmvu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ufcsvdvf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zzsygmiz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ovujvotq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ykehowyv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gnwrjltl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rwaoploq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3msxydkia.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uuiznkjy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3iayabpkn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wfuxzmhb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kdpseprh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lmctftvh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3usufnkzr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rbtpswax.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hwljiiqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mppxjiro.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hsqahlee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqtppuav.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xlllevyd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dtyehjqe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mjheqyqu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kzuicfsm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mwtvdlfd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3riocveay.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uaxexdns.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3scxlzyqo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fmogefbf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mgjjtmku.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fdnwybxv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hisizkjl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eleyiuts.html


<!-- 参考信息 -->