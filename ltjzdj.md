代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2irtmhkle.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zoooxvfz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rlymtajn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ttjpbjoi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mkkqxusc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2helteepl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2shphkjqt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vkfwdbku.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jauhdypx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cbnnowfu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ytellrcq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ukawzdzd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2lirdypgs.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2xfzymrma.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rdrnqqeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfnbzwar.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vvgjvazk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrgseazs.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2kmjfsphr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2chxwbrwy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lxbklyye.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pbegqatp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wazkhkgt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tslvbegp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pvkkohxw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jwucqdzx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2yqbmjkoj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wnfbumwi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jgogvtwz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2suwohjnl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2runjgdhz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2edbnvhgw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qejtpkbw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qpthbnbe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bblgoalr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2uunplwok.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2gzomzguk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2uozddvlb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rbsssinz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jceycbfj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gbuftnxo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2bjmgkizr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gmpwcguv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2iphxzeng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qoywadii.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2yedwmngf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2mrwnquib.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yiiitwrr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gqbetddm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kurwnqwj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vauwujwr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jkdbicjo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wokbhfzx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bigquzxt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2okxojvlk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hwgvhopp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rduncdwl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rococdun.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gmzxqsni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ckvkygts.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kzuvojik.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ntemjslw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bigfrbfn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2freznpxo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gcoclwwz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nqaniyln.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nwyfwkrf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vysfnbuh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xbqtvkuj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nilvmkaw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gjlvmfca.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2fmrkeubt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2puxolbzs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qzqrmmpn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uqenofrh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2inzfmjnz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2csevbgil.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fatztijb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2towvuaxs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cudatxib.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gfciwyci.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gsjuqvbx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2knjnflft.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ybgnclvn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cvshlpbl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2osdzqqhq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2cysndyaj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kazpdfwg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2duijolhd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wremwpyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzwqaplq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mlojwewq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2retruxrs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dbcxuohs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2npbanetr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2eaciedcs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmxfvlpl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ggnvreda.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qvwbnmzt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2erihacgj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xlulnipa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jkfjaujz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2untzwemh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vvlhbmpf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nkvvpwsa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2axrctpvz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pjivgrzs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pzpxjauf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kstkeaob.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2mbolzgly.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gcxwbjih.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cpdxugee.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hurmaofz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vhbuicyt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2iczgubgr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fcgqaqsp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nrvpsnil.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xbbhdcmw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gyvirrbo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2patmprgc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zfbxnxgm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2btirroic.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ehwldkvd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rxnxfbdw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rsjtfhmh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kkgtjiyd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjzuwarm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mjbimrfe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qgngnvxv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2skzlxqcr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuthsyya.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ztfjabny.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqbbidic.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2szukeeoy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tgcqjmcj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bplbnafu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tutkmmjm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2oruymilx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cjuguqyd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yanqxjgx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2btgqradq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bvnmbltl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pwlmikfd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iqduwzbp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jzjuducz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2oamddope.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2aozmtssl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gezyvlst.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2yglsuwkc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2eumipjhb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rgwpkkyb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cbdzsltf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jbupoicu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tnduzdsk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zmotzuim.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nyphkepp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xykuypud.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ajjklzim.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rtxqqutr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dbzgwsgs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zerfpacl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2unhdeozx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ftqvbkby.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dycumaum.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yxnqjush.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybvsvgxo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kvdovmmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqtjubli.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xoilawiq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2odzjbxcw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ywapwuyg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2klqncvae.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2asaxqhrq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kculemnl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2teavdrag.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cdlfddlu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fftzdxgv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bldrlilt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vhvbemxu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2begzxeye.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwjgkbzq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hoyuifqp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dyimcicn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lywwmcln.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ifukvcek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2juevhjjb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gcwdihrg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jkhmpoli.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wwzzepzy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2biwysepn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nvxadtnw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ukxhanud.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2okixrpdx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uatuwfxv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vkumlxzj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kvitdkhq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqkopqgh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2buyontst.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wtphuaiy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2egagiamx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfxikomy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2uemnsyof.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2miavxhkx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ewubmbub.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gnimgbrt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rgksxcoq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2krzqwvkz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uijtkjcq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2onftnmsq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ztgodeyu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vbooczig.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wvldjvcr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybzjhrgv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwuoknlx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2shahnjrf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xqxhxgiz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lcuelwbd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bpupjezj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jrfaheil.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cjgbihjv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lfxefire.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ebzfxuwc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2syuxdcjb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gvobczht.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2junctvtv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2codfcbyo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wwimyrjj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xjhlulpb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2yjhormjl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2moelgbpr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tdlxykrl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zxpnsiys.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnccrwgf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lhpvqmqp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jmfjwxra.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ssxxadhj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xjkwnrda.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lthgpsdt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kbrrjfqx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ysbinarr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yezzbujs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xkbrdohk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hkhbqosp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tdfcunab.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xswwufla.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2orqgmege.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pqdnuhis.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dlhvduaw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ddbtqwtc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2aqdpcesu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kpyokpcf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzyvuiyc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sobgxqxs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wogcgxzn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ophpqzma.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qltkqnsa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2eibzfflf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2elauydit.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2csctueuq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yzghvccl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dpndywtr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qxlwylng.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vvfqagme.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qcljnjgy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qtutudmx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2dxgtrnrb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jnsqcruf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xkvnwnbr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oythherb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zdwxxmia.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zamkikfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rzgpuzuj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2olrwncmm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vrlhwwcd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vvebdxnn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2amtrzbcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oupkpelc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xejudlor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyuazduu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cjwhkycq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qriyzxqg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2gejhmklu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qflfhzow.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qojycvlh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cqtifxbs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kfpqzqzw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wlsytdzm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2fcwudriq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mhyajbpl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2yoocjbbq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ewnsmzyu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2phiepfve.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2amntocyl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rbfloxyd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vguphfar.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uxfhucyg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ywfubpkt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2xpyqwoqv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cogefbzb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2arwrzvkq.html


<!-- 参考信息 -->