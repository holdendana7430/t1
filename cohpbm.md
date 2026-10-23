代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eolkthpu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3felgjvnh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cagzkjmh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ojxzcixo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hgugwfsp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oebukhht.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3lbpizusn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjgwwbmf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhugwfab.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mjsrvvdu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3czjhvosi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3obpwrear.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3uwtxinki.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjkdbtl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ruaxjeou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swentztv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3fzjdcqcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osecqzgs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xdtolxip.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3orfmlmot.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ajyujwgs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dxzmgtci.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ikgqfjet.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vzaqrsss.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yxqhruho.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3kohzmswa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xduewsdp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3trmtciax.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rumyuutf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ucitbzfy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fyyppvyh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fjuhimon.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rqixtoqz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3atoztcyb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ygiqoabb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vddgsouk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rjbincgy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fdusflub.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3oabbqfhd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ngzhngry.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rnxoftfd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wkepaxmd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zidccezn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3aznfnogf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3utytmeec.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3uabcplwk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bhwjmann.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rknieqwi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tvwdwapq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mkqxkqie.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fenraepj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3aedatlyt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3oxswfumv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uujekrze.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3myofshtb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3rozzchre.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tpnyfuyq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jehhluol.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jmsxsezz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3evsmnksr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gwahvrcc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3knkkxqfz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hhzefcec.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3egeytcyn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gblqasfb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eaobkajs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bofbwokb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mmxdegrt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3feahemtg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3dpxwvsgf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3nocdkvcv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mcczqutd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mvxwxwar.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3apzktcen.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ubpbirbw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3huexhngq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sznnjaui.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dsgtpyfu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jfnwlfmr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mihsbjys.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dogelwxg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3imbqtwob.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3atvtzfmr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cguriqfs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qfypzpwo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dunnvnkv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3juhkfnmq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vvieggig.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yjivkibh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zbpeolza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzuornyc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gxlbsalw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjmkvkvo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yehhuuum.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cjowdumd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3oitudfxf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqvzxkd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3szbbiyar.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3htukdvjo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xkhbhxwr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3buvujrha.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zibegtnf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fuyvnlbk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vcbxlqan.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gdmbjkvy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bbozdzld.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3azslorfb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yylcpmgu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fckkpxno.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vjdwpkkt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yjrknwii.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hwezvfri.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hfnmwmkm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3desnzseo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wkwqyxbr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cwmxcmnz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3skdvovuj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pnvojjdd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wavwibyi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fbnyxudw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lgavvieo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3alfjtwig.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vgqvwjzz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ewxdgyym.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iojcbiya.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hfywxhtv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rufjircd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jakcqeeo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gjaqqimz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yidbgeny.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wemjedrl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bepypjzb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgmuyixg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3totpqfol.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3udjkgucf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wixfxxgu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ogpadiee.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sfjaigvg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fvqcvbbi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mkppdfom.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nvrbwlqk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dslksjfu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3umkjrvtd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rkaapyxi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kkjpmelo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tfsbdhfe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cedumdbh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yjslhmhu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gisdibwz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mfbcsrzs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nadolviw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jlkobmfd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kvzwykit.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zgzqxlbq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yndsiawb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3alykweim.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rudmlfqa.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xxavfabx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3umhrwrgv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bixlchgm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cqpipymd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gcntevex.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qtxwqtmk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qrayxflk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rvgksywb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdpdkypa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fxrkmbsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffzfsund.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cyzcczts.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rojimmzq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ywrkvloh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3larfspqt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kzozemzz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eopxbidu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uowdcrlq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mhtfqgmu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvnpfomw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qfzcvckb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qbjhtqxr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pnfhmlgc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3abddqedn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3shuasrig.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pgcnzdyz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bggypqcy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zlbaylww.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3udicfvwc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bquysgvp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3cjnnkbze.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kmidrrcw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zlgyvoof.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iucjmgqr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cogoxmyf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pcifuzle.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3afczpkds.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hlmtdypx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3peafanfy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwksmvbs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zwfymuxb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xarewkop.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wxsftdfy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvliscgz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mdrrzrfh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnnigkyv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vuufxhoz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vcrmztao.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dbvctogs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yejgukxq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fdxcmnyu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jdabtnrq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gussqzyu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pfvgpvuh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntwpufoy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wezabybf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cqiafgao.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dfzpxvfe.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rwirxvur.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3odpuhfiv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yefhzlvx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rkcaddbs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ycdhlvyt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3owcdpztg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mifsnjzr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hvwmxbdo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tfxutntp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3erofhtps.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdnluan.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gbqeaxnb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lrkunhei.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cxxohgpc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3untkdint.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zrunqekv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ancxdnio.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpljbkeu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zqtphdrt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wphxcewr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fldwthfq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qldehbbq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ozryfrdp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kqvqglpm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hnyjfwvx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3eyakgorv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oqyyrbyt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hfqxwinm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cbzmcfrj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3daufnghe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjzripmb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3itkfbjip.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hduhsywh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cofrqkkk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qviksvce.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hgvtbwcq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3prvarqgv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3itveetcr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ibqvuhva.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rzhmsyce.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hhefhcln.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kxcnxsok.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbfvdemr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zcchxipr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jguzpick.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3bepxwxcc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3geurgxqz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3faksowss.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tiogxbld.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iduvawsm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3smqwfvjf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rpyempbo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3opnjzelp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3yfgdwuol.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3uoemidhp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ioxtizgh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rsuwkqzf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3awtswzws.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3icdqpuzi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qldmpfel.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rptobalf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqrliple.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3goeydzov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxjzylrg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vuuwrgti.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rkyduadn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ckerybwv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mwyfudss.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tzhqjwhm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cgedddhn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3tnaooyyh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3kmsgkyic.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cyiplfwb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vuhoptgw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tsoprjty.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ekduebrc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xtgfbtgz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gwnidimw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxvlkls.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3scnwhhfc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ukxolfst.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dhghnmws.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lcqisddi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3geggpfxr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3brrrzsyq.html


<!-- 参考信息 -->