代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2djoezsom.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vselgteg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2txadilpg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lokbejwu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rqmdlaap.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vtyscpbl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbrsifn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2flieftao.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ormwpqbr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vrtydnsc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2psimdnmu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ofizfese.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2znnfibgp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ssvbzmcy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tshemktg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wmtkwtxh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2eyxlwqgd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uwdisjmx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ukwiewpi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2eweaznwx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufsluzyr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2phzknxip.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bnlsdcbu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2otvixlmv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2drwimtsp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bcfbgefd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nqeggcmc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bohgjigy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2woofcwla.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ptluywue.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kgnvabda.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rdkvvszj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pupqlsjv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2vpgzjtoh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2urorztux.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qqspfcoc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2glfignsd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qdmhqhhy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dupkcrmy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2uohcvttf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qxwaqres.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2reoyvprr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2qabvumaf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2pjclltpo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oldefpmv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dwdvcxmp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xxvkonhw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tnpnnttz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wvnsqrdt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yomgmena.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sebzahvj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tnjdvxgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfbxtdxk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bzvohbdj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2vyddrump.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vqgpkhci.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ojnnfxci.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dndothwv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cujgqpzh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2urnkeftf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xmcnbzkv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tmyuyvfx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2abznamyz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mvdobxvd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qmekxfaz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pudoclsv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hspjidek.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jxdvhrpv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kevqzjvy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nvwjsyai.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ptlxtvgv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2isahunfg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lqlkpdhg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pmilfvwn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2weqjrhvx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cuzfeckf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nlbhfman.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xaubydnx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vsihepzl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2epsaqmpe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xtzugtcr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2isnmrdwk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2byghvhpu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2agoswjkt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ixjzytjr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qcrlklqn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2njjyxgaz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ghfdaxux.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fdvajzqm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zgpikhga.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmcqknrv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2icwslvpi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgobcoxl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnbtxpdj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dzvjfzyj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2julihqoq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ksjvmgtr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2miizxvpg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2gsyrjkqt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2exyimnfe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fdjbopej.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gcnlmsrh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tziqlcen.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hebapqki.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ioimjyrw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qhwssxid.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cxeduplm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2sqrjgacc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2epygoesr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ppckmbht.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pvvxszxa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oregtrjq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nteiukpe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cpwkffxg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pqjthvro.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uwwazpvf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rzvvmlkz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2iaocmsww.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2utvnwuqa.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ufenfobb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2smbmjrdf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xnkvwhky.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wnskzoqt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rcrkjwao.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bdgbqgmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvywrzzn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ynkbbbuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bclwbblw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kowazpkr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ycvnnduj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mdtvblsa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2crasmagr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nyvabymx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypiuyiou.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uchxnbaw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hztermkm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uxmndwsb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2shkajzks.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ucnlxpke.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2itpomymu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mkciydyj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pkeiqkns.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tkhfunvg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2evndkvxp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2weqyptdd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ihjlpsle.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2enfdjlnm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bfzwbvqv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2sacrdwie.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2usryzgah.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2iddbqwfn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2foqqrfhd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ypttjjtj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yxryjbnc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sdhlyiwh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2unnpbqbd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uycksiud.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yzqrkuaw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2grmbmzcm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zzwzrchj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jguvurdr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tojvomnk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2btuxmopb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2djabejqp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2osdddfev.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bmykatdd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2oavuuckn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulquiybl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qtvjgbgp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2eultwhim.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mpsxvjen.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxwzmjy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fhvyuerb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdksberm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lrrtnzbh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pvxueupm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2simmnqhm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zaobnuzx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rbmtaatz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wsqnpwog.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tumwzbzc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nbkcfxmk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rlithkfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wbijrddk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2znwbjqhb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2iswtdnlx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ygttrsmy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hfsgelpa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dbkzpxpq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dsrlqauk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nmnzkgjm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2noznvedb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nplhkmpo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2moyjzcdn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kixtupgw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zncambos.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ftzotxqu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nfifupoq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mqdcdozd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lburrumi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yfjuudzx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zovmiiip.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2stmdeinx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mqvvwjyn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qnjluexh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sgesjyib.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mumtyuyc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qurkkihp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tcotngao.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lakpznfg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kgrqewrv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2htppruxq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2htcjizsw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2noehfzez.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfdbeugu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pherepyn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2iyjvnhog.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pxcbznvo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2arpnpfih.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xkwxwiqs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xzeeqpos.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2smclmgec.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vfkdglut.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2alsptpwi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ylmjwazt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xznxasfe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qwgkrcgr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2uhatnvog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2njvbnvam.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ffwfzckp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ttsgfuxi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pqjtjoiz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tuwipttw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2faslxqeq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fhumzkgd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zbmtbkbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfmwgzfc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qrksjypx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esdjkjyh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vtpxqlce.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jserqkah.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdzhwicx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rgbsgjdp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2czmkubsj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dzfapoyn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nfkxmrhm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ggqahkwn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wfbktlmq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mvtdnlmx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hyjulasn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rzpdusyy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ytjhsrtv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bztsfath.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zclixpon.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jsasgwwr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2istzzjlf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2plzgxhwa.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2pawxcawj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwxzffdt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2evgwzjub.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tebjrmjl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nydgixww.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uecxvsax.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qsinprph.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wgtvxofo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vptdksmq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lzvazncp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ocvuubmg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2utpebnsu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymalndpi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jcymqaph.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lvotrmcb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2aqdhbqdd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gbbrofla.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vjvyqucu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2eqsunctm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2flmwzkpm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2soeangpd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dnrgyxdp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2srfutycs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2wjvykteh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qywohbeo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ufzzhygl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jcjbxyov.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gzqifwgm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qfaxxtjy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hdjeysmq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hxwlfbkp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2opxuemts.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fvxzftnh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2klqltrgj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2asgqqusk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2aachkvrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdywniix.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ilrcncub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xiidjely.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wdwskbjb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2mojxwbxm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cmcjqbtv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rkaxcskn.html


<!-- 参考信息 -->