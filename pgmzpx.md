代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yzhduxwf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vssizlgs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3aphzdeur.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3njrvnkie.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dcoobwvu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lubetuua.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3spgrloqt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3cstxukas.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vxfqezdi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bquxtatm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3poceyuaj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vfssjzqe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3suhkavwt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dqkmviex.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3euudtiho.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cmlioawy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3pyjpeiwk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gnzjjxjw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dwwdgfam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cycyxigj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zllksase.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygyykugg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pvplwrtw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3aqkdjxfo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3qshvtkyr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oxaxfmky.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3goavwkcy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xudtlhae.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xamsuxzk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3uexpbbfc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oajmlnll.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ytevvabd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mhktoere.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3llunbvld.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3priifxar.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wtdydvsq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yzparvfe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3yqxbwkqj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3usgofbix.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3higenush.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3xypmegyy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3xxkayzjs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nolxxqjs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3giyhkrbn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bqqpoczk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vsrztfaz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dlrwqlsu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3mklyawod.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zqzhmgkg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pkbrdftl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3rydcwyhw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sxyuoyjz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eyaxxyxn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3euxdoetw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xapqnrqx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qfdoyovd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qttpuesk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wcwbcidk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xlgdpjcz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kyjhtiir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wfjywtuq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3crpnatjm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dvubzbix.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vmgsehiz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlvhsfdz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rlpucbic.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3obcpkqfp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bhalurax.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3urfgctqy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gmybhqou.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uzdhyhkk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kevtwlko.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pkvoqkou.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rewgjwoc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mslvnbbz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eclovhys.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gswxiygw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jmwkqdxp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3khehanwb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fdjbhhvl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3oezyspxd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3isxpzrza.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hldspysj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ohtnxzfb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hjacduou.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3praczqzs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dosgbyqa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xqydvufj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3azxwbiim.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qfkryfgm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xjarfhby.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gfzsptno.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pjkmnhqb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iwhvgaak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urhlfomd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ugfwheyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcghfrho.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3svnwsnie.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oyvbusnj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tyradpve.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nouayarm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3roohodko.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lcktetur.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3tiwuedgk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pjehoksu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rxeleyzz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvxhzvkn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tzefbatt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xvfottxy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gnvwtbew.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3llwxzfyl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fkufiiqj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wcooyidl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pvrnujhx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zehwldua.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jtwuwfyk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3espwjnbj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3eqvbxafs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wmdgrfjj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kiithkde.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3brofupeh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jixshoty.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3yobslxpx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3awsumwuc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dyfzinaf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ruezmcqw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dnunwhfv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kizroykr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kozhquzm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rviczrdi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pnthhkxm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xklvqubx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rdarsqps.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3uogyerwa.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqzvkuhg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ofqzvlna.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hnhmnmnw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtujwtw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqutqxz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gcwboaik.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xkpilfsr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3trjxujsf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3knxcogla.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgldpvs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3suhqnwff.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hhkrmsmu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3puqianuj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qgmzpqap.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zkepisak.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kzqfgzrq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iylpzhon.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3blpdvbbb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nknbodgm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wnxowrlt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ccwbuzzx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3frskchsu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3iszpkbpm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wbkgzzeh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nsmgdoxm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ftfqnfod.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mttshgok.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3sufzjhxc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qpldjkhy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3juelhkka.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qljxxyrj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3cofgfbne.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uwfirbwv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ncffoghl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3htgpslbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zizbisft.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bebqujrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brmiefjd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ulwcsvwe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vndlmzsq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kgsvoskt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3htfmjrtz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zdydhfri.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sakyveyt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wepuevps.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fcnetmbq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywmacwmg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3oizyxbir.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mayqjynn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ksdnywzv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwyxcrz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ixjjuqmb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wizvmujk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzojhzub.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nhatmqgx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dyulaenl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3babfxazi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dfodeizp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rudoeafp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tkbvmtgw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nrgszgpl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ehycsryr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xqzvjzyu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3axktlxnq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3yceqvbno.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3llrioyam.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ysvowfoq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvqcxcmk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sfayeiya.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pzptromf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhlqullh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ptkixflg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mejajzvc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dvpkhjwp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nvlkmciq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nflkznqx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fxokvhdc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrsiumra.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsxzksnq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mmpjnimb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bxgsdewq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hantxtwb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ordlgmur.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ogckdety.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3txblwzek.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kzmegzpy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tlggwpkh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fqsmowor.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xasieovl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bqvhernu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ljxmjkpg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nrjqixta.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ucptigex.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3knykpxkj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tzekqzbu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3oloxycbq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xeioaerf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qzlezalt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3erhantfv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pajknscq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rxglivze.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3orrtdagr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oehgzebn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zppoioxk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ndzdpqei.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkfgcjzc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mtqpywpj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qotqibmz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vhcfmnuv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aeqivotf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3afedmrpi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jiazipjc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ztdnzuho.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fgfntpng.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tgaozvmm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kgseqgyr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wutlqmov.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xyhykdec.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ucadarff.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yymnrqlf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3rkhqonhm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fsmszkyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rvnkujyu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yynqrzba.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ggzwpxjp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rbnfmild.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jiqaylew.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaqilkoj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lvmtauaf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3euqbfnjd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3amxzsdow.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wamyldcy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gzibrewo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dsaxvxpr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3olvfpcam.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lesifgov.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hgbxkgby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rqrogjkt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jyiowudr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tflowukm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dlzttajd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nzonppco.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uiygytdv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3sfblcjph.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kkzbnkgx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hjexyytq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyanxbwb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3moygkhpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvamwtag.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rzsqpnpe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uhzeebfi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3irzjosvl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cakfhhft.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3irfjdxjb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3exkerige.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ejwtqwub.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3oubgqntl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3axzaagiv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3keedpckc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncnvsexj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bgpvkyyg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oryfttte.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3skkujyyq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rgmxskkx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3giepjmop.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3asvacbiz.html


<!-- 参考信息 -->