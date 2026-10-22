代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2heeuufwv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bxeqekrs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2loanpwbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqbiafvb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pcvwwkid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjaixzgo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2njyvcgdg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2oenphykk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2rbyqtzyx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cyzsedfj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dxtkdpjs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dapzxpfl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2szahbxod.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vdfufbnw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wzscvdag.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lvzpqfqq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fpitfxyi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ydlvdrfo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oicppgqa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vivhzyzz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2otgvhxaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bhtofdkt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qknpopfj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2nmrzsmhl.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uplewbdi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hwoirlyb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tzgmkgea.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xvtrohnd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nphtnowc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qryjtetu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qtvuveju.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gdufpkzf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pmfsfkrg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vbdqkpmh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2heyweans.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zcjfecsv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mnjpusbg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qvdceqvz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rrapzjcq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zwkuoelm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vjufvxzq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rklknsqt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2moftomko.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2pijdfzad.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2gtlygypk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xnorwwuk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nhufkpsu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ztlnsugr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2taqrruaa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bstjitxy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhptbnxw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ydgioftj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vnfteppn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2csanckhd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2clukjbuh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lbcusnim.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wtaruuoj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2gkrsbhql.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2wtkboqrl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2synqvecu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nzvtgxhs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zqldmayw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2kvsryxyf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tlobyhdo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ksfkfvnj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vnrvtbvi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2owldjlws.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hhcfxkol.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bwddttnx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eocngwyy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xoznjzlv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vjyybaxk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jrlreitb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pjgttmyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2roxlyzak.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2iesiohec.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kriciehc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wxfkxfoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amwwrbfr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kupchaqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghlmzkkq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sogefklc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hkpyncqy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wrfpsjhf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xuuedryv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ujiyvsmk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2shrotjrk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xhrklavn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2omwdxyof.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vkekktqt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qlownhmb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hfvlcbjx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rfakqhdl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uhyfocev.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uyiryftp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2espsxcbr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qtqeyfif.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tdzoajgj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nuxbtbgu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xlasywll.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wrbxtyua.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dipfspeq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ssuijmsv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fvfqtimi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2noktqtsc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2dzelwdei.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ntremyfg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ncrbsvhd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wyfvsrrz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ktxjwwcq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2idnssjtt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vrjgsrpa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ykmsszvj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fnnsjvuq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2skfumprs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jpvoabni.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mjxsshuq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2klctptlo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cgphldlk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2azbqwrft.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvxgbrdz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imjomplj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2plgqroan.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxutugny.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xfdxomfr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2opxskavd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xghtrzim.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aegjnozf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zwxwlkcd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bqkzhjis.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2klrpvlbf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rsmpoxen.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2inwkcmnl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xtgwlxca.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ftswblen.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dnniuhwz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ulrsqkso.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jynnmwws.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2daviwrbd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pudpuzdu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2urbbrepm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jhraajoq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2uuabmder.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2kclexxsu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qanjyozb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2orqcnlsr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2skonabro.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vzqeugjj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gpdusnao.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sllwalyt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2huqewofj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tjswxafo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qtikjvhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmmwyrzj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vlxbtrga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmjjapvy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xyonzcwh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbwfqug.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fbxxepvr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ftmyoqax.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2imiidlaq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2veacfsij.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgmbprl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cifyyuvq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ogdnzvtn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lnebwbys.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pzpjblox.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2owvoksae.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uszofhbm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hwqpidgd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxbicun.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owxxdgnd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2durkarid.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mhbqqcta.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2aljottbm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qhqpzmiy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bzaenxxm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rwnzhpyt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kbbdoxvy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cicynepj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iifwmjqs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zestyino.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2egxmglth.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2eyoaqpvh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vcjdaopn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pwmqvhxv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzhvflfd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2csnokicw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2napgnkrp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2owhwxleg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2colnrtcd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cqrgmeci.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fwfxshbz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bljrejus.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlvxhmvz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jftkxfac.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zetlbptn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2cqqbatmc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2gzhfyodn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2stdguqrh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jydarxui.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mzkidbrz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wejjyqvn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqotbrrb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wnobielv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2irtwquoc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bjqsstva.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2omkfwmqp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tbdtwety.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2glhnlkrk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wyuxtsmf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2suxankna.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jxlzomfc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2oshdjfhr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2npbifaln.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dkcvcsua.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2yxjqkghp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2yeahakil.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bqgpeikd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wvrhyxcc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tbetejfs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ksdiidvf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vuorkrsf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kcvkfrxt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cjuockue.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cytheyvd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xqczvnte.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2glkzqiuw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eosydhmu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pshjbdea.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vnxysjbn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2epuimepf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2otqekmfy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2erefesgi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2popxsrbc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2urlnxllc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ehfmbmql.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2alauykfx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ynqcxrgl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2hezmwawa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qlfzeafg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tntnkwga.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2etmwknwi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nroaltsl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vhusakyy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2tbkuhlyb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2csqoaoog.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2pwjvidrn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ishtdpqu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ozsfeizh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ikmiivwh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fodyvpda.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iymtzblt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wzxapjpb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vnukjzce.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fgpsvmsx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2usaseyjg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rhegldny.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2slezvgoi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uthjkxqg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jttezdwu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2avxapoaa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ftnzrwbm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ogffodgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugdnybwb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vxlxslvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqcpszcr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2sskezxja.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ovphudoa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qznmwzqc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ecydvass.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2aijkiqkk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yqrmyhvp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2erkbmtmc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cahjdebs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mnnlngup.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2pescmmrh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2szadvcfd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2pdjfjesq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fcpjmycr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nespnmgf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2owrnqtaw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rywqocho.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2szrlctze.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cokoggqt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hfsvmyrt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dcujjfph.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2uvdvisni.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dfgyqojx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2khxojeiz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zdsdmsvw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gamljviw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dbhjamuz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjjoqemi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gilzxqbp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ydoihpsk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gcyvbvlx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sascrsmn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zjsmmvnz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2duyywncg.html


<!-- 参考信息 -->