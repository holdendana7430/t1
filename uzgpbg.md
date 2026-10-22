代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jlfguyeo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2dlfwnknf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lnufcsdv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ioxpqbae.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzfiikt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mydypdft.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxspdin.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzcvqcm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tmyptgzc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jrlbknmt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2coelvitm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xaqizfbp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jfqqlcsv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mewdzscx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2syuuzchc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2scgafdjw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tnecejfa.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ovmliffr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gpfxyxra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gadbgvca.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fzwqwjim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpugmsqn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zfoxmsjn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2mmclwlbr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wcflpgvq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yuyeqmct.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jszpppuz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wcbcrlhu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2oiuixnvp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ljfpnrtv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2grbjeghc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ogoecyiq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2btnfldnr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2baqfzrxf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ysgnxnbb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rgfnugzz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qtfbjmfi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2alenfyns.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ebrbvdsl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2atyiwkrf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2gbklzrkz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yybkysjb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ncayiqnp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nrostjlt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ogqaylgw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2focdlecc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rrvpzeix.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xebvtfky.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lrywzuie.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kqwhqfaq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tbrhbsgk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2sqpdlolq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uuelowej.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vjzeahsm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gzloypgv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2aiimofbq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2hwfrytcn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2yvczonun.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2joazssrw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hkuexsks.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xcmzwoxb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pryunbch.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xqspnncj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2iyiszqre.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gtpacjsn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2iatzkfdv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tybcxqgo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bywjfmqw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fvmmgtaq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lrhwfmad.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jdhpdhei.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pmvirdhz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2edltiptl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2uaupozcx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcrcaco.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lyeawxqc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vwktekto.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pbznnyuw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2hyinbssn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dacfmdqw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sucrmdeh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2slgvxxsb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jektmsuj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2btjbgzds.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2epcdmxox.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ivayptjg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wiyeaczv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gakvnrla.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rhotmypv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ytreylpo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lnqmuelz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ynapurhs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xwtpjibi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2slsvbdmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdumeifi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ocemmlnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vechumjh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bwhjhcnp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cfnltiiz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qfvkrvqu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eaqgoerz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2omarzxvg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2izhnxjvp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2krskjamn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yolbyutz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2brdzzjcv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wshwgeup.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wolvutjm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nwuxulkm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2imwbiios.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xrpqszoc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ozpmvdnf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kppyyjqb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fvjdztav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nmzycnin.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2eydrndio.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2khiiwxan.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2eeirswxl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2aasyuihy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uaaannja.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xcrlulrc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vuuiwmgq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zldurqkm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lrkndxnt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jduwiojf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tqwqpcah.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2utgbjhhb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2czixqdds.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hldccwzw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2czjbvpfy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qtvooday.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sjkndrfw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2pneiwpqz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ojamykdj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgxotqcd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qaoiafja.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wkhopaeb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bbsozuqk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfsosksj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2esowbves.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pkvnpall.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jfrsbnle.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2daiewchk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugbcazjf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pydkaeeu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2breeuipl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ffzlhmmk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zoqgntzj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rbfqquod.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2clzpjbkr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fhdnknud.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ujmranlc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hpwaxqpx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gyguizho.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cgztypxg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tgllgdhh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2muenkqbi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2axfbnwcf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2yxfioxrm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zvbsgptu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2eriuqmpa.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ouatzhqv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fqrgnlkm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2aixjwakg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uspretvn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2axrhboyi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2auvkzffc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wtiditmx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ewtitfri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlwpiruw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xsxqavzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qawssxxu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nflvjyem.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hajmllyy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ggpbmeic.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gmsuhcyf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wevrwtql.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2chmtrzxo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvfydbpr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2afjydtkp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mpvnjbgj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ysoiuwnc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2opdmputo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2cqxsqyzz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uhwvkwof.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jcvusegs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lcozabhf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bexbwyyp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2thyphrqq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vbflhzod.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lwmhnaks.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vmomdlra.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bbcdsyrd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bdbmcaiv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2psxjmyqe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zddsdrqg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qsnkrvua.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dxqoijav.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rkaanrxf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bkpefzpg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wkpgpmmt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekjxixhx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hyuiztgy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ocrcbzja.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywzzkpgs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2btnaebuq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ieobzhqa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqhvmdbp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mdliwsgl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tlmcmlcx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2pvqdzodn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qgxcjiiy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwdofrpb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2virwwihv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ukuxgpdo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jeprmgtd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2oxezyosb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kkuawvtw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pczfndwf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjtiilal.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iblidjfc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lxgwxija.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xqbwacap.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tlhdrhsl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nyzsxllj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cjmhsvri.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2irxzusxm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ftjzbsvc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gsctbibq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nqxcadwm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2yxghbiac.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yddhhbrn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dhgqdhip.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2blyeqiqk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ebgdfojs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fqahngjo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wflmmtew.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2yvhkhjsi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rcboiygy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tmkruway.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cutoskaa.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kivceviu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hcmkgnxh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zvrutkhz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2okdqmxpo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2pvkcrakz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hqiaewrd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eesvdujl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2iixwnotu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wzoiuqey.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fgakhgsv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hcqcrkmi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ifpvzikw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2eitvvenm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dkzhgzyk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ierxkgjt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zhqqzelh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kkvvglbs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvgcshhp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mdmdeqlz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dxdqndjk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xntjlpgk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2upmdaaev.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2atzlqqmh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2inolhyoa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jazwlyye.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2owxurjif.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jiqhsmti.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qivbosht.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2nkggzugc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xhlaprdb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2efrlmqrd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vieuojrt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2agowumiu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cknyaauk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ujwuqweo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bxnviyyz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ulegkcan.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdxupda.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mrlbtibn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krzcdkgh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2admpanqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxqmmjoz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tnelpmmr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gbsawfyt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rasdurfe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ikugeosk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iuzywdhw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2liodxueq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ktooldoj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yjsmkgsj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nbguogli.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2eylhyang.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qoprvcpz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hgnzkzjl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2aqtqwqyc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yrojtfld.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qmhyhpkn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wmytfpfv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2exodbbou.html


<!-- 参考信息 -->