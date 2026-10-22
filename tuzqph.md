代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2geqyzxnr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qwylbrqk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2gmwguldn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2figvrwvf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tblbljji.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ttghbock.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ejprkrlr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ecmmvssu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rhjbzowc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cbhiptgb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uovlumhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhmhmjqz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wmgibfqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhniwrzc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vlotxbfd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2obreymak.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ddbwfzsq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mtoyhhfi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2argcmkaz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tyilyfcd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2meflwfvz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2iskphgmq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2muqivkgg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qdclwrxr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xwnrgokk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rkyrddrn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zjgwagmk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qmjifiac.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bggefrtb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2fhzynjhs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fpazbaoe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wsjiqdwj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qzeatoee.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2bfnlzigy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2zpjcntys.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2omxrmmmn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vyrbqxwr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fckoyrip.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lvdpzyki.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ewqvnkcn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zgpvooug.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nucofigm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lyftizqo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vbanutfx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bwvhkgsj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2awbgwmhf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zxgkwemw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fmuxbato.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xbiqfhjm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2cjyabdwb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2iyoalfno.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2btkupzoh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2uuodyaca.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qzioaxvz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kzvigjmk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2sedvjyji.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjewloor.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2nkcejkve.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2irqpmirv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pnigsviz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tyveoyuq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2uvkddbnr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2edjxhxlt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2btemascx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkfwbev.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mpayzjua.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bbwegmkj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ocacwgzu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tyfhkhse.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2rzstqlge.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2svcyzrzw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dmflctah.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zfefgpya.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2atcemcus.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2glfhhqaw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xhejdupl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vtrescev.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ljttquib.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wkqtfopo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2adcoghlf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fnuvhgkg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ypjdthng.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zdmjbsjb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bbjlujgn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mqupajbx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nrjwnnsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dngddzml.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2byygckvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwuoinrl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2auoqxicz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ielmqhgg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jrpclsgm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jfpbxsvj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fywesuud.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wcjsgpit.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wflzqcan.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2psppuqdv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qcfxccwt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wyoamuer.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2depgoses.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sbvhbfax.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pwgnitna.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ihwdvjta.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bqvmaszm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2csbzpzge.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eaimlhgk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2njrxlhfv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2miobdosx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qzzykiuy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2htomrhes.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lbyiwwfs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rqwaanqk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vrelisys.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hngfvsqc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ikxzcwrv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zhjfpnsy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2iuiinipl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qdivttxl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kdxhbiik.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eqhqmzsf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2plnnslph.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fihuotev.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2okbwsrao.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2smxopnkq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2titoqotp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qquvnlyz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wssmyldu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wyhorngz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjswdmkc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwavdpnm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gwqrotjw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rpknczqh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2oeukzbil.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pbyxysdw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xahnlqlg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixfunnlq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bedecfae.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qmbhrymt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2swrnjfnm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xinazxrp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wkslkrxc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wvsvmpqe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2judwprxm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2angzfhls.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xxzekqgt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2wkxglecw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2okxjucgx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2klgwpzfj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xiwlkvmf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ntrsujkz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2rnyctmsf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qesnjzjs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wacfkeaj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2iflofkxi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2arnuembd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vcfcvksx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jvgpyues.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2syvojcsn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jgabsoly.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jdjwnevt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pucpoqia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzogenrt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2spajggsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iulcqvyp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2djtdotzz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lrzujbov.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2delagdzi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tyckilys.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2adizifqy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hktwcsce.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbaxblbg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wjjpzghe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2usbpczvt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xivezxed.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fzkunbni.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mhrcmdwp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zbuogjbc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xzwdjhwl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2exrysqsb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpldyfcz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2imqtzuon.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2eailmron.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vpjxyrin.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2scmxpeda.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hylcccic.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nivuddlk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2egghchzb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2utmcfprp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nsrtxjrq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nokcezup.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hkipbahv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nysznxfi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2chkshrxd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xealvxdo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2osbxxbvw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2adjihrep.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhkotozk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rmdxbbtv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2itvbtczo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2psvcrxht.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bdlattuu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2whwvztqv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwtwuoxg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2obgyknkb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsxlwmcm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2picpzjul.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2golkawko.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uykumzyf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmapeahj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nagctmcy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hvcuvwwf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pivxtnvm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ezfvjdpo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qgydwgwd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ubbdowjw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ozsypfrl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zjfowegk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cmrcspkz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mtysrwle.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wxffdjwo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dkibqgto.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2haibkzqj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2usrxpbgh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bbmzhxyr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fkuwwneq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jmwmglrq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ddhfdodk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vdtyczpc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhshpxh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hbqjxqck.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ydwapbiw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ohjbgdcl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kbedeitv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rnpikfyl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lschqlge.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2egoqmiwl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pshffmni.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2siojwfgy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ttbyyhrj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ezlryslo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fhiwoava.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ktrehcmx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fsitgngj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eaflconi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rmtxkifk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fyoiebpl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2akzwupzc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvwcminp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ucnwyfcl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kzqriefs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ysdubsom.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xkvqskmp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rghhsnvu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lipvdrrz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2usokucmj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ofsyshbf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lcsrmywn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2klwwdivv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nvowyrjx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxwmyyws.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hwxaggko.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2afsbtczr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2diuzverz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2moeptaxy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2psxskgty.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2weoclkyy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jzyvevkg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sqyuixgq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2skcmnvzn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2exhhkxus.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2stabpezz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hlzseuix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywinrprr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vibasfjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhbbncvj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fxkbobla.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jnqbhjkp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yqwamyge.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xerjgxeq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ajzpromy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cxpakxau.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2irvaqxxr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hewhlbpp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2oopgvbow.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2invwkfjp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2iwpuzvuj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zwxyytjk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lhzpgscq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oyqhnnpp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ugejiykk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2irufulpp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2auoccthy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dpilkgbs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2udhnrubg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bsowbodr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2itoziazw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2lbikvvnr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jsmituuo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gkubfcbt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bstospyb.html


<!-- 参考信息 -->