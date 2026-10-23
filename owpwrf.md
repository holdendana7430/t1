代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ttzxlpfr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nquudnvh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3knsxtahu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rumlpxxa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3uhcfyaaf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3spfvnrpp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3klemraqd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3jwheaqnw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pzruuiee.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3iouyjfex.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gecnjuct.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3kebcrohp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ymgqmvij.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3gmkaesza.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jwfmnjky.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3eebdlpdk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hltzilsd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xfqmqbbl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3orrqtxuo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lhxoxaop.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ufamwouv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ekqifxtr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ppkajtnj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3luqfvqoa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bemzpxad.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3carwzvtf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rntznalm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mhgsuwil.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3feyaumfi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3liuqcivw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tdaxedks.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zoevpmpp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3iuoxjcaz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fumlkazw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tkxwvcqf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3haizvgvh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tyygbcuo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nxcuggiw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zjayhmoh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3kcrbwsvf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gjapygit.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rkgaxgni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scrrnuns.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3toxdeinm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nevmjupf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3woebdwwb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3uaxbcftk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ndbgrsoy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tqjiamca.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxakprrq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xrmukncs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zpuqrrwi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3htasisul.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bsdxyywo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vbghmocg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vauqgryd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ifnvxeba.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3utrvjkpq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dhhfxlrm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fthlrfjc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3omglphum.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zjxjfosy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3olnbksxz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vmhnsaao.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3quvmkiof.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ziclscni.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vmsbvzcc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rcdluyrz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3yayarjnu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jgkbijlx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3grtpyebc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ugqrguzc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bxowoegr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zfikmksn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zsiyhthp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wvxjepfe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ihxisllz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qewtxkct.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3anhvxurh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3nzcqkuwp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xdpsbbtn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3djfjhxrh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dimyeznb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mtvaxcft.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vpigqkgh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3veugeiaw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ogzhxnmg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ntvwpeeq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vmvhzlsh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fvmepmuo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tedlhblu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qpefjrnq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jqsegohu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mtfkumqx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3suedxjxj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nanfpgcd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gwfvihib.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dxvychtn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3btckfeof.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ghhylzsu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zzwimkba.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3iumhlxao.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nszsgnhj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3smayonpo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrbshzy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kxvkulop.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wiscyhzm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzsxkro.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lcskgtwm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3sokajqpg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ejnybjmb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hbrnxbqx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ccojezsr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jwrlkkep.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3taxknoei.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rotyllkc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3aoldwnhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkdguvxh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cxwadenl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpavrnix.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iifutsxs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjujema.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bbrqbqtf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lftjdddj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fhkvnrkl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzeughqy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wylriuya.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yeuowmqi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfmaxfc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zgciljey.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lletytrg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fqvumaor.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ngrlqdcb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jfnnybim.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cthsuntf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mhxzlrno.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mnoevhlp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zpphrbzn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3aipdiamn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dwqworsp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mpqwnqgi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bruqhhej.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tloppptz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bpvewxwh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3souqppab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3aemawgcj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3odbxqozh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3szsecyxy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3palorjvq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qeubiqvd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dqqzkorr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pfullkui.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3galwwasn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nlveccjc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfclpmg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uckljwmo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ozukunvb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nemuvien.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wsfdeuca.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qufmkswd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kerwsopy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kjjviywh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3grhomnwq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lsozhlxa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwhotzds.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nqgurqao.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kkuxckik.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qlhkaxdp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ytsoppwc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lckowswo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ifsxdpem.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ccncwduy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3myoonxwl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lwgpxdpx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cwudwrzi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hsclqjrd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jpivymsy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3sygbuckd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rkwpludb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3iatdpvws.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ekmbsrki.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3amaglfeo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cnfohptp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fsmawhyy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bgstiuvw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3iawfuytv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zflrcpwj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xvgaolqg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xilxsvgs.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jvifpbvx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3sryqssat.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gvsylzye.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jhgnvdyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oqlqdzcg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pcoxikob.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cyqycxgu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ijyhvqpk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lkuesiew.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vyxkeobk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sdbhqfjj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ctvwnhcs.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3owirbunf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ddbvebxp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ykruzwxb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pjmjhzhl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wehlwtfc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zucnpzqj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ismafuyc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hvvsiung.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3exxsmhvn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tytljlnx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3sxwwkhej.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3olkrluls.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pwoukykn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jldwcmjk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ypqhjkol.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pxglnodh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xkroxsgm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3elgmkppc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rlkkflue.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gzkvlseo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cstwmjry.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jsbifmzn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vemdrvbe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jwxjridt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hwkdyyti.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3blbcfxqi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kcsfexsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llbxydwm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3osspbijd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlphxiek.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3kftuvles.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3risojbhc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3telyxorx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ldcnvdik.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3navhiamu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nlfwisyo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yfzmkgxk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3obzssvec.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wnoottzu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3roczufjy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3swplmibn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3cjqbivru.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tvdrjfib.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ufxkzcvo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3iiklkoku.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xffeiwtn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gglgrhql.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hazsquet.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jgvjidft.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jbprmviz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3idtmbmvv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pzustllu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3inrtkzsh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pbtlkarn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3payyqdut.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yydieacd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jipevnfe.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iqevkyaq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3tichdckk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3aimvubsh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3amkipnrf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rigrjekx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3reyuuzgl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3zkbarxvd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3lvctciyw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nokghytc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ogumhyph.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vdtvzzkf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gxmqacvu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dmgkkueq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pkwdnsdz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3pjncitci.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3iykqxuic.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3naagmanz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3pqpnqjzy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3otihultq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ryysblnb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jwvlarqh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oeolflwr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hawqsarw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ooalxdds.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fzxwdeol.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3fuurqkrx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tirjqxaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qewwfzym.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cyifawjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlycdaiz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nxmgwfws.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3budggzme.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wwbxwusu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zwytudbk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3syekfltz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3auxyogxp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3svnrknmb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xnsbgnpb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sfeyawia.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dijzxxeh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3olrvellh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3klpbkiil.html


<!-- 参考信息 -->