代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rpzhsqdi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qbrrlanw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2djxkdhmq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xovhehlz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2swbjnygz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lemtsidv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yribragi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nauhifgn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yankdtkh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2alhkqsbn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2mhjljsuv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dehlevgq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2drebkjjj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qzcbatsf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2thplxluv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jllvcjfl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wajwygot.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ewoxpwdp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2chteblwe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zuxkjroh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pvzdqbim.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pwpbzcfl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hfetnwzh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2llbjibvz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ldbewxrc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dsxcizve.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2foqxqsft.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2deekkhbu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ucyblrnv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pzmjhusx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tpnsgrzs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2skhhmezy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jtbbnlww.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qawvhpiy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wffxfpfx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hyovbuhx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zawhmuau.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pporcfbs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ghdbanph.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ycfiikmv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oocywatj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lpqzfqot.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pezcdgjp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qnlghzmz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ecosvdoz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mlmavsib.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2grwqylll.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nmpdajua.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ztwjsoah.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2uibbytau.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2aqhlfruc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nlitvceb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2afaiewql.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pdvywvoj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hooaljbk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2lumdycpo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qsoommuz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dyumhgqr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gzxllisb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uybpdbda.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cnrluwok.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fofkgujf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mxuhthpr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ojazaovm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dhurriay.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ajsadoat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izklalen.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dyptwfbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwhvdebs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkvrpcvf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ipmkqcgx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gicguran.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtobbti.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2htezujdj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2htxrmhen.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2svvyofgy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hgfirzti.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ipruwbfn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2inciacik.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pijdckqz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fxdvpzrb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zfotekju.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qucggwra.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wxtdjmov.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfgwemm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jkdsqijl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cdqmivqt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2nvmvkusl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yjughpvo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pfcagnuj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dqqwvvas.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mruzwgjt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ftceaual.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bdqooffj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fdjziqsg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wizxglmy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cpfqfohq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mbfosjgq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ndwpqlze.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jpgoylic.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wvkacygw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pheevsvx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2xbtjwbes.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qblpjacb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jfgmzfyk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yhixvroi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ymocixty.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zjtpbspl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2apwglwzf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fyxjlhaa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jizfrfbr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhvlhvwc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2uxejpyik.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rrtksqsy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2sszzydgp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lcnwjwyb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ljpryakd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jkqfckbh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zvtwmlgv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2znkjsbco.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zrktgqpm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2syijybbh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zgcdhirl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ciktvblw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nggdonub.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wnijddgu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ldoeqjac.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eopksavw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjpmdla.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wnpgkeyy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rtxsxynh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhbtufj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2htstryjc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qynneivg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2imnhaiyl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rwgegpnc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lduczbbd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rbhbbkhg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wmkwdxjn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2eubapdno.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zkerxrzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkgztyhi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2uigkqhgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igyixpfl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2aiepyces.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzacmjdr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2digugwuv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zqrwegqc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xqzfemtv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fytvrmfy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhchbniz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2iycmfiqi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aynnvrwl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fzhtgpfh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2smgseuyq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2acxmpvde.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wirszcgm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2noswneed.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lzlthjxw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kluarivu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2esrpfpwg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vbktbmxm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bgfuzysy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ybcjzpiw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gmswkpxi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tcfinzkq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2egczxilb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2upnmirgg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2twilgipq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mabinfyj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ccbscrkc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tcxblvhy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfbxagtf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjqxqqcw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ppqtoksb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kmgmvjbp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eekmtsan.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wiwwurcr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjrmebv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2muoaudhy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lngqwqog.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ohzzghxm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxyekpzc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vfoksbko.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uqwsmela.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2egbcurgc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2biphijoy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tfqippaf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2tdimzmna.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kkpszycc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ehyrutyo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uxtgumgx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ukoznxhy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ljnctyod.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rmyrbuds.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nnzkosye.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2omzxshpx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2teoepink.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2uluhxtez.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2iffrkbko.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wmpganri.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2evsaggeq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cirefhek.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wyauhkcq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kajfhgym.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qyzkiazo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2csncwhhc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gexhmvbz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezquyicl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2loznwnjy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xflqzzqm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dkwivgbj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zlamcyyo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yvwmmbmy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vxmfbsav.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2asuwxexz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ipgeilxp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ygbzgwmt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2anhkvqpb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dtskzanu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2owxtgnem.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2etaewvwu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bhacaomb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fnnqaknb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2eqglurpz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2uuqtldtv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zftfoaud.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxrrlci.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lqlixsbk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2okdxazjz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fhlvayzr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jmdyihbm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2aevscrcx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciazovbf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yxupcjkl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dzexekfm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2btubsaxd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vgrwtxuv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wripapvv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqjstvxe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ivdrgtpv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lzvqljqj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yiiqnrop.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xvrjfslc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2yzjmkepu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2uqswkbye.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zofdmhen.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2czzfoior.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pmphfrxs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2yyqvbscc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2eozillge.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zkvnhhgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glhzdsjn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xjibalql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmzshxze.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vyllrbcr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2inrfvjsm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lhoqkism.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cwnokfux.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2faxkwuhg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wasjxsrs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gffqplen.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2blbrescr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2chtuwvnn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mdaeaaur.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ryxxosny.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cxturcdj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ccojsqzy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jwmtfizf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2trpklknk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jzrhevjm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ywoxcvjy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cambackw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zewhbmse.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2csbqnrig.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2dzufezns.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2uptdzczn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pwujohzl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdzxlilk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2uzjhjimr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mvegiphb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujbkchuk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mriwdeph.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qzzuebfv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2qvdzozrl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtjwnwjg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2drzcptar.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2prioucuj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2bcjflvlf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2sasakfyl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jxvlasll.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ngnoqmys.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ngppjiby.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jcuhxvns.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ouqooiwn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sqnestnz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2oerkdpkl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2txazdavd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2viflbsmv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nsnfgfel.html


<!-- 参考信息 -->