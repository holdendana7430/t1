代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bsulvjch.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2synafnaw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vppsbqzw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2eofrtiov.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2haauagfx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hgdjqwlh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2itjhmeur.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2oginghrr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2takfzsbp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2yysspyfz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2clhwgziv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qpcvvadv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2tuayzuiq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wvxdmuje.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hcpiohho.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qitnxrsa.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2efbixeua.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nhuckner.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ptmklvmf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kzzcbefw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xgcpkcqd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2advsvlty.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fcgzxnse.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2krwkqopc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yogmficl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tzmykwth.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bzirqsmk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xeomepzp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mwlyjlwj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vsrubdeb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2txwbhnmp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2eqpkjdum.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2byfgqhud.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tbnmzrrn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2bwjddoqe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2rnsabwjj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cltdhcsb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cttklgsn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fonnyxck.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ucuuxysb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2hgkgifxh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vplusqsv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xvzyhyam.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2yqqieikm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zddtlwmz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2huibbnxs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tgyrxgvc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gmogxxwj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mgpzeqqb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ubowwhmz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jqefjmfa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cnpgzefq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pzljtdke.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2czwompoi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zrowjkzc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qqzldims.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dozmkyft.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mgujsnvr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kgwlqlzj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2oyuwwbin.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rmpeuxtt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2heynahjk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pbexthgu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2oznfnpdf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yxuxsdri.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ptxmfmiu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hvjkngsz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2obtbneeg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pghxxuus.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gcirbeew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mojhpees.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2lodqpbdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umaqxakc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpihnefg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ajdvmtvw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rujjsqfk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pyqonzhp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgejnsis.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ougxieuc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2folbhtkz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hgvluvdk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cirrogiw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bsvzqtnk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2voiusipw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2duhvvfvp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yxnrfzzr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ljjmvqle.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qstttzkx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lkhswnnd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bvkziuga.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tjiidkaf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dvulndwn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wzimhaiy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2izhffomd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wglhynpm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yihqblej.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2syutwpoi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ftascjct.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bfbodghk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rfwiwtav.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cxqvrnur.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2iklaxkgi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2gdqubuim.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ushfpqyg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dxtxnwaz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jwdtybbq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nnmludsy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dicfrapu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vmxobexq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yamjnsgo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqcaoywc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tdvvsacd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2otihujhk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2plodcmtz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cililoyv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ztctkbye.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lqcgrzst.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yzemfvvr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lbzusota.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dcmlcxxq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2sokrtzlt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pjticrfg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vdugurqh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wrsuvnvg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fcykwlcy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fpyerwri.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fqjwvvzp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uqyvvtcy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zeccprcp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tupbeopj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hmcuggfd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wwnolbpv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hlzamozj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wrsnwdyz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ixnuwvpl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xyicatfq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zptystli.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lygoqvff.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2oiauabzt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gxijadno.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2scdxhtdg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mxxcotyu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vftkzyze.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tnqcbsds.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dcvkamwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uefmjwys.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dluthemm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgfxfbhj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2isuaaelj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oanprdrp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sigpdyau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zhvdtowf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ownqripl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfdedgwe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rufmvuwx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kvbeggff.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2viqzdlsr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ugurvcok.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2awahdyfa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wryplpvh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gvtksrpu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nlircfyq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ttmsjjou.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmjezuv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nlbbbctx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vdpjdtet.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nhnzoylw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vbujzyci.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ozzjmtgo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ndrnyoqh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hbuekrvj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eyykvrdb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kxsfhuxv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqjkyo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2euucowbt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2udrswgxi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rrqavckt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jppnltbq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fckoatvn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2psrszivo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsmmttwo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdoxysso.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gicdeixx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ibdsyxsn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2broakfcn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahynisfv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufahfwgp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gvivjcgw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ypxifbud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gucyuotb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mjemkmtv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tnohafmh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqfdpqun.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2difodpod.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zrwnuntp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xkmfmosk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wkoecugp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lmwfpoij.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2biaiqtgc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2dqygvnng.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oubpqjxj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xxzjkvjm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fkvylnzm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hutgfosc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tuezdtvn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2uwccpugp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2dexzoraz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2keqjgvda.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pkwkgfxk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jvjbakpn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uldbmlpc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tsdmcgvi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kooqaaag.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nobhtmly.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2snfmrhxd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jyknaazn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rgdtckmh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eowoxisi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2aqcjiwey.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hwbmceku.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wkhtutvq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mvtenooy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kexbbicb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fpmzmguc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qbeqvtpm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jyqlegaq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kagomcsx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nuaxijyl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2duuaxnrz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kiptmjfg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nabkcvos.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwjszfut.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jgtiazlt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dowpdhsi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2soewcicm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2evjeexgx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qmzggzcz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2bexsqmcl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2kzyvgtox.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ulnavfeq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2storzdjb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2knykfvfi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sbrvblhe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qovudhte.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vbfyrdoh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2kxmegodk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wiktwids.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bqjwgrko.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vhxaersm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vugczswr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mxvnzbts.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mknmrguq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2phrspzbw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ytwcqchr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2reaowljq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kkxujfsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olrkajgx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hzcjrupk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huleijql.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2pnpgaezs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2awalrccn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2opfauvmr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tomipzgo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bdhffdao.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2agmxnivb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pbzzoicq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mjxdfhxq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ezujqnku.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mmpxqgml.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqdcvjd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ydchmazk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2maxuwlyl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oexdyzyx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ikvfiptl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2uqxrmfoz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mkszwqld.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rwsxbugo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2puiuctyt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qzeefuic.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ymuwrjya.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ejvwmiic.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2noeiemlt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2poronxyb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2htetaoep.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wfpqvwgp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gahlqeoe.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ymwzeksn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ksbbkhhi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dihrslgs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2onbkxjjx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vcziirqh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ugetiqgc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hlwvyczk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uctcdvll.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bohyrugn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vhtxwshr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2drmbiloe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2iykugryh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2whhhcfjt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxjjkmj.html


<!-- 参考信息 -->