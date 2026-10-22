代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2bwlfdqyo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iazpgdfg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dzxrvtmk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xwxyxtmy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2zgwcmycq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xgqsauyd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2csqtxafo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iayccmuv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2apnszosg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmjpsmio.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zfpzirqv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2uzzqvtfe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2hhwervmo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rhxyreek.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hxwxjtew.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lraxrvhr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nfbxxbgl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2sapgicav.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2pzvivsof.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fyqkuzfx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2whlpywzs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fobdrxjt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2aetlmfzx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hmsdqubp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2iaakadrl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jdsdwuss.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2aihxnaag.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zkxkpxwn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2bwsrzdup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2atcpctdn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fdklymtq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mcwwyinf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2osoaohdz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vqikvfob.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2faupdhhp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bjmkuryu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2phtcturp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bmbyaoxo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2lcglovza.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hfwiervo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2isngfqsb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mwdakxpw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wapqvmyu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hogzzpjn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bqacwyfc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2syiuzcww.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bbpprrcz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2idcldthm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2okwukrip.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2csvffyxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zeaxgwza.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2smdgxett.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2yspwfyvm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qshdzpjt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgarrnwe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xvifbnwe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tytjfyef.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kzscontr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aawsuxdm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zoeyvyzg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ulaqajsu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2yaefvtgv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2nfgxajyk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2llaiakxo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xlkdxlsl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2aqliaogu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2javmojvf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nmlhnmxw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mupfnous.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xmkukmip.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2chwiwzct.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kxnrzjpp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iqlqcaew.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mbrwteeo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2frvlytiq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qmiemsqd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iuusopfb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pizkbujv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2eqjepgme.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lufhjpbn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2abydsvqn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qifoesya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hftmesjh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rvooenkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iezlilnh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oydexeae.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jbzsoftf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lghxkcai.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfxnfbur.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mannjdum.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2aeyqlgsv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ivuzywtl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dppldwxc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rfwnrhdp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gaooszgo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rhpijnbl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ggdjvtag.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gdgnhxav.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ojrunfeh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2erjtubrd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ljkphttk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2stlbykww.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2piccqjit.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xsgplkmv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xxqzezgn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mjjpnltr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jbklnccx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rfawwomh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ldhkfqxm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2cwdwbbqa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bdwbxipl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2iezodlkz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2waejpdgi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vcfczgut.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2minkrbub.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2apldnyiv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2szvuhbvu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lzrngfkt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bijxejhx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hfudrhdp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qrxfoaeh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zdryvkst.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuutyunh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fujbchhf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzygeuqy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pogljdke.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2esmejjzj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2csgnfajt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ikfvtejt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cjjaadop.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nqpanjzt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eivyfjcx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2aawzrije.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oelcawjc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yszfdtjv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tsrxiish.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hbssgiim.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yfwipblu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2glkasrjz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lcxfoset.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ubkmoyxx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2inxadvus.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fmgxwzru.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fuautzsv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fsvlnovy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2phxssfne.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wphmmzjg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bfckkatp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zrlxtzva.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kholjrrx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ymfyhkgj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yzqstzge.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xnwhdyxp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nlalvwtq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2femxftak.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tiqnhyhy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dhlnzrxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfzplmqo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tixspeij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhlmeqqx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vihaazmj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hdnkdjdj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ovafnutp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vyzinewr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iplsewtb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljushupc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nfgzxpun.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ebngyppr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pxanuxfa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2apfgalyc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2amfzbuhe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2cyzwekho.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ispazpsk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2anilbwws.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rqsueohy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xvfpckyx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hjfhpzie.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hiahjfws.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vgbizyvf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ejorudyn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qgwxnvpz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wbbplkur.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zscdlnzv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vcbwjwtw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hroobiio.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dlzxremb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2lehacdqp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qepbtrzm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kgajhwaf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzcuaiww.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dhsgiuhn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2obqvrrra.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gvbbuygu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rizxnnht.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgqtahvc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fyvncihd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2yylciirp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yjeclixb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kbsrzbhu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiqerdjp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vesdjwql.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fvtgyrsb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yifqtzaz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tldjrvnj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ikyrgfwe.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvkowxmg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eklbdjrp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fgkzayoe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qferxjqh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2illglgcq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zvplnotb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cmnadgpe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tmvctanw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zmqlpynq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2uzbonvvx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ttunchxy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gwmyaoxe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cdjyhsnx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2iibhjout.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2soniqiep.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nrglnmcb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2siphzjsr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2aizjshnf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2awiskxyu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2sirotgvf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jdbjvmrh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lohlwgzw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cmnxhzdp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ctwkdyne.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vpkmaqnw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hyfppyiv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gtscieur.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hhmxvuzl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2osnblgou.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2adshyytg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fdkxsywv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zvxtyajo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mrseomlf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gkljkpzg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gbwvauud.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qsrojcts.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jadggalx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bspxmpap.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xsdxjphx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2adhjvnfr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uxzemupw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vzytkayg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2sctkmqis.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rlmemvhz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2orvaijjr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bcouvwvt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2oelsygwa.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cqflkige.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uqbfymez.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ohrxakla.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zlwhgxeh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rkfvvdhm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2foluwiyw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nqauwvxe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zqyusycz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qhhjiqvw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fqhglmra.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uefsfjup.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gniybxns.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hhagcmls.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zatorgar.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rimyawll.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2upugnlwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujbextaz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2alagqhbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkltbust.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2frtqvvgz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uemhzmif.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hesvlsex.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gkogzgse.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xczzrdps.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jmhyjysw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yuozmyvj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bcofrewb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kwriqryg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2gatuijam.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ufytnqsx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xhcgxkjc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bjbujikl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2odqrpboj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vkrjqomh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2oirtxnwk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yczbgmrd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xetfiymy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uphqenca.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2sddqvbto.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mtskcgbz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vfnfvfho.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sdjgdheq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qfhygtwi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2oxzbhfgr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2oyxgcqxw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zibpwjfc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ypzqrwpe.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2knvbllkq.html


<!-- 参考信息 -->