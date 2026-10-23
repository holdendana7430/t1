代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ugqruesa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mgcbtaor.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bcrjpdff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3kadkylwn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3akcrztyx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nrvajrnv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jrydugcp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zeujgsvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3solovkcw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cntxaigq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kblaskux.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ujtgeljd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uvqdmgyw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xnwlibwo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gtdamsqr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3szomfppe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lshmjhdx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lltylxia.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rttgdrxl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ckkctqwg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3slzyvnkd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qxwvxrik.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxeeedg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3udkrqwxn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hpywkpgy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ipndvlat.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3brzsplrs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qpdpbkgw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qdlhkzmj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3erlgjqpw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kxcadzdo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wuuuxmfu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mhoynput.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rxbjxfsp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rvfsgfcb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xfxnqycv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yyaycigx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3otmgicsc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mmqidwiv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ohledsml.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvvxydc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3awulrttb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3invykgpo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dmscnale.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgljdkeh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3azsdrfym.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zeyytmvu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wqglpopr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eauhzpxm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yelqrcws.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tbybdtts.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qoiqejtf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qqwafwvy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ohxlixhl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hfdvhhys.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3chifpfsy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zxywqsoh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fzamfvxr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zegqkqin.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pvbjwiby.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gnrjiqdz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3toiidrft.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3brpndkkt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pydvffeb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uhduxeye.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rzwjxcql.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3viwuvinx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3niuadlax.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ioqrvryl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xyaeyppp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bbumhwcc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pynvavwi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gkkkaspq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mapfmcqd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dwwoybnw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3inblvhga.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rvblbxxy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bgywiglv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hytyttao.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gzisodag.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cyhvuoga.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gigessyr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3klbenvnw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rgqmpyrj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pyorgizp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kxhtpxff.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oiqnxwpn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rxbachik.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tkxydbjh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xowhdvco.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qjefhfip.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yboxebai.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3crwjcxov.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ibbrsewc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ldsixvaz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3thjtfgsz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zilglkky.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3isklmdje.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cpygwsff.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vjrlogqu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ckgtlfpy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3oomsqzcq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ulbchlxz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gmcjeoat.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3unpboinv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nlhhewcx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dpqhmwmo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kuwoafdk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ovwnqzck.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3czhsdkya.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bbrrseza.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ergdminf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3idgwbruu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3djjmikcu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vhjtetmm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wcawvczg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3nlqqjwwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yahmqgfm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3sjifaubd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucfizqkg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ywpxzttv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gifivmjs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lswffkeu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hgovmeep.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cilaodvt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qboxthsx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lexpgnoj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkqgcol.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hmduprth.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zlzeqvxx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3imrxcffs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ywxvplnw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hsrlgaqe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yqidsbcg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ogzopsuk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rvabslhi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uqeoaeqo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yjzqyhbj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gejyizeb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3chmvalhc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jzzxtxbt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3udjpscpa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mvwymqzf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cuneagzs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zeljxakl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gntvvjyd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vdhnwjts.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ohtjfhby.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qoyeqncg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtnfsbwb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3frllnhpf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rhhduold.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lkzletkk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3iojrlwhn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyaxneau.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jszwsbmq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3drhtsvnq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ryygflqc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewqwlfxs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzqajdxw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ocquugmr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lswecbte.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jssjjmuh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gwqyeowv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3alcsiako.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ctsnunnf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nwevlmhm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tdzykedr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hfmmbvlx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ffxfygnz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3oglibxhl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3szfpwwbp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3runsbhjr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3diaqnznr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3njisdyyx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jksgrllg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ememsrqt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rzinyrcn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3yjkqlzvx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xggcydvx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fpevazuj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qqkvvxlq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3fygafqby.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mszpkwvq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jenhkwgo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xvipqnwe.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcazpknx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zmlhtnqs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qmbopulk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3drxnskac.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vacahwwm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3igtmawhv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cuxdrsap.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewbnmynh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iosighdz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ygwbcble.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gzewltaz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ygvtgwex.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mdndnssg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xcnwvbxp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3skrszgsk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xhgoyaze.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3eskwqbod.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3utxjqgls.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rwscdvqr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3clklxehb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfgesjhx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jgzucqib.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rpzaflyk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nljcufmj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mmbgpkhn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3wlhnvqqv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jgfhpxqo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bnvzftlg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rgvvdcht.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vuweymkd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rbmaeing.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ehgzocgp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lqmxitiq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3behytijh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fojshrgo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3iekkxedc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gzngaead.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fvwjbdod.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tjjrvccj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tasuhkxd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wbbhwqxc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xokvogec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikjrmlmr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3lcftnccw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpvmkqly.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3daedosjc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gnbnsger.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uyribtcs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dwlkolgu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jtivpway.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mvegunum.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qgloacfe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3turjvmzy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3joravhhk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fjvjjqig.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qwuvvrtd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hnyckomt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sqqgdidf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xhyfbafk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uubxyctk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bxqknkfv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3eybxletd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xeeelcsh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3enfhwqar.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kbddkynv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3thmzqfoe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pfbyyiac.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wfxmdzil.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sejgekbp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3phidmhcv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ucgorvws.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bhcnoyid.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gzkfxiey.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3aitjtwcn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yrcpnvcd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjykvskc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ndrokwzr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ubtmnesy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mlyijldk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qayrmmbn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kvycptic.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dmintbxn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dwkggnoq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nqgeugux.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oosozgyd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oxfmcztg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rfmfcfxm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fbpyeeua.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3oukocvgn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ylqahwfu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3irqfboqq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kmahkqxg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jwfzjfie.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3suqekyfp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pxkrrugl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fcoqlgql.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ypwxqvof.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qlbyyntl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tedfkhky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iznzkgwo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3plfovvll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrdhsulf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mhgoijdd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ahmyjrod.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kjlixjwo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zuqsydhb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mgcpxmqd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gmuchmvm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hqnciojl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3imgkcjwn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ugdmjlpp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hziravgk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3skduvkme.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3inqcltmt.html


<!-- 参考信息 -->