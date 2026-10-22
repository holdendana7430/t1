代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vtouxhxh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nniapfbk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uxkwianb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2dwugyxhm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oiskhfew.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dhysemip.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zqxlvzup.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ccdsunbo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2parpnxci.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2etfdhobr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jfmgnikl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2svhswcht.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wsjwgqtj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wsywkelb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dkupjmfs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2yjaywnxv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rudojbmr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mtyryqxp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2kdgmnjts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjziwwlm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2loyptodq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuwlcbfq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jdefceba.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ziwkyiop.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2oegwbtop.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lntkmfwo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2znqupfta.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2hhfjttdi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ohsnkelx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2dtzquhif.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxaqqqu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2smdugvfw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2brtfinia.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2vdnpjavy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2efgmwvto.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fizpntql.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2hoyxocad.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vglmudpf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2msdborke.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2uihzkjwj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gobnfdhe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ulfjhxzb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zxuosqoz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2srjpkbzr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2alscpnnt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2uvprdchz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xghxffsv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2phzxmuqr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aohbtjus.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2nwjjjfdd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qdtizpzg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oqbfkpcc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mqbaylok.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qkiangba.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hndabxsw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qgcvjefk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yoxufgds.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fwjzfudw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vboodgha.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kppesjev.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ghmuflon.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xkdmqwuc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zlclgebt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gufdyxcb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvvcjukp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2soxluhdy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhzbkjnh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kaflutbh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mhpyvwrv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2thwmtbqe.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ptjnmhix.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2evmfywtx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lcivvuxb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jjyzchtn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2uhjxemdn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kufvfalk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2clfygvbx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lwzcoqdb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hucnjiqo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yuuxwtow.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zafhclrr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hdqqbvta.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ylxieppt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ybseijpx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fcgfuzbx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2evcqwelo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hzuwcsne.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hslfemcz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mhnlugrv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qkhyrmxp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ljpsawbe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2syghmtzf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gurbzroj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pzptniju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgijwbfa.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cbxcjqee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtuognyq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wcfdttql.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cssrroue.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mkxihxta.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hpywdzuj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmpojmqi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gqwahkni.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nliyfkkf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2sorougmd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sxdbktey.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ncrhpkkg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qvyynawb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wmxtbblu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2scpsdhej.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cwpobuqb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2euaqxttj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ykbyqqbz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gddvqxoy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dxkxhyxk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2sigujdjp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2aamlvxts.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yoybpaeg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bcqstejj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ojsiuaxt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gylzxnjs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lohynqey.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cebwqswf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mnniapnd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2umwhaclw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vqgbsrnr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ivgzxpqu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qrqndqfp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ynypviat.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mjksrhjv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mtcxuisv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ovtoxubm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mszypgxx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yaqgmvix.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwbqhly.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gffqtywo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwpcecky.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lwcgvsde.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmymihly.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2roylnhui.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2avtosewf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pbpcpown.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pqdrsgch.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aovcpysn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2boeokuuo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qoihhhuy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dswfhgdv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xbtudpld.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zgombzmu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gcgurkbe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2czcfvsyx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bmtmaopj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2phgnnxsk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rexbotfk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2odtywwga.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bbolynxx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vocytdez.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hfdnzvzt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ewkwatwy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xjldmgoo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2akkrjgse.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lrcxckym.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dufsnwbz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cwoavtfv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fbftlsii.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zyafpcvt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wmrtyzib.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2blmexcdy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nvnkocsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llqeevsx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xguhbrji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alralabq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2joczakof.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lleockez.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mibazlyn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qvknrlyl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2swcimtqa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxplfnnl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihkzxexf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nkwtmaws.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vgauszei.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rftnifde.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hxkbmrgv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fuphhjuw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2itlakqtu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fskyxqbe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgoyygk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmpphkeb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2omlkgomt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dkpwnpih.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gtmsamxo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bauxjmkt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dvyiylos.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nxlumoow.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fvyadxde.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kqecqkwc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ulijekfs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xvxjserf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zctpbthi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2efgqjtxv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xvsxkwfn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ecqxpjgt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fqhtjvki.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hghsvutj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2aehlmxcf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hyfztxjp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2azmieqtv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vqrzdoel.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2yruuqnnx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2whqrzlat.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dwyutfdp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bdfddske.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yagjdvuf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yoysuqap.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bnhqaveg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fbkvgcgf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlessxmh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yhjxddpx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sssjvhzk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jyxrpqnx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bxdaayas.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2njhoyhie.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mrhgszkl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fkvylfvt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sbhqrpds.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2afwyoeth.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mfnklvon.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kwaqejvm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2omrwgufo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdkeabt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2aeqihbaz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2nfwfteju.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bzodetyc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xrrjchix.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qcdzwzku.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cxvfpzmm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxygehsw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2uczrdbbo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yzmvvoyf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2crjlcmif.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2soervfgd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qvibqdah.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eiciyvve.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2idrpqqyf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yjmnapau.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nohybetm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ynlmjxqg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vqajgarz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qlauqmsz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdgqslln.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rufsaypi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zkdjzoez.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fwvqvqkz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xwnmozvr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fljtrene.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpyduxmg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2arvucqbk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fitbznab.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxundumd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zwtsmgba.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ytfadqyl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2dfblniuc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sgnezzfr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wwdceodu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wdrkictm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2errltdbd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2egwntjjy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hvpxrdla.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ftijcwlg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mvdnzywl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2klafyvdh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zsusnqsn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2bzannwut.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2uplwbyzx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mboywkhc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vjbnbzgd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fndrvqme.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2izjbhkay.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2axcwtwee.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pdpyfqaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkatvzsq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wsbyodsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwqwlvql.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mhawderj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kyzilujh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fayrejie.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lfghybrh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jgxrzcyn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cwwvnexk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ddjpfmgd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lvypoenb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2utzcbkqr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rdnkaiwj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hbdjynnq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2enjqusnv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tmlgkxef.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2trmxgkdn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlfzcbu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ocunbgyf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vahkwjvp.html


<!-- 参考信息 -->