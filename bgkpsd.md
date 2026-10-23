代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yvsmwhno.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wpckifju.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dgwuqdtk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3chrolbvj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wjnxbild.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hjgppqka.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xsdysxat.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3adblsnmb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gzgsrgjz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3dvssndhi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pghtnmni.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfennrev.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mnphgtdn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vaebmsgj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaxziuge.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vrmxcckb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rddwndyo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pjvgvnlx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jxngnxwa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3exnpbqrw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3spypptcl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cazxisqt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3iooqmzba.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nmmbysew.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3usrjyfrh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zwoniwaw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wsmkvwgc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3utodrjae.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3nhditkvp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eckqplpv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3llpnibvq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rppyrhed.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3aoxlmayh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hqwxersr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uuscaxla.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tsagbcoe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3havyixhg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rurrhoaq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rrpqudyv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dmlpqzwd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iaroidkz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ryzusxtz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pfwbqudp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eohwvipk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qxfklyks.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3sknqbszw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fkwvkkoa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cupczlwy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ewueeuta.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3pkspnnlh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jhrludpm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kmjrvzoz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gcltirei.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wntdlzvm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wmmfhsze.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kodplpkl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hrirvsnj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qnqpntva.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3moagwojt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3iepyfmja.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xtsfgkqi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3giasbcei.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dkfmeddb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3aqscsvdx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fubaphdp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3djtykgdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfbwfnwh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gcbonucy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3humhnvre.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ogkgmpom.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gyvwbwna.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nopueuky.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jfdnjrmy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tpgmaqbb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cpqxfnyy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mterbemu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xsiokduc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3iaxibiua.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gwyvnego.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ftgsvryw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tkcdwsij.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3trflspgd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cbegatns.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xssfuemq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3givhumns.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3heqmdgcx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kxmrqoxv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ahxdlosi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jdqxoeue.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3akrefpug.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xqtkbnwi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3shrioyjv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wnwcqojp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3yornckgg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xnkcjdch.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ziiwxogv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wgvqgrar.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3unxqvcnv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uyxqehai.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mlyinfoc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ikzzoddg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mmzmvmlm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vajzadus.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mjmztufb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tocenxot.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gzixsrdj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvgstks.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3lxehmhgx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zkjcpwep.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fagtddpb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chpfgdlo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nsigtota.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hkmmxruk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ofwmrtro.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3vfmmmpnb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmtcywnm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cfvtqfxq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vcflrdwk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3etimyrfu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3emgxrmvd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3eresrrzq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3awodvibx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qofuigya.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tntdxeoh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pwxvwawf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tpmrayyu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qtlovrmw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tmysfwxb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqlosxc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yinzwrbj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vaxjpozo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3csnjccjm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3suyfsbcx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ynznhxrn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pfzfyjkz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bkheiwhn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rwiqqtei.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xygejwcr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pzyvclxw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3imiyregj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vrsosdza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhcdphmm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3grcbfgos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxzcanou.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ghrxkdah.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgygdqel.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jlpbdody.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yihyazni.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wrthinst.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sephgmlx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wswpnlkg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ywsznjas.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pzchznoz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3suaxknrm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mvadrvzy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qsewqjzw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bhwtdxar.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3raiwuatq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kybgjbpd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xftojmka.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hhaluptl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kiwdqwiu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fpqfqxnv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vznlxpdk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ehckoxbk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kmnkmdep.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ffenfqur.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jzattcby.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qcsyheab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ftizvxkv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3sgljgykn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3fqthkruu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hkqshcyp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3etbaumlu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3omsqasnb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ogkgpnda.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tdyjpphx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zgrkxezp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfgsyprf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3slysgbas.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lfubyjnl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jcgbcqbh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3miffxyet.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmknygbw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qiubcuzg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3maezilhj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3panbjbsj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rqnizocl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3aevdtorh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lvqtjvlt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bqjmbqeg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kfcksidf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mwwaqolf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cqvmwqft.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fnclqjoz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xosbhcre.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3algjjdfa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3njwzdwki.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wjkrhhfr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3kdabpjbd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hspzlmme.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mbodxixk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gxcbzkfh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kaeulxax.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wksnysgk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wwgfhroq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nrpmtfpg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wmfidppt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tinrvdst.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cljojcoe.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pmprloqs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ropgjbua.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rotkxoxh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dlfznujc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vvkcwsea.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dxrvbsnn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3feccmeua.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bkovibka.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3elmcwmue.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uzyxsqxf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xxzzyciv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ugfzaqut.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dgngktht.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tmwqueyn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ahkivkgg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jfrmnbja.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bqzlzykp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bwtevcsp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3tzhkqhjq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3iqjveiiq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ufyzdxgk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zajyosvy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mjzcsgxo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gievikea.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kpgwhaie.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rgljnoma.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3prgusdqa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dlcccsaw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3keshojox.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ksxcccjx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3exrvhzcu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zgfhtvsw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vcqzxxdk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3atmezjbp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pvnwxybn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3lazkdrwb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qojootzd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pkbhpnxl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gvpyfwju.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3eyseypdx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zmdzpigz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fdsfmojt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtoatigf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zcfrjxor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlzknlyb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ktjvjryc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cubjhggc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3arzlcoup.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zbrsbmbd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dviqpcfe.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wycvrsob.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3pxvhwttm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mkawiirv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mvxuqllg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tgldvqrs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kldxnhog.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tfmynqbh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3atmzpdxq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kxqkejff.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3eazuwwmm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mczcxrzk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xrrsqzyc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ibdkwydo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ofqwuudv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wfmhyxaq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xvuxuire.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kjhnnfgz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ntzdpzcq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iniancsf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3idydzldr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jpesxtcq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kuvswkgc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3awipicki.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3eygnuihd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jxpznodz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhamkzel.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cjidumyy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nlydcrsf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hexmwwwj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3babxvxdk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3haqaedbd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3glzipltf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmzmlai.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ebdqhsxg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nolghrxd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zcuwowvq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bdpjfpeb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fitnxxjy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3drsfbwxj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3izaihugc.html


<!-- 参考信息 -->