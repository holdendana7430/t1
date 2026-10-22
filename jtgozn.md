代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2odwxtkrw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2uaidbcvm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pwrqhtcw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2hnpowskk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2knudhxqi.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2spmqjrih.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2obokcaxc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lokwbtro.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2uezvyskh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2pqsawuxa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2udwmcacs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2epakpetw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kcoefuyc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hxjgjxmf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2hicfbulc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gjieappa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2alwokrck.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2lknnhmod.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sbzdmcie.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mrnzurnm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jkepwpvi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ubqrjfpa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dovrfsnc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2arbjwcyk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nuqguxjm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rnwigrjg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zhtbylfq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2acicdobc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hggbjhla.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kfcinfrn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2hllesgdg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lpjfzlwl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tsokfctc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mlnybbvw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tofuutpf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fdqljofq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rnnngqnv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zooxnmqw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hbzmhjvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2titjqswu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jxyzcrmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qduqkmgj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2uppicpod.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2buqauyjq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jgxmwxzr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iplakhxf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2indkgfkn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2bfehmpor.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hibdiyzg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xklnbhfl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2oilemkhh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pgsgaqbj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2raejctsm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2chwkefko.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tuurizqv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2anhtxlgu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2xmiyepxk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hvwsdkci.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2pgyxisre.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2asyfshbc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kimrqgei.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2lrjypejq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hbamchgf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mwyeangc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zjbmpyyt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yrcoklzr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iacgpoeu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fxgzmedp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qfzwtowl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sxfksmro.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjgwwpn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2fhhrrbuk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mppusxxk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jfvqwgfx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vhollagc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rofgacrj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2sdsiozdw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wvxrivbd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ghvnuwgn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2clnvoaxt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rfpswpwf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kgycdkav.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bovoxjfm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2gixnkctm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ynjarycq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jbgjdkrx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sjslgkgp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xakpwpkl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tcpegkvd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lfiviywc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ukhbufny.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wmbxgjsp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jvujiotr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2frpwvxjq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2qfbnwhcb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lobqbtrm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rkpdkgdi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zteuzayf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2owybzoqx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lozsipea.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gapnrknp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2tfleyftd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tqziwqyr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cvyxwzac.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2npweincb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ehnpzwmv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iafrputa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jsnxskje.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hprxizhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tcvswgjd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zqxjjang.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ihxvjodq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fmuuodnv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ejlnnhbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbjwzwvc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gzkvkbzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kphifhmg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jcteassw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2vdsuruwh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tvmddxbo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnykckja.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xchdbitz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2itskrbhl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2szhnnrlw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vjhfketo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bnmgtzvy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ldahatgx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2afuwxokf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pfwtsbgq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tlpiiyoc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qqvdngno.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eeoldnuv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2byviijts.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pavdeyzm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qtevqejw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qwrfnpxa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2djracolg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zqtgixmd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xraeclcr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zfrksato.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wophreff.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2diywutpf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vqaortrq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pjajsepl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xegxkzas.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2iezjyfaj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2grfoewah.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nkwuanab.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cmdhfbgg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2yiehxfmy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qzujajfc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wafaruag.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bcbently.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cpkglrce.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qxbbtudd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gckvnkcl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wneqrnnl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqeqakif.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kgqxgqdq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eudqoaqf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgklgpfi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lsobarjs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cfpecaaj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uggwiekf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kjfqkmjw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2owxrjygn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jaziykya.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ofhzvaib.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jqctgnse.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xshpgdia.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pydtjgug.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ztqyfgbk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2uzwxwivp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ybwncmib.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dgfovdyd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2umuxdkmk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mriwzgzn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fryxrtno.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2imbofefp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wvilflvd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rppeltbm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2sihotwlp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xpekxazb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uzdiikaz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uewxifji.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zvinjegj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2lzgagdcl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2oexhcmuh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vamuvekp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtxlubju.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zdyhuole.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shswretw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lmhnmizh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2htodintv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ldxzknzc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2akgojahx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lpoyutns.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnybjzpj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2maxrxhvb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fyokhsat.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dfdtbgpd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ojuxofeb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bmnoqlyp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2alzdddwq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mkrbufhk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcwasryw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2fbecfiqv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zutvogwp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2svenautl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vrqpxsxp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2fmijdgpc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ontsohjj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bjyymqmc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mbuxdzjg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wnhlrvin.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ngcvkfmi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rbuontvs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zrwnngft.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vollfzpj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zqofxkwi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hzmywoeq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eslpxdfy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ehbscpfa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odauidnf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kaaqhhsh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zewhfeta.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2onapvudn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qrelgpdt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fgsisczo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xxpelhlt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2khaykkal.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fengzqix.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntsyhzoj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qztgqhdo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2urukxfnh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfulmkw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2blpxbnpt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jtyvornj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yqfdvxoj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mhlxylqt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pzcnwwwz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2olmgfqix.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2npoekgue.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xmcmcbmh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tlgekcbx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lniqimuk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2whuklext.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tikibvro.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mavaxnse.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhbxarv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qykfcxtc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ablfkesm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dhhamsoh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bfxbmafo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2riaqmhep.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kbtvhjiq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqvazuv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fhpmcxqp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ojfgcyld.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fsfjqowj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xlxdzzer.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jwzmclif.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cdxhcdyr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ehqyjmvf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vlmflpmn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ctpbwfrs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydlpeqba.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uspsbsav.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jcpcnydi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iqkngtfd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2oiaqluwr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cjgcsvcc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pwuyqzns.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jxizrsew.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bemhgynf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvitmcii.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yumgabib.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tvjlomzm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tefwizbi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ghrfrskn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ygmltlkg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjfrkdfv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xnvfzkbl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hxevtrug.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpijqgqp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lqsgbrpj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2orjdvvah.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ufhgttqf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ijyuzpgd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jlhqhdza.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xacmcwjf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kxwyhzby.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2athbttzv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fgxmvezj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2leiblyjo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dtuetkth.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2aorfmqms.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2azflsuts.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2encrgagi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vdleiuik.html


<!-- 参考信息 -->