代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3euxiorwe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gwqgsktl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3tbmxodjo.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3iuqodqrq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3llnjozzt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bkezxkvg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3suzwwywk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3kuuvkvoi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gwjqmkpu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mlmwuvss.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3epyxcnyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hegoynhr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3syrzbmzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulhqcckd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3oxvcndjt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3inknrqxf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3nixrvjrc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eccguaky.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qeuzfmxm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zueqwtxf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ynqxcxdx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3hgkxmiiw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vaskrgaw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ufaxxkus.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ackpoxai.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ijvwofbp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zgxlxxwa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sswsyiic.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3aaytiyku.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ndyjkqje.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qpwwhreu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gtmgqzsi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3avtsteju.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kuaxiuif.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3okmmfuhf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rnwakkvd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gyeaufsl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xxkqbshe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3krpazbsa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qutppyzd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ziymlmxj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hqwioexl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwairjz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cvhvsmiu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cngcpscv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xylicaud.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3knzmrbqw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3uvfzumuv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3uftebpbr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cbynygtw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ryjnkjkd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3inftkhao.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kpryezvr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ueyefsal.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wybpsvtp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fswodyih.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kyecsmcd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xdaqmnzn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oumzvoap.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sfzfeune.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hmhkhtiu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rlcammqn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qbwzingu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iysqnoky.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gamnfvdj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gjiqidgg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxrzvkv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3velfrlqk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fbjfyewz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gtxjwaqm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gbjbthbn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3byywydps.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nccjvdbd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3iautrrgt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ifoauqfn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zchpknzq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mzfbhull.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3igbvotkm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jiwodtpa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3yxezxito.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nrsarhmu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fzddltng.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3aztomoqw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fdjwwiir.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3phsfrbdp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3icutkkyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrwifbsf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mjpmessv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqeiydol.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tlrosbus.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ixyayecy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3schglyxj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fsajzhzi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lzvzlort.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jfztrhfg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xphfpepp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3empzdayi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pqdjcwnz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hhmrdvqy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dmjtmdun.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jygedpgp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nwmmhxsh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3aqqjoswj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pmazivis.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eflkvlur.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ufyjanzz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mbnrzcjr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rgsinqad.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xgodyzpd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3izqjzrra.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uruhnqgh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tuqmnfxg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hfolinka.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qholnsjb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3endejdem.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3czapzzqc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wkjrunjt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dmrlsrqe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3avljqclh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yniefwdk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hvvevgfb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3eishkifx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pahtjhqw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fliavjcm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ubgbclfy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hmtloqrn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxiiiokp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ywkrbpic.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3prmzpike.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktsvuqqj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dznpmpde.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3luubaecy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fiezzxgr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ekqljvsb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3krzejwft.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ntlovban.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tfinwisk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3feaewqpm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nawwrzyv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3noyxobfo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ukxywzuc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bqoqnxtt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cntvsopt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ikczhjcp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dyeustnh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zqemirks.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zeszwinx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tpywxaca.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dqpsgpgz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xwhphscj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nagtiofs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3udwrcpac.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wdhbylyi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ojvcjmrk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lnahjsuq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qfvlpwcv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iytoumrw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jhpjyhch.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jvvivkdm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xjfvvplx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ixviikld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glcotfnn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mlfhjsnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esrkoctx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3htjegdlw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtfrbvny.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fkmzpdgz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mkodzdsx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3llpudmfw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3opxitjdj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhoddbxt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3grpgfcup.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qszhiqht.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3seitscov.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ptzubixm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vwbmgqfa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uziqqisd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgrqyhsv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3scbbalvn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3msaenovn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3chryficz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ptncbtcd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yxomlkuh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yosozedb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3flaglnjw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hsdyjmcd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zmjzmiya.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xzzafrdz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dzlgjtow.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ngzausjf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qtylzfmr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dmtdlhpc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jkkipaog.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtwmpxih.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glxbdwyf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ntvcydze.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihbrmgmu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xgibcyxq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3aftsxhub.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mwzrlfvf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3bfasfbff.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ygzhrecu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3olyqxkuk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gatfsijr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rmoowsuy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hqxkskku.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3excmbdds.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3txssvhkh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xloejzih.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgxgvvao.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qxyuyrqa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akqqglyo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qldnbflf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3owqkjpvx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ektttofh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rpmqrrlu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yhfjwuat.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kqkrlvks.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3znkqzvlq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xtzmkznn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3odvanjgo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kyekorfm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ghisxdvq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mwzrzsjx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ooepuibs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3odpnxyja.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wnlbffdi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xusxmroh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jdqbsgou.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dpfqghzn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bhhntshu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zxxnbwfv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ckvetqxm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cphhialt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zrxxwegi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3temeziha.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3snxscvgq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gjukagys.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ofujweer.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hzltdepo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3levqgmyx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3orcfceeb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hsosgtyz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nfihwhxp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hmxmdxks.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sqaxluig.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xnlawqws.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3elaqjzsl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3amikixic.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3egerabnp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yyaqkhbl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hklsbkhh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3omykfmco.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fvrjnaiq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3oryvrrza.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3twkitqks.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qwgwivfc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gmtqpqhs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3htolzuln.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3itqpfkkk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zwyzcdkx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dtdzkjvk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zhudcpjw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lhmqpqfv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qrqqxdnc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cffyzxfy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rdoqteyw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3akvpxpqz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kmoaddeh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rnwjrgwo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tgpdpiua.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xxpdufwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ciykfzdf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3tqoyhgus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsfnvtst.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zzddvldf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pdurvukk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3umazrkli.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cutncmrc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tmczmqnd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qyvmheua.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dxjhsjqr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xlxrtikv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wkvgubxs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gzrgqbfr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vzcvnkto.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ayoinnbq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3farovlnr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wdeibptk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3crxiexgs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3sbekunfh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ajcsobeb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3aemsoycu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bhhsxrwi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fcpkluab.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xcmphpkp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3dsmnmqyl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xeubfvvu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fknkqctt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jontbafj.html


<!-- 参考信息 -->