代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sfgrimhg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2irwarpmh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2kkixzytx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vfhhepjk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rienymwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2sgiwhzlt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nsapmwsd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ehjvzreu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2owpkjmjv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bphsbmqv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2jmeqoqag.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2youcqlce.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vpiuhsdt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2renagkyp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2zspvfxzz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2eaxiojwq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bvbixmqm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2lzzutfar.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lxxdvswq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2imcowixn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vaogqrsk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2asfpturp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2eztfrzji.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qgckgvrw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hwyphjrv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tzstdwhj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qmamwszu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hsdabaym.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2teddbsoc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bvobqilp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2beitosng.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pemucqye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2eklkebmz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ugaieaht.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2egthivgi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lsejekel.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zhpaiyjk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kgkbmbnq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kqxwotzh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ffohshkq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2asbpefyz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hruwggft.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qhkgcljk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ddyklprl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kyjhpeei.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2pmfwwsmj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zzdsainu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tsshlbhy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2islklrel.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tbnesccq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jgtuxnss.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ubspxxoh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hssrlpcr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mlprmrvf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fxsuljnz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wrvuhxwt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lriuzmfh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bfhlehyj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kwdwdiwr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2phutuqsu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wuhfmced.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qewcojod.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2uqhksjld.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cqyoswrj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pvfqfcfz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lkeabxnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmmtndhg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cinsnqpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohzaspxv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pgsijevz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2uacvojdv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zcawbdtw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckzfvnui.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyjpuqwe.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2beuvenqx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dymddtae.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2thkpirvo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wbxnevyh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zjpwkoxn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ksrvgffl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cvixdcau.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xawmjilj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2leqbfyhb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bkrzookw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lqbqfnng.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dcjxgkra.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kaevoedn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2crnwlzpl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qclukyap.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2esnmnjpj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xhrxsjwh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wdiqbysp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qgulgodx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2veokdhoz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kmxmowln.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cykkyeuy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nlptvffn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2iyvhmdji.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ozydbhtt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2crodtycn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iduhhxcn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zzxrmkxk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cyezqirt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2axxaefpg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2rdibjrdp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2selbyqwz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2guaknjlr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2enjozwvs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvfwjxg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2okoctlpa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwfbljxu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgkizop.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ztmepsyd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cvhuzewx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2exaycylw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iuhgvyni.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mcbvcbyq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2stkgpzrx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hlcsasfv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ozaimhrp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2avkacceq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ziqxtahq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lzkxlbnt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2liddwmab.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2aklhlbjy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uqxzqemb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uppgjhxt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mzohjhlb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qraxuybg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jtdsdnuc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kxxggxgp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bjzrpgkv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gyurimoa.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2atmaovoz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2erbhhyyo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kgcozvpc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bfxxqpxz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dlyrbpjo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2gjynkpbf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xjqzqkfe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vgygvcwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzdsrhmx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ieqhczgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkbyzhlr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xdznnntk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxzbkxbg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2odgwtfic.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwuxfy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qfeyhpeg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qgumzqel.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhlicax.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xtptmgfe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hejgtqjv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ntjdluoc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nvvmxtan.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2dyqdyyod.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wrgbgnlp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucwfnhuq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wflorqvc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xffgndlw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nhbmuvah.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qtqitfth.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lnwcdkzq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gruycevo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kfryqjht.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qeoklhpd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gqdaaunz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qykcspsi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ekxwvchm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wjforrep.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sylosjwx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2titsexmf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2azndkgtc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2boetgexa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2njgooita.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hrpvvpav.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2iwwukcfu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xgdefyor.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ugvqnzhy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2blimkhsm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hlhkfgwo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uerwqkij.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2thkanzly.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uulfxqfk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vahuxfss.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2cvjchmdh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jzladodw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vnpnyqmm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2deoxepwh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lpyddgdj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ngopzzvb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qzyougcc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xbncfcba.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tjpumlqp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fesoztww.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vknjznmx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yaurfvdf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cfahhnfe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ypgyulxl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2euhtvmvw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lvnvwgqd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cvocfkpc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dgxpjuns.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zjpydkck.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ecwgzvqy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rbgzmhgo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2sgrpgrxd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hdmfeuhp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uevzpgzt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2taspfkxx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iycvsxri.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2stbqnpnh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pksoywif.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mpcxbkph.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zqzszryl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mdeutfyt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lekguqfm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zlbokyrc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2clcwoyqm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2beovrwpt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cfifyjhh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uabmmssh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lbwmcnbb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gufqtepb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nwwcqfwx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fkieprbj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2svbpkina.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aylhzfdm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2oyglcffr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2tppovlnl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2opvlthdj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fozllpre.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2umaujjgy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwsnoeqt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2djdetydh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2eimtelox.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gtdukajb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pbvnldtw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2egczctiw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dnfqoebk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nostifeq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ijjyvasf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vjjednjw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ovhqnbuw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2aawxznyh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rvjzujhu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2efdwjjuh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jokxdzqe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ousofiwd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2krqpmvdc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eqquymiu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2eemfmxyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aitoiuvh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qmyhjrht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gchvdlmu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2atiphrgg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qjwhbtcj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2acillkfg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xmdgfbew.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ipzqioyq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ingnazhm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vigldslj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2eviewrzw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2fewebyst.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dnogbqcb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kahiwkry.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ywgsgcqs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xmzovjjm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jyrqhqsg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nsnzmefr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2uczyyskm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2bohmfszw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cngscxeg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nttvofzu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2sytixguh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jknrbbhu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2tzydrslr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ajdqsmqu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lsyfwgdi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ewbkjsfj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lhifncdh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwgvznle.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nwrtazjw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2prpswyku.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ydmlkzfo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuohssyw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bhpizmly.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tvsoauru.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wrxoeljk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ktmwkgbz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2kqsunydf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2aryfqztt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qtvzcgqp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fpkyahlg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pflsdscu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rvssccwl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nhxsmgva.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uguhvjfx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ggwhvzlj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkvpncn.html


<!-- 参考信息 -->