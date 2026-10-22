代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2kyvqdvca.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qhgzpjlh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2kdkhhfeu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2abutienb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2znkwctfo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yjvefrao.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qmbvsfve.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hduqzaug.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2hnnrsrod.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nojzupmd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2arihssvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsdzqvhs.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fsylveug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2meyukvid.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hrhargez.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jaxnqlgm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2renwwmou.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tabopoqq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwupqcz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2uisjpwmm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hbefybcv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2kfshmcgr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ropxmtkx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bxmywfzj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ibxchnfs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ubtzcnjg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2owmzxmhx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ucoccjyn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lyvvkcoo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2owimmhbf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xqixpfjp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2siztzhod.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qogfyhub.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xuibxklo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hwthroaa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rkltdfph.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2apogbasi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cexpyqzo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2sizhmdrg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ndbtdvsj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zqyiqwad.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2nyozkyua.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2obsrbrue.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pocgefki.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yczproxm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dvclwuow.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ijjqjcnu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2yyyvfwus.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2smfjdwnt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vmzeelan.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2kgziqshc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2iciglguz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ygwsettz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uboucrut.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xygiakes.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ivjyjigk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rqlxwefq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qvqxlhaf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iptzlxpv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aamyokws.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fxmjqror.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2etrkltwu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2athavxxh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cdvvfnpd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tmpwbnel.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ruuqsqay.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ocfklpxg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2eomunzrs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2svwwpira.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pvmrqspc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rgvnkqmk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2psgvqkny.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qibpwfrg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2smgffebe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hxbfczpa.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kmjtdhrx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vxlokvgn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fsjdylsf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nbhdvgmt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tdqomccu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lsezpafx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2crqrpgbc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xtyzquhp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2iwvpcgcl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bavgefkt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vliabovy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhhflchg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2imocpijy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbcbybdl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdbcoeag.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xmxvgmot.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mdgnwqny.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqjqlpmb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccximbcy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2anovtqri.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fgjlndrl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wskwrhib.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ivfjbrrw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ibhhwqcp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2olirmtiu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uzzcluwx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cztzbeht.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hpkawbfx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ltfocbsk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2plckdxgl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2woppfrsu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qotsdznr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xkzygvsi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2svmbcutg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yyzilccw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ciaijygu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dacrmion.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2copepeey.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ttajhvbq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2sxkkvoon.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2nmxeqbbp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2teygfcoj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jzhapdca.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pobrcumc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kknyixlm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bfidnlnd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2omadtkjj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hghjxpxc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2drgjlfnz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fsvmuhjx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kdagbecr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmttoove.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uybvehez.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dycffsks.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bbhkzsqu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2afmwgnma.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hcijrixn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2swhpcqwv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ilykblxc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pypnwrog.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2aqdjiclh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2udwtjjbh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jdawgvgr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tbgkxysz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eerhnrcr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gahynlgu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hmkvvuud.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wgppsrux.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lccklmpq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2exzsyoug.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fcfwaauu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mdwyimyg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jjmzlqwr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qbvwtxiv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rlaxhgna.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ehcexljp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rjxvtfsy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ypatddnq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ttiqxrjp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lkugdaqe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rbhqiwhv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rxhpsvbz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mkrjavks.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pjhjdbfo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hcxvgiiu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bbbrmtcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfqccptw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tuxaakct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbcizzpr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2smcgaobt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2azttujof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vgrytyin.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yfldhqna.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gdcukhab.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hrennege.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ruyswcja.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2upgfznkm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gartbahz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2cdgddqmk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cdlzgvea.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bbwdisgk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gsotghdd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hdkcmwrr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ojbgkktg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wroatcka.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fczqlnci.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zgmmjiba.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2fkvmtadh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ctckfbnb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tpftpxdl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kwmaplpa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mlokedok.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2swcbclnb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uexbgxai.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gwwcgbnn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rurlesuv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ktxnrzhb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgcrlefx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2thpcivim.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tekurlgd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2powcnziz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vgblkwgp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2akjeyzfi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2veqduvww.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2njzctcgl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dajbvjbl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yxglkxyv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdeapjvl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwrvyyex.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2otzscxlk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lshvsdbm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hwazfioz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vxlvcjky.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mmqibxwu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hiobovmg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2anipcbef.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mowbkkce.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2przfikvd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xlafnwrq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vxbwjdwm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vnlcyepe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hsfmvaus.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xdutctdg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2vcudupgp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kfealnnv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dogchpvp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2natagjjk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2azlwqton.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wpvucrpz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vwitnpvn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2yypafwwu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2daokasti.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ddirkxhf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwcewnho.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jonhutsl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qvhtnpgs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zfntvuja.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2laowyvqp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rfzpxbwq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eozqmtca.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ubpgeuho.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jvgorzcm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fwwltsgj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aofhhsfg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oyiuqqrz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gzdhtqrm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ppqqrvqn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kdwfgdmo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pmqkrxsc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ldntycnr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2sixrzkbs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jhejalbb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaqavrek.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rzmoodog.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2yshnirqd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2aimyoavv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2eqmjpqsc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wnzssipa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gkydodag.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2semekpnh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2irpvnnos.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkwzpvmk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kpjuofej.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2afrxkzrt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yvqgxrhz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vhryuhyw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lmvflnpr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ippnboqj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gxroqcqi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fpajsbmn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wypawzgw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fgxbvzfe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2olxbxvjm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cnyzzqsn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2szblqkuq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2dglzruqa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2shjajxuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugkehtff.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2amtxblff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjqajocg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lpiweihd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2avlyqmcf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wdvohlwq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ryrmmbqv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vsjmnzsz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kmxfjadw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rdhksgcw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qnjhiatx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dwpgotwj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jmujdkhr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zsemetyz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tzjrgnhj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cpdktghg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uoulsgrj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2obmqgkfp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2faeszcpo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2eqdylpzo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xcvfshul.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pdzvvogc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2poyskttl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zudzuzdp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vfbsqact.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fuutbbfj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukllvhup.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ceefohoh.html


<!-- 参考信息 -->