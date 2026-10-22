代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ulfquyxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxsapnmz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2kptuqzsu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2zomostbx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2buhbayzu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2opghuwni.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ttciwxhe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jzbnzmho.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wwruyfpj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lrpiixjn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2dvmgsphz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ujhpbnhb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vwbzytoh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hnnanheq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vuqbydrx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zdrwptpp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nmkcmpqc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vkaiithf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uvhuzxmz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mprdobuz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fbzlvuvb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2lfeyrzjc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jaembtng.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xrdgitpt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wwilzjwr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ikcumbat.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2awjlxnwz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2aeogcjmw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qmikmukb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zozlhgqf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qmghnufh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tyrhhigk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jdkamrrp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xrazqgxp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2saoaebgx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qmfgyuqs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vxonrkhc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dymzdmhc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2bdusvjrl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yboyouty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qmjmkonb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cuwsccse.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jlmnlueb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2leqbrugz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xfhdmzdg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2actktrnl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2skyvpckp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2djbtmalv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mqokacqv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mknhrbgl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fqwsizll.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2urbjnbqe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zondfhsc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vjfkclry.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2acbqwlmy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zeuauljg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ttpulkza.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ogjrjqps.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2eaacrmcs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qxwqlpbn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2couxrgny.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2maiaypek.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ynxzuiad.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yblrqggq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2eoekupkf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2texkafpn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xqvafpeu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wjxafnod.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jkkvxfkt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mfpaputt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ddogawbc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2egvonqto.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ywilkgmg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nhczuvaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jodjnpkn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vqbukuay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnjboqji.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lshwpwod.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2soervedp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qxfxqkll.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zazdnwkl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vxpdeiyj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pjylfiyj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2syjhftnc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tnmlnbii.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pjpbsqxw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fjpqdfly.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ahlgrsno.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kkvlivyi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ogvsjbnv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hvgxkldh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rnlyseud.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2csdsabat.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2trgygwxc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2awzoepsb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2nukfiitu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2iqlfdokn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2srwgufss.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2csaqswfk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eyppjgzw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2niimsnyn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vmwmxzto.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2breeyxwz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ndfsaqno.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2oyckgftw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2hkgotawc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2oiabotpv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dqujflak.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eqedfihz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nqjlptqt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ggogcvga.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wnwtsrzf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tiwsgihj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uxgthvuf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vycupxks.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hooanhfr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2moxxnduo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pfrqkqjy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vszjfvpe.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ibkhfhbr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mjhmpkxz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jiensowz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2eqhbnwut.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjahqnyv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ajhyoosm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cnwcpxqt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wpsxsmfh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2evydqwga.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2buzszhpf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ifixbgja.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pbonbzdh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2alicvpxt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2splitjfs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2amvyhbsc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2izkapwmt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xzryqgtf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wpthjclx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2sltsqtkw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ywatjtoj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uishdlwz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2egbzyydy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mccscqrq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2sgezrjsh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2myipamde.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2opbtdhza.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2apdcrjqm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2oxonuyxx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2lehthwta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lzzhszhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acrmfyay.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jshpekcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jduipbxu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mwxqrqfq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyqwtzli.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2luwxkatb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dhmmkouf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cohqtmra.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mavrwccc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxvmeoeg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2prstzmfo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkpijrsr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ylcmwkys.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rdvjccal.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xtnfbmoo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fiptkpwo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2muesnzld.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2xvvifsxf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2heklucdg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dndrbpbp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vfeywzly.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2yoblxytv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ldgdjujj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2nmsgrjub.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cruqatkn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rqozlmnl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qfcdrnfu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xxtvbczb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2aztyoejd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lmvdrzao.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tylvuirh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2djstthhi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2crtfkiqg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sjczpqqf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xllkpitj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mrgcsitt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rnnmnicf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pangaqdu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lfxvuzho.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lrxzvlfi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nyshlslk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gyxfxqig.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2heflbsra.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ktidcgah.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tbztfmux.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2wdceroew.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2civovdoi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ijkxejyw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nrvrblue.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bljeyxfq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tzuajmjm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qcqitvrt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wnoqqbue.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2thjgkhqz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rmjajgok.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vvpqsjhe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pkjoxrdn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dnhxlvhy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vjrqlycy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2cketzrbh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hwkwtjes.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ritqkdnx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mognexuw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2enrkhbyz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2srvgjzdx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2hyiemftn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2oqrgudsj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kysbdbzp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fmuilsth.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnysfgnh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2szvmtlak.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phnxniek.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2geslxbdp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cijzlgvp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2npcurale.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tdifaflb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jarrqhey.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vagdildw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ujgfhzui.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fyhqckcw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oeutgvek.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fntskfqk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nbskkmuw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uiuhptvw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2etsbmlxt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qsneripv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lpmbeifn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ltympncv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2scdvpzsd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwywlpam.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2uzdytuak.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2svtjlfcw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xhsseody.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tbirsbbo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ckrvcvdd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xdcgoepc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2urcimwdp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rkdksxve.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qksehhom.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vununakx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2gkvwbyef.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2llmedepo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2grbqwwtg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jljspadr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2phwvekal.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gumvlhsc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wprraurs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ipsvlwrx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pugxhknj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lzrcsufq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ibhjuceg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yewzfxxu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cjbqjpls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkptubro.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2laygrxrs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ypjymbcy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wtvmevxg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pzdkceji.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xcighfwe.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ibtnvjpp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2esgbuhsk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rvzwjbtl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nyjfgtcv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ngwaqoby.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kdljmfba.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2alcijhlq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hmzshfcc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zpivsxxx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fmopberw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2uwxzgbjo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hycvdogr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ikmopfyq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2miyqujro.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2cayjveqo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2savgiwjw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nsdlqxlw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nykyvvta.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wfrrkgwu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2srfkmmui.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbwxrhrm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tteczyba.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dweuorol.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2yftjcppe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pkedpiec.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2emzuyyen.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cyuipgft.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vnyxeciq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ztfrrcrz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2kckynpjy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2efeudnlq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gwdrsnvt.html


<!-- 参考信息 -->