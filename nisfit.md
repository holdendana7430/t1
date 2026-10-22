代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2kuldvuwa.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dqsazdre.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nbvimklc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2gxadfdts.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zvqixkut.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wldoudhx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hwovviaf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lxdhzaxq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dcipcupo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2qiqjjffi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pajlapnd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yvoqyfkv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2boobqrcw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2phsudbfc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cwvyjkts.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zjmjoocb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2tixnlteu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xxgbwxxz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lprhhaed.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2knrlijeq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jqmwmnyp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kepqvgak.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vgmlfeed.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2htdoovgf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rldiawyy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jomckaeh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bknavbng.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jqmsqdwq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nltpiggn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iexmxoyt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ctuddeaa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ywqvuqua.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2sdnjczxx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xwioeveq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rdojgrhd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kuhrduvy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pijvzshl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xwkzhmlj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2egenazza.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bahuyxxa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2okftpxrw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fpqguwvg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2akheaboo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2meoqrlpk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2waonbloo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2iykdblwa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fxrqpvgr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bsafncwv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qewainco.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2qypnpgxy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ogfaxadh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xvmjwwuq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ykdrzvtm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2owbtnlkx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vddvdkfo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fdgjkiie.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mfkypfji.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bhpmjbqu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rdezvkhi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bcxzzxmd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hatrgviu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2oowopnki.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rxgloxfd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2airjlqti.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2myajmyng.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2udezpjzj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lvjubcud.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jdxoddcj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2svhcyhhk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rssaeuaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyjseyaw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2illvhpxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgduqcke.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hdizyvzm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fgtwkbpp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pdxlpocx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cgbjkmsb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2njfttlji.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hguuoemd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2yircnkjo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2savlvnkg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mnopxcbi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gcaqwopg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jvxjsave.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xkrcdppr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kcwcxqqj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qwizjzgv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2efwflrwv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wuhwbggl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zjyknyen.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pblyrgcz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vmszzpoj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2urxzcwbv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uvsxcklg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uwxjnzrr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xhukseol.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2txntjyug.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rckbihqp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2csdgletr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zddgwlln.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cnsothhi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2pwfkcidj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lfgobelk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cswibitc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2okglvhyp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rhizlnfs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hyctryiv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jnuabujk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2svprmowf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mwcspmqw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cgdbeatr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2llrhxrsc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2shkpswar.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nggscord.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ktweagdk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rpkkyuex.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bcseuutg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ynyeaiqr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2uejnuwqi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sutymbqu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xpnbnurk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xbeihgwl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pwbroluc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wixohsas.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2blxamzjc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2iqjvorsd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2odhegfqz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2iomstbgh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ywcydpqh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gymczofh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mcjuwvum.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zkoqqoun.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ycrvujpw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xfeqzwto.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ayydalks.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dfqinbae.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mwjrrnwk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2udapxzwk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jfktcqdv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xrgiubyd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2chbwxupu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2sdvwwqqg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2aaxipeol.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fzidbbud.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ictxmlvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icseekcm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bmxxhxxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svxjciwy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rmgoneja.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oqfbmbjv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2msuxazgs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bcqbeokh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xlkityut.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpvtzsr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2udzwghcj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2djoqzcfa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rdldtcyv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lejorkkn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jhnxlxkr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nbnxkgzm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qyppbhxm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhccgix.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rxpuykay.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2togmlehh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mnikvutb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kevhwnej.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2antbbrii.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2prexaugx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2emgogsvi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lacsnflz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tdnlooeg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2eirlylkc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bbdblleb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vvihpkqa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jicpzkvc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2raxnlcny.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nkoxgknd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qisvqzkx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nuktrpjg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rwolfsoh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zqgxueij.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2opdzeekm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zizxmeqa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zlolyqgp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wuggrytu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rwdzzkfn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2azkrupcq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wqutowbn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2irnnhjqw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2owfuxpcv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2itelbhlg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tdvbycur.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2cnteugep.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nhmyowtv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hyihjutt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ajojciqk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xusvxfwl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jcoujvdi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vjrdszuc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2iyasetku.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iymkougj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2iyerzwnz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2repzechm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dmcxenyy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jzcnwxbu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2nxekxpvv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2lflqgxtg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yyhqiabe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ifrenics.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lvakilap.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hqhequuw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sksolngs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zmrokxxz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwridq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2osyxioww.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjpjhycm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wrcgfscp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vaycrewo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2piomxbwb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wwmlvaza.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wrbisvhk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2lwfsmxgb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gpbuuyse.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ujxvjtlh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2rkgzcwkt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nmfyhtwl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wkjrnpee.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oifbpkso.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lkzetppa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wpxgzjup.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kmwqmdsh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2kctwmjid.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uiwwhwut.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ulplcgsa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2prlhypzl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cfnxfbdg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxtfqfq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hepehiae.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nrkfkugp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ywmmohhv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cxquwjbk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fyllquie.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nwwxlkbs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mzdlzshn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jlssrxch.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qobwtgaq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hlvhyrkw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bexijpcv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kymwmsml.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vnlhletc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jykhfeat.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jmtfddzi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xroszfkc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mfkpeipm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ixirqomy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pibdnabc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzxkuyer.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2yxbodfgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srtnwwoo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2zoroaukw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2alxfjrta.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ijiotowd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tlugkeee.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eqdqgryj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bqzzzbrr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2sybazufm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2frtfmifk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2zjyzptic.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fjdcjdpl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ijlxeqkj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2weuzzszf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2anvpdjxo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jarpvzmh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ogpihlis.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qqllalnz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jurgqsnu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2kwbqtatl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lguivzof.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ygjhxroc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gshwivgt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rylhjfld.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fokymdbo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tdynawfd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vfrmlvda.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mljoayzx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngomoaal.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2bbtgrhib.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2advitumi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wxpkginl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2egzvuiia.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qjggicom.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bvrqhdgh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2senrlaym.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jhxmdnco.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2evyidymo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2nkougddz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2enbcqkay.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2oudskjnu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jgunqslr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jheqlwvc.html


<!-- 参考信息 -->