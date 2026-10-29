代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gcrxzsawu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gxlmvrkfk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxhhpicm.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/grabmjsbm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gghsfreef.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gdhboxuvm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gawzvbrhq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gtrxsshsh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gsgufbsaf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gwrzccbfw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/grzxmbibc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gzbpxmnfp.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gtvcquzmg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gczkkyzbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gyhwmktjw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gfkcmevhj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gvfvwhmkm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gcwniuvcg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gbzydqiow.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gablnrnly.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/ggrultgln.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/goikewtpb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/grrhrjixe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gwctjmbbq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gfkylukfw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gygpmfqdt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gfquxaipk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gmwkwchdh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gngnlzulg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gxoijvtpj.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gwvxpmkoj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gqxrkeuek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gqjohmbci.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gyewzxvyu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gwtpjjxxk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gkddmwkbk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/glojwxzai.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gksujsrmz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gaxylnvwv.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gdjsouvec.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gmwryfqde.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gvsnjkjdt.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gxaxwbpde.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gakowgigs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gsgepgzip.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gvftgbmkv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gvqiqimgh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gphqslmps.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gipyqznta.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gwlwdqyoi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/ggwgxnbxp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gzmgvgqkf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gmrbeasrd.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gqsbzoncv.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gaotjbhjn.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gjlnjzwcd.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/guwjbxufu.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gyeqeefhl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gsmlzqghk.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gzjaczism.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gshtlbawl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/geekgweso.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/guxzwcqwm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gdtxinnmw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gnryzilaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gacbaslhd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gldhmhzkz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gzcoczysv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsrotmqwx.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gwrtxbfdz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gsccrbydw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gznynxybd.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbgtqzyd.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/geamyffsi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gwfjxxxsj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gejwfomxd.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gcosuyhed.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gqnfoozrs.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gizaoszkc.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gsrhwsthd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gynlaexmn.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gixpmgbse.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gxjxdncds.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbawirnfe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gezooomol.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gfblblzhz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gugbaudom.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gyavmhuzs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gnkjgleop.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/glgvpzgcu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gvgeybgno.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggbcmpygk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gyzvnlhxt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gbirryiah.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gxfoayecy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gxdtolkpo.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gxjijgdhw.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gyilhbnok.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gyywpzods.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gghipgxgi.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gtynkqaoo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/guijkzive.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/ghvbxhdsz.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gsudowijq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/ggttiyjov.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gxqzaajls.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/goqnfmkwd.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gzvewpgty.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbqnptofl.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/grlkuenef.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gxqoeylmg.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/geehpsspd.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gqglmzyti.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/ghcutadlt.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gnfkvelyh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/ggamhxgkd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gefutbggc.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gzaarawox.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gfnngljiw.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gdnkobwxv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gjwhkdhck.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gctofpclq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gxrelbpsw.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/ggvfiuagj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gsygaakhq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/guycfbnrz.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gtelfiysa.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/grzvbvyvi.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gyezgomln.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gctgtixsk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gszutsuvd.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gauwnxfsb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gnbwpciot.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gmosqvszn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gkjphnxfb.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gcqltdjiy.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/ghdjxclvp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gmdotqtes.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gbkpflzgf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gnspokqkw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gsdnstgpn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdlbopyeh.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gegmwhgiz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glnzaiejn.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gnmduftqs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gjavmfzaj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gfaaudfni.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gpboftjjx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gxqkqkokk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmoqcmhkt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggskkpexg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gunwuiqkp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/garcsiqmp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gbaoerobg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gknahtkoo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/godjnvxys.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gzyuofyta.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gfeiwyrjs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gegqmzouk.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gkzebrbwd.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gkjsxodfa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gewegadns.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gzbwohhhj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gbuqrgczo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/ggksrrlno.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gfaonwrkh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gpkkmvhgf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gawgtbntj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gtqxfeddo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gdkdmapgn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gzidimqfi.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gfxhdjzvj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gqizkwdax.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gtuklygyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gljrrybvg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gpdhgdlfj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gbfweyjby.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gzurujdtt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxpdsxhpx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gkcrilkbh.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gapvwhxes.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gwfdpfwzb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gvtszjtcq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gyvzzyvwe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gpsmdpyzr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/guneluojw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gfkedjwuw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gxgotvidm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gocpohmed.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gdsuuxiij.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gkluulbwn.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gsvkgpubi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gxljiezvh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gldwsnsiu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gmzrpviep.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/glttkxxde.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gkftclzpf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gnwsahbfb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gryebzsoo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/guzhclwdx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gjabbakbo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gryklgssd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gvgsqyywc.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gpcrueyza.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/ganzakkuq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gkieoyxid.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gqcvmehgi.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gxhkccect.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gifxzaqxl.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gncmkrmot.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghiqqjvkz.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gijxmgalf.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gomdmkpia.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gragqeffm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/ghkcfjxrl.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtatqxuhh.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gadbhfzxg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gxxyyamtf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghqdveayc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/grsfjqusl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gtfoikafp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gxghqygzf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/grhsprnrx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/grxtrsjnv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gwtcscqds.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gsikavhwt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gtvroqdvl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gztdfsrko.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrxhgskk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gythtqzkn.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gruevqakg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gcrrcczmt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gidifkfzo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gtjzvwjfh.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gwrqdsjbr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gjzhtahby.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gikgbicjn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gdcpbknbr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gyfcicimt.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gbuszwuja.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/glbmwbcwq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/ginseqrsr.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gxwihgoni.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gocqfeaub.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gqwjelugi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gibzqzipe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gtffwptxu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gkoojbbzl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gkftijzmi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gatduooai.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gulihglcm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/grhvpqthv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvlrjqalo.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/glsenbuiq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grksndxsd.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gqjewrnsw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gdjlppmai.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gywuexpdf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gcrxedxym.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gudxvtygi.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gepapiwtp.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gosjoqbkp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gaqmdzqgp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gopkyvvgi.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gsyowysfa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gwphflaht.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gcxxrxqdj.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gqlwfdosj.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/ghkwgeyhk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gykormlta.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gtwdzkgtl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gajavsfdo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gajsbukqm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/grnwlcpwc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gvnapfjyu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gptznoabq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gbyygptyp.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gcxduyjwp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gynornfhn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/glhqsimne.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/glleaujzf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvhvjmom.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gxszuzzva.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gudfifuxu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gqgbzbmig.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/garntpysq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gxnyqpveq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/grkzbsyyf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gxsqdndul.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gqefwldzo.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gppkqiomw.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gzsyztday.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/grunlzufa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gsknxmaue.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gdvztmesk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gpjgisdpj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gofdyjmgr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gbysxenlj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gzubleepu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gjgsoolov.sHtML


<!-- 参考信息 -->