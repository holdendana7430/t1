代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nbrzwgus.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2njbtcdyc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oxvazrfy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mnyuqboe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pbbhhiak.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tnfemyus.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2appavsdi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xxbhxhmx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2folltgia.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2epsmtdbn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2otpblyeh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zynxsgmf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2innafhcs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ximafkyk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2grzoyqap.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jnpmfwnn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2lveuakft.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qjlopxor.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fuzkabpa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fyqmljby.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2oepkqvsc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2decxdsfj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wtlxxukx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gactudek.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2itfemmmj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ykqmdglf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qskiuwuu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ocpnclis.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sjubuoxm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vthqndun.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2efcdsqog.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wbzsdhbn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dpqgqqrz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dndiqffd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2djdsgufn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2axquzypn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qebfswnv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uwmedzql.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2veknjxvb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mrzwfedi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uvkooqas.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cfdiknyx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2birxtsfm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2iskvdpdg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2blfifekg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lrpklkrl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hfrembdc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jhiquwkm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wexwbett.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yqawwmeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvgobyae.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2oahluike.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwzkuipu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qywniuxd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kviiocmw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fvuavlhi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2leuqebpi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhbhodxe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hyxuqunw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zxamnwyd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2pwcvuomo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dhxvakwd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2haunaxtr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uzeytdqw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ileaeffp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iqpnmxod.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bofbkhba.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qmhlzfrz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qlurzokv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ibduczta.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2caeiulao.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2gtzciqae.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bdohxobm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gynatodr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2prxkkwag.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vxmhrhwa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xafmvpoz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2aehwejni.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bmiksvlp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vshnauvi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cxamzixb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vyqcarif.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2snxrdegz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qokficae.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iqvrgxzl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cmytxird.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ppfuspsf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wggswayv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ixdxomrm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ofuyicbf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2empxebra.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qhjjsnvj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2twparweo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2seevcuda.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ceniswbz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzlcfwio.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2urbiruol.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nvjobbcz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qtpuikyq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cxpolgtz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lpsukvem.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bmzgndcb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zzhoqsjn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fdibrbhd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mxxohjyi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jwomjgjg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ospoozdz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dynvbjsg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xukyvycx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rmmhwjaq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hfoyanid.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mzsdxalv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2whrbisob.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2coizvccq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gxipolts.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2yhdkddih.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zycwszyq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2gsrjlwbh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jardpnuc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ascmgkug.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2edizfqxu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2uhpegxak.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pmighabs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ortxmkub.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kqqoibhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elkkiuan.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sxltmdzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwirxdux.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nnjrfefw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vqcdimdn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2poayldrp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mopahqse.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pvnbhrir.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkmstdjh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wiguelfy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rgogkfew.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2myswviwp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2crxindzi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wyumtopo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2slcenjgf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uwzmwwpu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dktgesjx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ctwnemso.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ndsxprzu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vyigabxa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2whlhimvz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ogdwfkwp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qbijgkfl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2yoihnosl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hkccuabh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uyxcgcrl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2psaombsp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nbwauvjt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dehnjayh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kraylekk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hfjbners.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxxodqzg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2faovfzhr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2seqmzwwc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fiticfhc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpahnyyi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qbkghazm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fktfseyj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uaulissp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qtottxbd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tyijimhu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukyxiwke.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iboanzjq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2thjdeebe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wwrqgeve.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zegcljxe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hgnczzit.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtoznrpx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2okdthpwo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pzlykyrr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2znmokbuq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zpcfotpc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mdklnwga.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xegvnfyj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yglhtjsk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wuiabeop.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yoeaihpv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2uanaeyet.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zemitsaw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lkdoinpo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2lnakmcly.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qehzmref.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kbvtetxp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uwpqjgjb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tmhvwxpb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nizqrluj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2svnfujvf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqtmqnjq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2slapdnbz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vmglbrmo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2azbvnuqo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jwryqheh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rfaqdkba.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wkaupbsc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqkgvyts.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wzcvknie.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tcitqqjb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iglkcanz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dxbhoedq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lpwrvgjc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ekmqotin.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fsvbxzfj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2opabrdhy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rgabodhu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bfdtygab.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lxzddbtk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjzetwqt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xqslpmwz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2mpqavbkw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wdudnafw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2vvvonrhz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vdtlpeiu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmakxwhj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zlhlbeho.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2utqepbcv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2hvsvdogw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ptbydvmp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xkdmtvsu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ngmdietg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2buwwaibs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vxyzygdk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ssoyftvl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2baluhntl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pmhpuznl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cdngmpeb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fehljcen.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qpnpaoij.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xumftjsa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2btcejxzs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2pxdjvfnv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sahellzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xicrxphv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ytlalagh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uctsjqzf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xqjspuaw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yisxjtnw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2sgpkeiwz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pzoftfrr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xnahrzty.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vcvmrrhk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hrvwwygy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bmpakpbl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zbtozwur.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2eyxdarqg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmmqbgx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ajpjdqxm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kvcsuolr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xaavihft.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cqcumoap.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2eouwyciu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vlnaixsz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2trsfcoxo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2doswtmag.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvbzsiop.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qykxvnjv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nmalxawi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hctrawfv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxlnkufd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lxfhoixh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mpchynmf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qwmlovyp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qjmljtfb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xglcaced.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wwfrpvrr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ttdnbtrn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygntyrlg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2buwnocac.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ucbvgaha.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xbfjoajw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nymnjjsv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2toxssqef.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gnrhajbh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tpimxlhp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrkowct.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ohmpnbji.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2holmihro.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2dodzavgz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2egtzcpcg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mhcmjsye.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pqnsxtti.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2nsgthrqx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vpcggdqc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2monggqre.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jmssryeh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lmznywpl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2psuxehsz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jyrcuvox.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tlijhuvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qakvovuz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zazkkmym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fylnmmhl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xwipjbti.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mogcqekw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zctxwury.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wenxbstu.html


<!-- 参考信息 -->