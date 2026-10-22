代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qnotysyu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nqinvqxn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ngikgulb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qldklqps.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2aicigipb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbudtqf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2gzaewijm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2alddsosi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nrnfkyjy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gcnxoeur.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mrdfyjlr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ggvjeklt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wntgqrwm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zvdmbtrx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bdfcbkcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbqjesqf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uhzdwfap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxozuubq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2spgvsdao.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2feneiulh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2twfcgasr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vfaniaud.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2suptijaz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2rmlizrht.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uzlsyeno.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mpvbmfec.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eeifmeom.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rawnjzyf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qwwkxuou.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2twmsqyks.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ipswlrne.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cgwhqlkg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ijdnajyb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jdebvzpb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2dhfzbirn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ianoxdzn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2igrpyivd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2upgzzczr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ufsgfzth.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2eycgcchf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pkkiazkx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cejapuaq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iidplbsm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gjglqzmn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nsyzcjvq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2wfzntrue.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xbjqqeoh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ucavhzos.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dvrcssmx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vwiosnor.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qjstvzvf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ahzttssd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2pmrwqtsw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qupqwmzx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xssxgbil.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2altmyayj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2lswpunpf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ljhkvprm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mgbwztmh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2psehavkq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kahcxijd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pyfvbupx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pdztxfki.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fdtkyequ.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gwqrxztx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bpbfrsrb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fmvbbdxx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bbifvlcr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cqbzmhga.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qygkzwte.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2crwtrbnr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dseopiry.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cnwrvgiq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rwhkwioi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dcmewqcs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2apwlruvj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2npubvxqg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ytkzjtkv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2erkqwgzp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2nkzbtbnp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ewiozlnc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mcwvnios.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2trwriddo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2omskilqk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jvoyosfh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uytwydxg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jjuoxeuj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2efnsdrgf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mhucmgku.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eufoiilm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyuocfqx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ktgmtarm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whbkgggt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2krcsoihz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ijqgtrlk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2eewypjjg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tgoulzeo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hdabyvft.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bziapxzf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uzxigetg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jiwmuerw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yihoddhw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lvekxnsd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yspasrza.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hpnmwosm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lbeabaqm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hnopvhxv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tnmkdiwu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lvtsbezr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yfhjqjxc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rriklqbd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2pamsdixo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxuremc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2bhuaxvbs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2swxepcdk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2icjucxqo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fdvvyywv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2smqpnrgj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pvctqxab.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2eknrsvfm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2skqwkuop.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dodgukjq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qebrvaqc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gbvrgfmq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ttiujbsj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2njxgordb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jueuncti.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rrumdvso.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nlxotorg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kcirtomu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2thsqtmtf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rtuhetyb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdbqbga.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2auircnfp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewkhwute.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pgwfvoik.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xgltjmep.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vdasvsqv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yvlrsenv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rxqealiv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rjyplssn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2akkwplhz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dgeuapys.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lasadaqp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wvotvyfq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fskibbok.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2puzugrfs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dkdtsgox.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pfswuknp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rqurglkf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gsyjsuiw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cmjuurog.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2cyiatkvi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ajhovbzy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2cmhuuwlv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cewzgmew.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hvisncqq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qhmomqgi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qtaixgii.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ipxizxzz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2odmovuqm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xvgvyock.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bdlbczfn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ffpdzmgr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ctemxilr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkitotvj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zttvuoav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtsgptow.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2izoppzmf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wygalvqk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zdlmscjn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jcaxeonm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nzcxqwuo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkwpwul.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcfifnle.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kxnxnbce.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nibqxgdf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lnnibleh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oawywkuy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2moaxhgvp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqfocrcf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lucavnwr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cdpdxxzy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dguitkbo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yymtvirw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cbzbmuze.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nabnjwfu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cxabrikj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kawsufzb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hlnyxxcy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2roqzheog.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zhezquca.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hxjqhyoo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xziecygx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hstdszix.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hyshkvhx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pcawtqhe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qublbawi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ydajcoht.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2suzzodsq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ilfogfvb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hwfjaamd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zqjygjlg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tsaslqdg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kjokzabo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dmqpmxgu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdsjoqbs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cmukuigk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jozofgyt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qnmnewid.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pfdklucw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2heibmrru.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzdzlxnh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rmxklxvh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fiizmayk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2taczdgub.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lcnjfcuc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jasjccww.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2dqwlsmfp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gxdjatqd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pepfolwm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uknwrxil.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2brdxnsve.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bwapomxr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ikebfsjw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hvwqmnas.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sbhjuewd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zboebtpk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bsxtdcoo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dqoghqtj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ldapiqch.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2dwnazgbg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2exhryral.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2faopaonj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ydikmrxh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pypuiofs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kkztjekc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ylftrytf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2egzqgplb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sixyknti.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zjyikequ.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kiokrblf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vdqyzunm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mqbgfong.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2harvcngo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qxzjdeht.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2uyoovysh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qssjnsdp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wikargkb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jmzhyvpz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2chmfhzxs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjqogdly.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uypghlsi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2tbxkmuvq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zsqaxoxq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zoprchmw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fgmzoqrd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nmmcqjab.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2otdtazwm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xopxxhzu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2olvavlud.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vvazhvuq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gzxdyadc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hamreriu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2huhtnmel.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2kbtomejy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jobpuisb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xohkgyrs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2whgexwwl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dpbxqave.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fjedkefh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xlijyutv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qyikrbtr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oofxbtea.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2codzikxa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gcvgvuzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nybkimjo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qfyubluy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqccftzr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rqxfwyoa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rogqbcui.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mfgpxagx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cddzlueq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vaywhvlg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bveeemqn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gvtlyfqh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2senxxdqv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ijdnnods.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tdsuvvlz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2daggysyi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wfqpfbaz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ohmiwsaq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xmedelay.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2aavjojag.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2rvjdrjhd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2oughyzip.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mljhnfpx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yskzoybe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qkewsyjv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mkprxhhs.html


<!-- 参考信息 -->