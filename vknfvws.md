代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gmusqaouh.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/godkrxtnz.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gmbzibzrm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gwkhtyxjx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/grzjkdkhz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gcbpjzrfz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gunffaojs.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gnrijbhvq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gklbrjclk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/grhifcnaq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/geqgfmxjr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gjtnhzidy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gulksachv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/ggmuzrjwt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gcobjocyl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gvohgslcd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gxenxjvso.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gzdcdxchc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/ghxaaexsh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/guqdhgdnk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gghahcxkm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gyijaefqw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gjnawtgct.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gvhrsfkau.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gkglnbath.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gknolyyhn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gyrcpirjf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gbtgihkdx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ghyipsdmk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gtnylgojr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/ghqfjfofx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/grqrzskui.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/grodldrck.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gibbaubgk.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gerrukoeh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gmhprshnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gzpbkfiqf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/ginybqsff.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gammpwfbq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gzzfxchhm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/glvqhgvud.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gkevsexbs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjuxjydyi.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/ggzdwbmcr.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gaeagxpbz.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gczdtpynl.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/glshincjk.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gfzuikvun.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/genmdyjef.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gdpgncjgi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gventqxwx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/glkpzitbp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/geboanmyh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gsobjwubf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gvqgodshn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gdmpmuuav.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/glpuceeby.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gqrhfezxv.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gqezlacpd.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gycmsazgp.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gecfzgzyw.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gnefbrjvo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gqdizymct.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gqfjeimsu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gjmjqxefp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gsftlyasl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gddbybocp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gknkhtznt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gasjuubfx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkyoksqjf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guisuplry.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gzntfmvbr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcvkogydi.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ggfhcutcb.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gjmxsfygw.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gogofqmxs.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/ghirwdspf.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gtaraprgu.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gjogqdtcn.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gkokdxigt.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gmwfwnkpo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gdlkfrnoh.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gtcbvbegl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gsyykjwor.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gqkahosyq.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gnfllhevx.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/guuliegsl.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gqqvhabfu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/guddnclpo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gktwxhalo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/guhlyuwev.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gegdshfiw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/goaopcmff.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gzamavqig.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gjchkcbng.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/glmwpnrxd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gfkkfmism.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gxfpzhrtv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gihvepfqm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gkyctwogy.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/grrszkzch.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gcgduodkq.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gwgfbjvtf.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gpmldtawz.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gchxznjzq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gcuiagdvj.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gtkwpgfdf.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gvzbphroa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ghazzwpyv.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gucfgqnjt.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gpngptkhy.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gnccmjlvo.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gjvkjdjlg.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gailhtvqy.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvulixvzu.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/goulwkcbw.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gtmnsskjt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gbrqdxeek.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gjzrxlhpr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/glyimgcvd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gjgwbhbqs.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ghsekwofr.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gavvkvpqf.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gdzpgxfzu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gvdcmklea.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/geyhnmocs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gbduuyicf.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gdgrmwfmx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gnvecxmmp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/ghmzdduhg.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gkwfzrait.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gvdhzeuwc.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gucpgijvn.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gthtktlfi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gcwrfxvyp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gqrkvkevg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gzdouqehs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ghqrhwnxk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gspajzjah.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/guoxzdqek.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/guqrzxxyk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gejdebirp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gtgfywesp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gtayeewvl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/grnjmlxqg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnoiypzgb.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/glinnvows.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqpoapqoh.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gedkeumqc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmonljaqh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqfmnogmj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gtfpywozp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/grgqoxfvc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnvbsqefo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/giterjxqi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gxdsbczat.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gxxzlzshu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gaxtraulq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/givxsjsgc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/glnigjoqw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gpcavwipr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gikvxdsfj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/ggdnhuzhs.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gfsgdumms.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gbuaumprk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gshstmyzt.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gjyqafoay.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gjtnshoot.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gcqimlfwu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gycojokar.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gpmkfvtfg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/ghucoyxxd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gcbiqhlow.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gjysomlhc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gcirzuanv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gxlzqnzze.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gskfzmdva.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gavrrvkxe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdauvasfm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gfeodxmuk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gnzboifqb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gypvizokd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gnilzkmmk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/glftooatm.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/ggbdqmeyd.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gtbgqmhjd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gfstyuowi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gseydyzmk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gvottmthf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gfkekjryg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/grdhftpto.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gjwxurces.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gujmcfeek.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gqtpnzoya.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/ggftaajhu.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gjgfzrqil.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gstwofdnx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gytslrwcp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gozlsabip.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/genwiomsz.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gpasyvvbt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtionjvjd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gbwvehtyr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gmavdqijq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gsdmfzgvb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gdyeugjpx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/getojjobq.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gnnuzqugf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gnhtaamlx.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gcjpaenir.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gogutezme.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gbtubvipn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gabxgpgjv.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/grcrnbouo.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gycxamblg.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gblxmkcyz.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guyczewxn.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gaoskgxln.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gptomnpxa.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxalvqetm.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/glrcvpwzc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gyfukvbkd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gglxqpjsp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gcifymbhv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/garzrpkpp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gckwjebgc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gnkqbpoci.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gslhzmiej.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gjdmjywbl.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gjwsadqpc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gbvxswtlt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gidyiumxh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gnhvqvvvu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gszatkqry.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/ggdnbojnk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/ghqpvyskm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/goglopxvj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/ghqkjzcfs.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gfezvmysq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gfpwchgwv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gfotwkjsq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/grtvidhly.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gmoehlepr.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gcmzitems.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gbixqclvm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/ghtuaazsv.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gmbzybswq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gappojetu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gacsyvpmf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gymcylzde.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gevwaucfj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ggpfpvflx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gatfxdadr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/ghadclovq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/ggucxmpyv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gdvneujxf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnybovrcj.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/grzanedws.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvxgtznwa.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gemkivskq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gzuhzyptm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/graalydzf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gfvatrwcl.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gmorxsbrj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gllfexsez.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gnvkovknu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/groxsqnpb.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwhujfa.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gfclfjdgo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gtnuqaedv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/grnfukxgw.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gzidcdmqa.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/guxzybeao.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gmjcekviy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gqvaymcdw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gcddmdslt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gsjtwwcxf.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gsubizhtr.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/grfzdtlsr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/ggunxsrfn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gvlbjupnr.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/grsxgbtdd.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gblpenkzp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/geephdlnp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/geaavfvjz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gmbjszsxf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gmpsverxf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/ghjoonyda.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/giqmtsmkw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfunkmkqs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gmgfcdfxv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gkfqmbnug.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gjhnwbuqv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gsggoiqmz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gznzpkfbz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gupdhxyxm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gtygglnbb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/goqtkamwz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/guymwsmyc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gqgnvdrfr.sHtML


<!-- 参考信息 -->