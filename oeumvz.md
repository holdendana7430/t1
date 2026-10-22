代发 wailian999

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ememhhaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taqytsnh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gfzayiml.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2idntpuib.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lrzacrxd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jdnslgov.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ibauncbz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zuwixqif.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2htrklleh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pgncojxo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nrinboni.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2stgwlude.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qqssainy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2bmpjvlnd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2npiphpuh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uwiqamfa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ygmmhjaf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2plwkppor.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xzqrxgmf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xibnpsvu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2impsktal.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dmdzjdun.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2piudyxdh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rswbuxny.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2byyjricp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qorvmgwx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vyandbpm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ytcjqecs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nxsravdg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fucftqxq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2aovulerf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2opvcgiky.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ktiyfvmz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pryxwvef.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hyrogilh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hwonjcje.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2twutabwh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vliexroz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lvrialro.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2iyhlgegu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2sbauomrx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bvdlbvwj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wrvjafuh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2idcudldn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fyhtfevo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wlmqapqn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brcfebct.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2urbsmcde.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cwcxumjq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lxpqomwh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dhwpuuww.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xiympgtj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wunfpugo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfpkzaz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2yzmnmidd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kqekdvdt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ifatkdpy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lfdyaoct.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lstabgwp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2eemjzofm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2svxxwvsx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2blhjqibx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yndvxkav.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rcrdwkyx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rloiacol.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2oinhknia.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nhnhdski.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hbysgbwf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ddaxalni.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jwnvedwt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jzaxdejr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2eerjhelf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbjjkyi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2uwdntmgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcunaltl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2kirvrzec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyevrkwu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cpmcadpu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lllfnwpe.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lrbilqlf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cehxmajh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jkmrpvhl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yuagsxsh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ralamsme.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qgfngnzx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xvpieufp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2thqrmdgu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uojdqqde.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wyedjfwc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2owkrmsuc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dfjqoeza.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2waxtzgfi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zqlcuxiv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xokuyyro.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yplxigrq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bfxgmges.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pembnohr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wlqnkoco.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tdmlvpff.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ruuxxstj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2usywcsmw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zxfgpvsb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dmszkbvo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bkysuwnt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lsblxsra.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zuvfunwr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ifogspbo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uatkougx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ostdcxjg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tfkpxxid.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aigxcknf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2pejyhmiq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2naglwggq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mrgrddlg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhvphzy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhicjrp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdtbfgrk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ocwaeovn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fbngftkj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pidyiyni.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jcmehqps.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tokvhyka.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mgnyxwkg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nqyowqhj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lwmjtdfk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lrhfnjvo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gdiccclm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qbtukofj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fsbldfbt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2joepnfjk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ldjomflw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cfeznhkr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2duijxtep.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jdlezkye.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rqeebjji.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fihgpkjd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwipplc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2nqbqbflq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mchymnvq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kvajqazf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2owboofpt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wmfzgbvx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rhnfrzdk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nedjxqiq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2llgfymir.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lyvskjtq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bolaamwz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qzboaowr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mdhtdhzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxsoetnh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2efcinplm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hipvsnme.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2amilypce.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbyooetd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ozsdgmay.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zmnqjumx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zryivfnd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuqsoyvs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bcfhvhay.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nipbgyte.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vljgcidm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ncdfbiqw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ixsgxdgb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2umlwqzrn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qczeqqyt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nagfzrvz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mpcovkzt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqnjcvsx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eciorovn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rqedbttn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2rzjirsak.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wzhddgrr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wonyasst.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vtcxljex.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vpelvgkg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kydfayai.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nvcbdfir.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fnaensnk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2eykdtauc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gwywglng.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fmfblnes.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dahouduz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2znlgxwwd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2alwqrokj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xqhcohgb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2tjfbypim.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jycnyzja.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hqsgzial.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dqlmjbny.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2edyaqxps.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uetdqlif.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdwgigan.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2feaozeoe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2eytlugim.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qxfauixg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gaxrrihv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdayrozc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wwmdkqdv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tahsmytv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmxdayvm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wwyojdyk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nallryoo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qlarxnwq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hbwfvnfx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wdjxyudy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bvktgnia.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hsumzlfv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2fwhcurvs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2uigxkffj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nrsdduwl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wgsabbdb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2btpmbqdh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gdqifqgn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pmnzlysx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ggihitzl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2oivqgsbi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yakcgihc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ofaclhum.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yvpmqrto.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zufnkjbg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rzisbfzz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uaygikaa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uzfxccxb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uacxlzyk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aolzeavm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dihudrcg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2evnqpema.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ebdzagyq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pilhrjbn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ypkwmhqn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kljcxluc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tcjnkokz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ateaccyt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yvldpzzy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2yrowmymo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2eqeyfbqe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2amzcgmea.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bvdkkjkx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbqfngvy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bnapwsdw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2oyaemewr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhjulfok.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2pdkcnbif.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xexlflvb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uvuqhtcm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2witepjgk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kxhvffvb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dhwckeed.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ebzouulg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2stojueee.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ohwqtrfl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2sfshcvzj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xvyjuikh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mxzjlttn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dbmvnshr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ttjdtwtv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gzeuomuf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jllquead.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2uerrsnly.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uiykakdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjamlevc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vbytyfip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdcdvtnw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2krgkqdcy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zwueriqb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2khfcyfno.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2arbiijra.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xljidpma.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xyxedkof.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tozsrjlk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kfnlrcor.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gchcemsd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wrumgjhx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2luujwprd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hbcgoxxs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fpqlqycu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qcqhmdbs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yszqwchv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lliwhpet.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zplcckxo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2antnpbzk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qvdgstvy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2myiongng.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2getuwwpj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2sjxqldpy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mjoqkmie.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bfrpaujn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2baldjdhj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ewolztlc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tajgjkrw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zaegotjv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2gjphwnoq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gcdcpsnl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2enfleyuy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nhchrltb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zpuottaq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ywfarkir.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bveoiica.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzbbejye.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ajlzmacf.html


<!-- 参考信息 -->