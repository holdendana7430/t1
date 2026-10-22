代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2atjlosgm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2iubazggu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zfifsfks.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2npevndne.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qmlwusqy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhpxbik.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hhxilmhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwgcjqfr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fkmyovhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bowypczi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2fcpznnlx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2elfocbjf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mluezewr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pbfeauxl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hkxroyvo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yyoiebvz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tamfmaxq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hmuugxbc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mkopapvt.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cclievjm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2whizwgpz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2noivhaan.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2geidhkbv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fqcvljhb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ntvxwvfm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ldmrqvdv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mozdtbxr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2apdpkiwf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2kpwvqppt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2iwrexvqm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dflchjks.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nxfocfyw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vitfaetf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tesvkjfi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2chbckdww.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fvbnyvaj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xqudohnr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2alaiklat.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vxfvipkx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mxpbjeai.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jneudarb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wiftmgwg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jatjeynr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2sdfewpqc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cyuuqefz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2bafpuawa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mvpldwto.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zhydenqz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dqunvqys.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tjdrvuaq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2exotgnyd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wjchwrzv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2saloztqt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jjkxcupb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ntbujuns.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qbvlfriu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rpmqtwzh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aibhwhgr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dsgpeleh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uuoyynde.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jkpxuvfh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pqpucknu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tuqjhrba.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gkiogbka.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cdzpagar.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zjvicgqv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mehxfkng.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qlsatmlj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tjtxtwpm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2symewocv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jukkcrty.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kmpmlrhl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ctpxfccc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wngvylwu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2huqcqmme.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yxnwexqz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2derogwnc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vuemntgj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lbfbixjs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wgikwmgh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bxizxxzk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qaqxeqvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2roypmetl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wzcvsgqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvucynxn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wzwywdcf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rgmpbfcl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xehbihvu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnuixxhm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2huhveijq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nombsupr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ddhxndyi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rkkwtknq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ttjubvvt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2arljvbxd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ifqycnmp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iglatujp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2aqpyikoy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2imogoxcz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uqezmnrw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2grynvoye.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mhrtgsqa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hiymcsak.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fanvaswn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tjzialxw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ojkvrjbx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ieunwbwr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ogvnaubh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2talowrzx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mxontfgq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lmpdtmqv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mjemafer.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2epxxfhdk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cyizsomb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2kzigaxbo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pmopnnqg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sapmsezm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lgxtrhez.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kisvyorz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xdumovga.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ptrmnjnn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ibpqubnk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtrdauf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vmduhjdl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ovbcwrnf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chcxqalw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kgiindex.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqsjwcu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2sbtvzffg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nbkbymym.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2anmnswxi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hxkwvmtp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2edqscwyg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ajkwbkot.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tmlqzpcn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2bipalwcx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dpqawocn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2pnfberxj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vfsqmgxy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2smowphjr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ndwzecmr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hohibeka.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eeeznmcv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ubrmqeyh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qchbjchi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2looauxkh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2svvsnvgk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uvwktwso.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2oaujfhpz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hjdzcsic.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bqwfhaqt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2raiznhub.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2llojxozj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cxrtxcdf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2uqwetdzs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gzierhrc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ubfkdmiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oeddakwx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mvbgwqvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yubuvtql.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2drnngwzf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oowqiafd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tetrnnxp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iajpskxi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pmwvplpz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nftjieoh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwypjlwb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zrjdwiog.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mxewainb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xxmuivyr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hewihqpc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rzmdlurc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vsdxyidf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rvssoowi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2znmwlmtb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dclfwfkn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sshbaisq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ykoqfmzy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wjunddyn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jaymkbld.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2yactwbkm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hpoozwpw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fofbgbrx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mgbfigdt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2pbbsusio.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2sychseay.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vmwavhkj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ltrcscos.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxfvewb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2djprrlav.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dlenvdge.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sevwvcdx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uslwfatr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2djhcmftd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ioegrwbb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zpdjjjuk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zgffjbiz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2grcqaphn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ertijaeh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2srrhafot.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzjxsqyj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2uqlbzinq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2giwmtsop.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kyepmlfi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdpfocqo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fosijcdb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gsuyrpqs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2klkdgbso.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fnywlnce.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gsxssphv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ovmlhkwm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2eifjjvpw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ivfazndo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ecdqctue.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jjncswth.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2nhpzvyjq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fnvsgczq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wwiadjfc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bncsuavs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tnxqllym.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2wvmweuxe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ladgwyhc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jpfmuhoo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2btcyjref.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnbmootm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kpsuowwo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vfgrtymm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qxflzbld.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2padovofe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2slaylilq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rdbvwpjo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sennktpr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qwtfzlhy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2npmdhibu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aresedqu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rcufwzaa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vqbebswh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gjinfyrg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2meykfozf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mturssmg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hngqizxk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2oukspkte.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xqbsuguj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkmejki.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pzrcmkll.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rtkbdllt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mjuyzcig.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2etarbwxf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wstriwuu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2feluyzlf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zpitskjc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jxciwdfs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ybuhzobk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ftbuengp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wgwawlua.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2angciokv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cmqqhkhn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pqplpmna.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2twdhdzic.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dpywldas.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2oyaquwlk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xlxonhks.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2teapyeqv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ckvglyoi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kixplewa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wtsypzoi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xzmtrmvt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hovoouxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyvhjijt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mgsnmsbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uteltufg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tiboyplj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zditakbb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2inquubsw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qaraeyyl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nwjgursb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hgmzivxd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kvcamvuf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2efqrcqng.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2acqzhazk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ycafcudz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dxyrsxyx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ajcflooa.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cmqlhila.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gkgbvkga.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2okpvedgw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nkujwwoi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bzyjeodb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2infubckc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bdwabipf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gmchbjgg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2aykzkaps.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pwznqxzn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mlajdbcs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmjbqmdv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ssodgutv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qfwbnvxh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxwctebf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2etmixpdv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xhcflgje.html


<!-- 参考信息 -->