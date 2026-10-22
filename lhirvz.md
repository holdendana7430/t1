代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uyimbqdu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2bocjztio.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pkdhvahw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2jbabvpxh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fpyjdvjc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zxldsxqt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yuulobbl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2amalrlda.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjosqwy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gwphphxp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tavfznfu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2oorbuwed.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rppzowfx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ezcwamnf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nyhjwdwk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2epujxrzu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2kroedyxz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hcuvujtg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dssvabje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbhsbfdr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2aeegmpqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvtymftw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2grovtzbb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lpkzmsmj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gaqtqjjj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rppuevlv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rmayhkxg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2mbuscsac.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ijgvzprp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mctguggy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wokaahck.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sfqthaww.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2foupevcc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fhcoapkd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pgvmsoxx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hlenzxlg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2eggczfvf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2aksbgkhj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cojqesmu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2sdtxvaqd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xxtmtnjk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2unzkzppn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gfvidpgd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ihrbzxdq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hzqgyzgk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zjqplslz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2baxpfewe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vxomzuhe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wbvvaztz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jrfvmhdw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2aqveaxxm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xwzkpzsv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sperjxjs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pvdnmmfo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2waejycdm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kucovlkh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2hoivkofm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dkkifuwg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2chyzbxpl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2verbuftw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2oisorbiu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nqttodkc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wjcikyzn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2mhcrcwlv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2uiscepjd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xfcixhwi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mzbuwkuh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2vkdkiwcv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zpiwxpmv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2aecwspul.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jqutjref.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kmxzukut.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cyororvw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2amzasneg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqhguuj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2credelcg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2svyoynhp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jwsiugbd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lyulbmwi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wtoaeohl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ighmnbkp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2macqpzxx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mpxzyqbq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zadzmcli.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2esfcqmgy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2iciucaox.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pjpuccpo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bpijtqvp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ejsyasvt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vfdvfrix.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dlojfdrl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2txtlwolp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dxotbsst.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qiixukkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wupvisyc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xqzqwxmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dctsjbxw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dmiyinjp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ghyhgaod.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2sbykrnnm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvsvydp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wtegxuff.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2auqmaumw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gwsegijh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vdclbsca.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kmuyjxnq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mwejytuk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eaqvpuip.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wkrxhncw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xbsgjdws.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qzdqepkm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nkpvmyna.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2anzscbjc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pntutkzd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vihxmdew.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2initqfoh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pcpkxjvd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2klptfiis.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fjjbgqjn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zsstmzcn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2iukhxlgb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kwmibzxj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rzgogrhi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wgwarkvb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2fywkteyn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2elavirfe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ithcheqt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iygawmjq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ezavowpg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nnzitvre.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bwgqgwol.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2pbeubeqa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ojtkeeti.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hfxrrfux.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmnkfagg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hqwqdebe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eritubvy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cqzmoxbf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukphqgsq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jmqdvllc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2imirqhtu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wqeyexcy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2veoqxezo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gcxnpyih.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ztjyrwnd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xilcsuiy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nhhovkza.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pqtzvabo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2eswbzmjf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vcfdfzha.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mlmgwewy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kurradot.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xecfriju.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gmsywlkb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rnvgzicd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cvndrzrm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2oxfoxctj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ieltmhwu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ymiopfyc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mdrwteqc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kzpaoduo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tpzhydfh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2drinzpfh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2imnjioqw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gioznsif.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qqbirwww.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qaacvtyb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2iyfrxszr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2cpihynym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqmhhgsg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ccvuvori.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cegbrqog.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lgsbautl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nxryxung.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2makisltz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ubkknweu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fixjuoxv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lbhokbmo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2noaszhvq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2waqfvzth.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nutktxqa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ttaxwkim.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2otvmhyxs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zvpqjhmi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cwiimbry.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2shbtzivd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2linuecch.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ytxxatzs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bleixvjf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bslhsgtt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kqbcgjop.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tfxxrdyd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mkrinopt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2syksmsvv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2spftqooz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pzbwjmxj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2yawqlxec.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kejzakbe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vvvhugzd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2trwysnhn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxcqbdc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cthlfhus.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gtuqkvue.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lzmkfwdu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kariznsu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2upzcnwnk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2truhsdld.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ivusguxj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lavbeweo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmglaxu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2eeqlefxk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifcnmzff.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2feswtvpv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2asrjxsfc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xdjbtfrf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ayyesvqx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ywosqyde.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vjudsdnx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2grvdasru.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2slodujxr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gqxcrlct.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2egarsqou.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rhjwvcta.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xflkigei.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cjnqmqzw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jmuacrcu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fmsyoxuz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2aukhtnjc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mqptpuat.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bvkmjcyd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zxvwcwxh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pkqfrvwn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dwlxdlox.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tpqcpblo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2thfguxde.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kzntlhqj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btenxnfp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tobnppyu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2olxtuvzi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qvkmensf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2khaczlxt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vzokdpin.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yxfjgizm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qrfpkxnc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aethpofl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qjfjtnec.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kqfffsjp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pjiubeou.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lhvuigqx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2grioqcly.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2nldxbezc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xtvkymba.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xyvrjeba.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mpbkniaa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sdbehsrs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rlpdcuvg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ifnbwlqm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yumivptx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojclqsis.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2atzszawr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gdxjlndt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2vgjkpvvm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rkcjufnj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wwzjyits.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lufrcazn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uvjngjnm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yrknfkkz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ihfmykvr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pqkzkdxq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ppkhppde.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kysjnwco.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yowmywqd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mhkkeaol.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jrfigosi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2taybayjt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rbfaujag.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fsgfgnbc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wxytiorz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qtxiavjp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hjkcqsit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkzcmnnd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2yxkkmbog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysgbczdc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ppqnnszr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vyqqrtmv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2abtjtbvo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fbmnswph.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hgpdtbnv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lynhbqch.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lnyiiexw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rdxpknmg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ssbpmtmh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ptgndlto.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rxeryfbb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2aristhqk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pvgtingc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ivfphsqj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zzgqztwm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ulkdjxnn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tojtsfkm.html


<!-- 参考信息 -->