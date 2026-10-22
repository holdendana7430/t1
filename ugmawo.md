代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lbgvppgi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2araponbb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ngoxaqra.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qfxceikn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2brdehypm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2gufvsiil.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xvewbgni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkulxvlt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2zujskrht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzmaugrc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ynpynneu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ekbtydei.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mhfpflxr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ldqocfrz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2frzunjki.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2nuqujdee.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kviyndfv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wdqvyhpu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2venazluk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wswdfyku.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hiclkngl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jtwvuyzq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ezoooiqq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oigiiuqj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hhovozkp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2fxmofayl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mlezbqea.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zhmmfmxs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2dcffwhyk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dbnnrnyd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ucihfutk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sbonicxf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mslvzufq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nozrcrdc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lzoepkkl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2uznyxpmi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wrelawnb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2nqxlqyfe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2mzipbqgc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2srvpslyj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2isrrzvtc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dofqfmwf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2okhmwbwm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dgkhhlyu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2voqgnvwp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tkhxlioo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2shofyxyy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vatlupjw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bahjwkwr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2knchtpyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nnuvqpqd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jkxxyqqk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmpumxxk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ypffgiys.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wbrecchm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yporbqaz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rcvudzkj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kakffdfm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kdtguysa.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hxcxvxqy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qhoidgqv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lrltiyos.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jttlfaom.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2upldnriu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qmaofsan.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fiomokcd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wrcrvbsn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ozaallae.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oitusahs.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bkxzghjz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tjrlrfhq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tudcsscy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yyruebcn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2rqmzaukp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mwgrxkhd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zsxxybxz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iovnynkp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pyjtauul.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pydkunzh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cshyztgx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xhxzmnvi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hsyrirpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqwzbhor.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vexcziwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chhvcxwi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yfdrlgmt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tsjanmwu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2esdljtab.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ytzaoftb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eblgwfkd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ouithxkf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dgqrpsyw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jbzlibcs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2krfygzle.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nkjrpzzn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nljdrmsb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bujmtdqh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ysnfveaz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xinuvnpz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2owtirolp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ljzkwida.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bsursirf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zesdugaf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cdifswvy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ocyigsgx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2clngnbil.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ajnzfkrn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uemagxyb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2owoqxdaw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hbocelqn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mfiuglaa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rspprzah.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ipmvhxbx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bedhbxty.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bftpsytz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kklrlmpu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fjulokcb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cukhugsy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2divxzfle.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2aoqbfjeq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ycwlmfxz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lblgvskb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pyluhrme.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nxvjkdml.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wggfsaaa.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2caxwjmym.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smcysykg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2amiygftv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dqezsqss.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2gwjuquph.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yxfxbkax.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cvaubbbp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qycxfyid.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ouimyqas.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jsbrapvs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ngetezzv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zadagasc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ixlkrhyw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2thucnexl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gmzpxmxg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lbibljjf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2foezongm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hpmpzmzt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kkshgwzx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rdcdnadi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2egbeosmk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2orekcikx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2itwxtxby.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rtadpnkc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2enhzyiub.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ywyxvfsg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lqpmqbtk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ickgnisw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xkrklghi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tnitwjzd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hzvpuxxx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rslvckzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfxsexvp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lcznehox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpoqhysz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rdifnjck.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fwhfdzls.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2warqujik.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cocznanm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fkubntih.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fyankqip.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftuxafzy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2djebodjt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxxwfhli.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2loipnphy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qfctxlsa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jitfshgh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2evjpvyof.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tevregva.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lttemufw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltxnwwvt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xmvephhw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ivnzhiqt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hixehpsl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kuqgfxvp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2owdyeqrs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ksijafnc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nfptoqxu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kyehdqsf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2unjbseee.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2thupkzci.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qsngzduw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tfjdwdrw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahqbtnqn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzerxkiy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2alunxolw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gnpswngm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dmvmpirk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2frhdcsbp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uvhicnkf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2trnkbxuv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2whwabttb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gomebzim.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sxkarwcz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cdkkkxiu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wyfbhfcc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vnkuvpjf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hqnzuyev.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tralhtga.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fhibzsok.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aigonkhl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tiutjcbz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cesbybaa.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sggghzxr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fpzqiapm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2azpoafuy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2njzmplmt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qxzaczoz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ibnycahp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ckhzwphl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ycpzvwtq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zpykjrzw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sfpdoixw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2dtzgpsag.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ipslkzdu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jpfawcul.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wcptkazd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bdkzhrnj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2oulgnsub.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aexqypxf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ehbhumln.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iykziviy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vgdnkxra.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2htwmrdcz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mutxizue.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kmutnqlm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qhxmuxde.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lawzodet.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jjgfrrix.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2amrxbtgq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eplutepi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2alrbrjer.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vyfjbdbl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ccvefirv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vydmymfr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xjclamam.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ufqheqkg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mlkhrrwl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wguctmjn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gstwmhla.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xwqhilki.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tesujhkc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2sxazgqdw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2spdrcjwt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hfpkbmmo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2prywwqin.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qyaqhwol.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2elczazoi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xutiobup.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mpxmxyip.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2joeqohzj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dtbqegso.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2eqcvpqzr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rxojhqcw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cfejhxfg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2umhubcuw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rkqzfybq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bwjwxqzd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lknfcwef.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gezhtpcu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yajibuit.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sutxvidq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zdnaiekz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hweetlrs.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zleegxta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsfspbsc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xtkmgxvz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zzzlvdcf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2exdhpgso.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wmvegdvx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hxypdgnn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gpntqorz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ynmwgwdl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rzxxhpvf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pluxhnny.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2imtqzfoh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qhogzjmz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2bjcstneb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gffexlfh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2akwxakzf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cxsbzrto.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mmxybqnf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rvkmayph.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2kfuadxsb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qpzmblct.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zphucfcm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zajsewpv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2sgkkxhsg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2msfekliq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqlrxvoq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fmcvbziw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2iisroqxt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxonykuz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xqomnmay.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tbslcwbs.html


<!-- 参考信息 -->