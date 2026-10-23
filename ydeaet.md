代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jtikljgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkarpsad.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3kdgffsca.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3lbwpaxwy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3nvrdgxxf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3beljeonb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qxlafnxr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3jdgsqtui.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vfbhmdyi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gnnxvtgk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3xsdufwtn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uxegdobi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3owlnqluq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3vzgqatjv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3sirrhyeg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3maonkouy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3klnqrugc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3poxuklmp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mvowpjxo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3uaqkwkbi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3xaerbdko.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3volnjnjo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3obqxzejl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wynnuyld.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ehhdjaeu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3inevhaio.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mqxcxfca.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pmeybgqi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3shrdamun.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wtfdilxp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3oocznivp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hvsmlhnd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qjauwgva.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3baoirxgv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3evfottab.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fltwadtr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3liphvzpj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3uquezvkc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3sirgeuke.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cqmtxlyb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rsbpwixb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wnatsvkg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fmgxwrkl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3regnltmg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3njyerwmm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zizjwpyt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nnfikiyc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3zsjbomxa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wrmjaamx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3efaabazx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lzwgsbju.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ogjibqje.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hziwxrgl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3obsmgofh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wplhtpsl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cmibnxdr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3whfpzfyk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ulalwfjc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rgeywwkk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kwwqporm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lgqtptsy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dnpraaxl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vhwwnkfs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qapncaxi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xvpktsmr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vazhtkxt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3wycxskcy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bvsssatl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tmxzogow.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3orrtmxbv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qvbwvakk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3halpyvvi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aduzorxl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ponilrxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibdazaci.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qbxapdjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsuxxznr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bbqjqfik.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dqusmymc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ltbicwnj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxunulk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3sjqspucw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pnqzreog.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tuddceml.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dzxsjkrz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dlulnngg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cizyqnch.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3spenwgzs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3whdtyfgt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3igwjvzma.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ylipbgsz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tyolocam.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zilyqtjd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nsqdfvuj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lgglilnj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sqqrpgku.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3maikfxrm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nmgrqmld.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3igjgzetq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jndzpmli.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3arwzezer.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3okbsxjnl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3swedycjq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fefbkuke.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ssoejnxa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3healgadk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ghwvanag.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3adsoiamn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3egbotced.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3eoqxvhvf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fynqnqlg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yabfmygj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3snxaauni.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3eumxfjia.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlauptff.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ynetwvcu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lblwwngp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3etkouqkl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3epujdtbf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecnhkbrm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3iaqqemwr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ayfyzccg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rqtzkscu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fykfpthu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3izosuuvn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hxmllctd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xuodohwt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gvrcpdyq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dqyqqxiz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mclcjppv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eymmbslk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uwaosxea.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fvevxuwz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dtbcscoq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tueaehqw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pwmnwvtx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hxllyxga.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zoyyflxk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ppyfvhzd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3inqjqznx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rgnrqdtx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bnjhnrxg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gvsatqnc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ouidtgma.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nwypgrso.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kiozmfhf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3feqvcrwu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lihcgpve.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3lfblyuee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtlconge.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3etnjvjyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fujvpwww.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3vscpmkxw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmlxugud.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fqrepfcw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qbvvxidq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uhcmtdid.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwguorbc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pouksmzu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mruwslxm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3upisyxqa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rzkgvyox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rqiqnqag.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3huwoznvk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xtjejyan.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3boidimgz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3slshectr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvmubsn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3puxqfkdb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3viibvspk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3poektlvd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kyxmorsp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lbwvusuo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qmwhqcmm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vkaazpnb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3szewzesb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tvizzuha.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kofwnspz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3thvrxeyc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wtxdoofe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtzabra.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kdxmgzvx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3npduibao.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tetpumrb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3coqsauek.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jepnpina.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eujdfhne.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bnvagqoi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zatqzifp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwmcufwc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zyjelwao.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jejdyeja.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3evmbsljf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ffpgmnnz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nwjkrgxt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tjbetlpw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqgbnfcy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xwwvlqil.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3abezbxbd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gylxrtzn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3frevhvne.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qeplxuad.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pcbsmdjk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nwqnmijz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3guelievp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hwgaqbex.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dzissghc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cyqmzvkm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jscdsgba.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qxbyzubx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mbmmezqs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3huivdfbb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ggqloerj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xdiqrbxk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bzxydkcm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3sdubutgn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxnzjtjx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jsehyduf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fhknsitv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3imyclmhw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3omqwkslq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zksnynfo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3thctrxew.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3thmjzjmo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3psavsong.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mhpemfsl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cnexsvuw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bszwnosk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lxwfkmyq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gpktihcu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3klcoqrxl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ocftckri.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bbdsymmb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fyifiebv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nicspgvp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fomjhqwd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rczlxlcc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mxtvopcq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nihaihah.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fknowjan.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pggnyzek.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxxrrwfi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hjmxtecz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3acduvhyb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfypyivp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bledmjnq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ieqsilxr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lefribbd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3strvdvek.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fiacztgp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ytsdlbiz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3odtrsugs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xdcciugc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hpurwwtd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kwatysfq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ddrzawry.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yihcgihm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xqibxtdo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dofznvjm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pyvsuxqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvouglgy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rxccjoqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jibedxkq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3orklrcrk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ngmeotdp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3anhitmfx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cnvcnwfi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ypzdacax.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3knstkdna.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qexdfoxu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3rrslpgnv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fddsitbn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qockfraw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ibhgcxnx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bmiqktzm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mdwnkfsa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kkfenrzg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwqrqbs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mdcvwath.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3etjfusnl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3towjyfvo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fmmtbnry.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ektezggb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3uhhoasyn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3steygufd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zcsbjkjm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrepetvg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pkndjqvz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3osrypiot.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmszjmyi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3suvxgikp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jrbplogi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ynnfafuv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3adoiszlu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wmttfdrk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ddblsgiy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jicfsfed.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ubxkrelk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bvpiamui.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vmfkvfbs.html


<!-- 参考信息 -->