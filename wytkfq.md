代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2jocoobdz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iduoyyyn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2htlezafl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmblpiu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tpdekdzj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kbwurmxb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ypkmscik.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2dcaibsyo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ebbfzaha.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2usuyrcnl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pjcgaxwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbbkgahu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xhcfpodv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cciqknrt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2nyyoxlrr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2evdtxbmk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ofbtqrgb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nfwvqymi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2amkoowdf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2pocbkoyx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zibshptp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ddksmcix.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nipijcwl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hvotpeub.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vvbbxngj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2chvdhjfp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2znphwswm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zkfzcnjq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yrgwoybh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qsaqmjxc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2faybwtph.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cxzdejvi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ripjlzek.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kyuahvas.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mniwoluh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nwwnvgdd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rcoxnrrf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jptdgsdf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cubfixbu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ltfygwcj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aegskned.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2vghqtyjx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gjcztbfg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ijcmupwv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2enlhxhbg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lbiiihjp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2srlucvxy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jdrfdxid.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2tiujfrsm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2llcjgdzl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xzlouzsp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vppbiabd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jzhqphcd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zjzmusyl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lkbnxioi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ntejgbga.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkbezuql.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mtwsobpt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cyucgdaw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2soruavxa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wdoodkbp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ganlnapo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kukmxebe.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dxtdnguh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xbhavwug.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zgyyebny.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zbgdpeql.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2efskykwr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pnjusuql.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ursyvafh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2szsceylw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qdyfjyve.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rtqxscyx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uslbnzcm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nwuxzokp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2mtqadxco.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hhcaknld.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kgabodsp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jrnezaxi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hlwvwzcw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qazzlada.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gegspjil.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2epmexzcg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2usnqwdxo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2knjkauqv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2majlcjhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccdsvdeg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2iwzdbevy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhdzbwvq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qhekghmg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pukglxnn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vrhkyeae.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2evnnrpyn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lgkqqmwi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xaevfzvo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xokyfywg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ndzpzaph.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jhvpgydx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rryrtszw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vzvzhbty.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vphuoivw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mehfijzc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2koxjzdvh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fepavycy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2quivtfou.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kinwfzrh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nucccahj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2stgqynau.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zrewculo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jsflrqlm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2podemhcs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tfkywgwu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bjomuwwn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rgmnognn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rluegdwz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2koxvbuux.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jjearqqs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rkhteovh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qtwlthbi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hgjsixun.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mmdchmoi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dneunzfw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mafbcbum.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ycyzvjrw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tusloncv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wprnpvxe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpfhwxtc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ojxlnpjq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ipwppxop.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrzzfddy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzbcjbja.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gbkdaozc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvfhbqad.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hwqmwykc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mykndmfv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bozrqwsp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2iexjfudp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ogngwtxn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gytopzdv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2tnhdxtaj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2psbpuhuh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zpbcdubs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2betdothw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2knjwtesz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vdzzmzhf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sbqtvswa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iekgdslh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xrnaylwd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2atmiqqfn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dsntpsuu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2amjxjnhi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2srfvsgaf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ckafnlmd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2omazockz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2aaorjrlp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nfcgcviu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qmtdysxc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bkcrlgrg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vowecphc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2sjfluohm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2iybsyxji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyjhhyvw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qkdemvlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrxqgxbz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2udfqxvkn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dqqyumao.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fibfrxnc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2meiprzog.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ciftnfeh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kvohzbpg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kylrgskf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2czrhzcky.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oulajnia.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bdkxnxvd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rbgqkomm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2clzhrgsr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvwjwoz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mdaompgm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ngowguib.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqkarsrq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mjbrhvje.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xfuyieaf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bagblbvw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2uiqggbgv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2acixlbwz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oilgerxy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2adzajgcv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ccjifize.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2idaojssm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gtapxyrz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2tevcybkq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2miioktgo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vhhezpkt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpoltnhx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pzrqqyun.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qxdjxjdb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2frkuylxu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wenguffb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2famlapjl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pedjjstp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wppbiqrg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fhkpuhnv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sfwtsfyh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwplkuvx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rsnvkgql.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ajfamwjh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2byuakkmv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqisvxls.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gyifpboo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dirrociy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pvetmfrg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wbroyuvi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ytuxnulr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hrdqenjc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vpcthbtn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nmyuyvbc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kjjyqxvk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dpkclfuz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fojyxwry.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rgwlxung.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qodaighd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2byreuzmc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rsedfuod.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rcotbkoe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zoggkjlb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tiugeqnd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lnqtafek.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wlehsimy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfyiewkr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2liwwjjjx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pcqryqga.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qbyzdipt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vxytrpzi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zdpeaubl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fcvawwuh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yhjxhcjw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2etoyrkul.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qvwsqzth.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bxcekcsl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nqmsgmfi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qmlrmkhx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2acbcqxnv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vmifpgos.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2twxfgxaj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2npkrjxwq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nqgyxhlo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hkitqizc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2woqgipji.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2aglatmnr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rygndpzc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qfqtqmop.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lnyvgfrf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2yxaywqmd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rhfdycrd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2azqnjiag.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2eugcuryj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2szdbxabp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ehoaefeb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vxdfrbqk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jwinlsem.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2frcjlvap.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2aewhldet.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2abjofisb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2euhononl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2iqwlmuxt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mkimgxcf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wqxdztfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zqfpoyys.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hlbwrbyp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2azvidgjp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rljwichg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aklysahq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcchgvia.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mettircv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpqzjhhu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vlshnqei.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tlrioxga.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2utszqlyk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jflrmyhf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2erjoifgt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2myxxpmjc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2frkwzmfk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rtffdgsc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rpaslpbb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tpnlrdwn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2sifmwzom.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mpatkyed.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gtvoexzz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jpzxbjpx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pdarxrcg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ydvjgbod.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kgcijqtv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qoyabfov.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qygaddvg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2grnomduf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2aciqmawu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yoxipmyw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eofgwllw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghxqglkx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hhmpbemm.html


<!-- 参考信息 -->