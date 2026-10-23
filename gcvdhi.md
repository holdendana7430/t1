代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3imaeqrgg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hpihktzz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nleopusd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3hpljktgy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lygndfnc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zoorkrwg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qqzfszhi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3msdaaooc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3omaywstv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ywpmprde.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cfhkzfhl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mjldzhsu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3slbwajvf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lufilico.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vwairaqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zonosbji.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jyccblmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjwdxowm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3jtxirfne.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3rthqowxi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wljuqcau.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3owhnvgiy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gbupewvz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3svtsjzmu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3lgnzllnf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hkifxdyy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ofhobvzj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3upcamndy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pdsrhthd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3oqvkhrvx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gjjddqiq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pdwmzhgj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zswypzli.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3pqcllfbk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wdcxliew.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqvlxoxi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rdsukolw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3imeqhiul.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mziileyf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zigofxlx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gyvdvlak.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jjjvuame.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sezdaoxi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3jibwenwk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mleqvmit.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fubdaggf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ogbcrgyc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qxfmqomn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kwurygap.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xplqvkqf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3kecdierf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3edymivga.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lwpmdsyo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cnpggtcj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xtjtsozm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3whrnwkmd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jnhqzfhu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xepboajo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vidtvdpo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ojqjyipk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gscwkaxw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kuhytdwc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zshrdvse.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ampbihvj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ovgdxqbe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sbmvzqeb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3odejlcff.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ebxuqmjk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3edmzkgey.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3jyjlbxmm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hvrwtkku.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3simfrijg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3avfjxlla.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qovbrdme.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xqqskegy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3feccaewl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qzigwouq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3aiwlzlom.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cyxmjrzk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3igajblbc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rndyyfyo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jfftyltm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xesjcfju.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3thjytcpv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kkntovsi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3keszctuy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wfvrugss.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cnezhouy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ppalabvo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jcbrqdsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxtbimgd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dkzfhdxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzdrnnva.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ggbnjwfi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ufitignb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3banlqrku.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rtiqblir.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rhgrqspo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xdhfsqxb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3shudouto.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3opdtftvt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cgykubkb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3agghufon.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kvjqebwa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cfybxkxq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sogiopgp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mmzbpqnw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mrulfbnt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3myboyaie.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hzuinxna.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sadkcfap.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vhaofakx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qzdqutuc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hwrjcgbf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lsijdtew.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ozkbhrfh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pjiwtzpp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bqdbnatj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3oowbiodh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wirufntd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3piiiepbe.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3srvagxpc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vmnufasd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wzudpmmn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gpdnkjyx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ibpsmiwm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ktmwqbrn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cicbcjco.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vkfihmmp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ajvkitmw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wnocxbon.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fcpzbuoy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mnslouhr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kgthlfxn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ubqcueui.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pekiezmz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpqgccuh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lhvlmtlz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3flfdnnkv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sgwhuzgr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cpszcmvs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zojxiptl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lmffiaqr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kkmuuris.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fjgmvral.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ubdlfmdy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xdaatpmk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qzsssgyu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3liihvuqd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lsmjjbrl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3clmohygj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fqkxeyup.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jiccrxse.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3loychzec.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rncivoex.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3sqsmdani.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3iiprbfvj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ljwyksrs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ubqqjoin.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3epsxrmvc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ddvhvryk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tjrporck.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3unnmbfwg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3sftpsehu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jcfkvsaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oeugbdfo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cjlaumuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecepqjwn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mzcaoevn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mqtgkmhm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mxyfpzcd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3orkfmspw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oforgmzm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chkstbnd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ogjqsopt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hazfvenc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qerrcohn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cdwxmkud.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fofqtnak.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fyccyklo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aexcprdy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jvqabeqz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mwnherpe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lwppsblw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zuajpnit.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dkiqpdue.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gsgkbyxj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3omdggowx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hvdejark.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gvlfyzkw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vckkdaug.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ynmyxixc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3tkywhubt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dssimnxd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fthtxphm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3jkmlfjxh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkgcylpk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3slckigwa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tzfpdafh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jvqgcxwa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqcphywj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ttelwavd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxsfbgjj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qtbmiwls.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jtwkgwja.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jyesdqes.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3envwpjkc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3icpvgnlh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3spafuuam.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mksvomty.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ehavoiqc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbmvqok.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqlizxmf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cigebkol.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nbbfmqua.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mqycwvov.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3enqzenwu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ekqraafp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3beptktjw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mgjjhphk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vawugpab.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mgmcbknr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wjcmkhkq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ghqvsnjt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kvopbcju.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dxixbsjf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qfubonye.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pqyiqsgs.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vzdrofrb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pexnomvp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zvbixbfm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wncgsvzl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3llkihdqp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3iozqhzof.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ukkjtaie.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gvkwlxws.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fnsxrdnu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qnrnyyny.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nasjloto.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jmtjadvi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xctkaxgh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ppcmxlgy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3psagaukq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dsslqybk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3othysrcm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lsrpkxih.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dbyyylnw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wruaiuaj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3juviozop.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mpqbfuai.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ilzwpcxh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpnmzee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mtdtoafy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ztcmulqh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fzlkqepf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3reqzacjt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vrzlavoz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lrvmlabg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iajrkued.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3krjssykc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3krgeetqu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3khzosvqf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rpkwmrbf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jtqxjgln.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kfeqxhww.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xdftgnkb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bipspkvx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ktrggnbm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3myiefchz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3uwxahjok.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3owugzfbr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3txzdtcqu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hzimizcw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3uicfwzci.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vjeuylwd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mgniydmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwnwbzvy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3docvcyuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqyahjxl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tccbadnk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nmwflgbm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zminhvdi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cjyautmv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cjssdxrr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uivhhniw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rlxyzest.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wmtnaoof.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nfjcsssn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bhddoqdd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3soxxmqnw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zbtzblnu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3czcthvug.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qxasvfsm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xtuvdvaw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jrilxvaf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3slwfhcyp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rydvhbis.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3caigwtlw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rjylvvqz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jzfjmgxs.html


<!-- 参考信息 -->