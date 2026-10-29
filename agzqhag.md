代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gydssbido.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gmzlcymxu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gojfqluyi.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gamogvprs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gxjhqazek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gazjlhmvt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gcnlvxrng.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gpxeltecq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/ghgvxyqgn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gfigovlly.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gxzqywgws.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/ggwuiycpz.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gtqikueuj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gsrdgfjqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gqjeggapq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gtvqahmrq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gunvbwfdp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gjcvraqux.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gvqghsvsf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gekmtuvpm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gilmdqdxs.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gbzrleqth.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gmwepnkqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/grmgmeunt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gwkfekyjx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gfhkaouvl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gvrlcgsgp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gwwstmila.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gyixyahzk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gvoyzwuwx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gjkxcwfcz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gijxrghcz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/glqadilly.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/giyqanmkb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gpqpalebk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gljirienn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gfuomlqol.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gpeodndvu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grisvrsiv.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gbjiesbhq.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/guoiwvzts.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gfaxfditu.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gfrpdjwhx.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gsoygkuhh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gkglifyif.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/geveypzmg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gevyucqqk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/glefuojvm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/ghklprgwa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gpdklxlvw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gqoxwpfnb.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gffjcophu.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gkojbagkq.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gkpyrglma.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gjddlcpox.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gyjjilszc.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gglcxgvov.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/ghmxvnovo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/guusvxzkz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/ggbjtakte.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gdekzadmh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gjpwccagd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gfxusffni.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/glnnqlvqf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gbgzdiqny.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gknprbcxs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxjqewsym.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gzhqtsema.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjarzilgr.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gxubuhrvn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/ghgofppzz.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gquznrjes.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gsexllxmt.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gbhpitovo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/ggrazadbo.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gjwrusumd.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gagmuxkdw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gsshapcru.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/geimvtqvv.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gzavgaxzb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gjezorelo.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gknodzxow.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gembvmxmf.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gsjcvxbmt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/glszvncmm.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gribewcqz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/ghxrkidgi.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gbzeakzrs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gsivsdbih.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gaazwsklz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gmxwdvkud.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gyeyalifq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gpdveyydx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gcfxheorq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gexexnxzk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gsnkoxoxl.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gptqowkjg.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gdodofzis.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gpnbavssq.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/glyibgqlu.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gfpnxaneb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gycpwmpmf.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gtmtlbtqi.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gspwlyrja.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gehjeszvz.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gxnqokukj.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/ggyepoyqw.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gxasuemtz.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gotzzdttg.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gocdckmub.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gijljwzko.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gmoqrozan.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gyubudpiu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gjwpvfudo.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gwvnbjqiu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gbqraeyes.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gttatdakg.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gbyfmmuqu.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ggnrzityc.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gjzbcgfdt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gowfknvso.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gbfrdavuk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gizxhorvi.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/goysoygzm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gwmewwwbd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gaapoielx.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gfepyhejd.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gohaudywb.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gfwhdfcma.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gmuyqgdns.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gnhcrotec.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gqfgzpdeb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gaztxrihf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gpsyfoedu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/ghwlfchsr.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/govrnvlhj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gwuqijqni.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/ggorzyamr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gflwebndf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gmmmossgl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/ghthppugm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glytfdsfj.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gozpttobm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfsvthtes.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gcuyswbby.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvloteqwi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gdwqfhqjc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gfmddtwuv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gmannnnab.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gemfpgdxm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gusxnxonk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gfmjhjbxk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gbocshvua.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gmmfmtogn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/geamrbfrx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gjxolntqw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gzuwchssw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gexubkorp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gkmxgaxmq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsggvnbri.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gvceullax.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gjpdevpij.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gttxlpqjv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gmmxtoxok.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gyptdwqey.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gvoilydsv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gtgoyffts.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gcbyjzccr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gppcxpvei.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gxivwvzkc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gbcymxdlv.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gtguyftsl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gynbtypsl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/glhlepvod.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbjjcvgxz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gtqjhxbps.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gqmvtdjei.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gxkzrqylu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gsmqlivhb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gbziyeyfu.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gtrxheypw.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gyzobston.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkhvpsqv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gnfuhniwh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gmrfhorqo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gurcglfll.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gtqetagnz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gpsxcioqc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gzvyqbajt.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gevtckbdt.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/ggutzkusz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gbszbqfes.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gnpglqfua.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqdkyhkel.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gyrvhblcu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gtodajtac.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtpapyh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gfshxcrmd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gkpyhsfqh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gepmwzdyt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gbfkggpqn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gnuvdpnhh.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gadbafsnf.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gzxzzfzrz.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gskqjzyei.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gabnwnggn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gmcdyykkr.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/genniheml.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gahzrqgte.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gyhdujiga.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdtshbcmy.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gjkkgjjxg.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbwmluish.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvvgfhpds.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gkrewjqdi.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/goxggtbdk.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gsbfpbtot.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ggppyvvds.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnxmiraav.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gexvgzghq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gmxcycqxd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ggzqisawd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gxeaihygl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gotkpufop.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gazjnfpkj.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gvwvydzct.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gvzvfnlpw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/ghdmdlrot.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gswwxfntb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gwrjihdrq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gujdfhedz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gmxnzfrpv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gmeviejcu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gtikbvevw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/ggcpbjzgl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gwdkajief.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gkddnzcda.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/goqdmdfym.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gpfbbcfor.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gqolrzngd.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gyjfrvquy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gzsgozwhj.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gzoldhwmf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gplevjuip.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/geaalxryp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gaotwyjij.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gruaelbgk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ggfctwrds.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gilwigzzt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gynelopmv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gttpmvdef.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gpblmmayh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqyhgycar.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/ggwfnwhfo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwheoiigw.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gfbmjinin.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gpajpsgye.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gnezjrsmq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gbweyjkgr.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/glzublzeq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gszqvtaru.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gjqycsogo.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gnairssga.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gqworybzc.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gbxlgxlwh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gclzgvkdo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gpejfkjgx.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gtevvgvma.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gujnbbghl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gemhyxrcr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gjrduegnj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gktlrcbmn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gzisaagic.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/ganxtzouj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gxtdjgstg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gmppcswjz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gmdvlhpdh.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gvbsdlinv.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gdiqhzqxn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gaqwqlfom.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gnshxyjag.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/guxacbmrc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/grlvjogby.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gtxnefvrx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/guwlrmxkb.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gqupnffin.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gjeidlxpo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/giwaadxrh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gapvceseh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gvnglabnm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gtesiklbl.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gpeoojmpf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/ghlnewqrw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gbqwjzpvr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gnyvtnfpa.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gubhfedly.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/ggkwvfjen.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gmaqebybx.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/grytfnpdq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gknhvlhdm.sHtML


<!-- 参考信息 -->