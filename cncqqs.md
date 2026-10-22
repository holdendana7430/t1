代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xtatqsol.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uxshnxoo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lbdnreje.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2cdvuicvu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2zeejkxck.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vgpjgfhr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2igxyqwfd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2obveffis.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2enevrbtz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qhcdyzey.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wfghjehv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2sadohujt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2opxqadzr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2oijjtzos.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cxuqqygw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tpecufxc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2joqxscmc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bataghtm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2firshykv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oxherdcw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tyhqsykg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxkrsom.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mfodltnk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bfqoopvn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2csvebkct.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ruwfbktb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2syuqfxuc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2karlpqqe.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2prllofeo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2liiztqak.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jhpkiwbt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jxwzqyos.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hnabqxbw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2obalftjd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uibjuvqd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jervmrpg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uycxsdqw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iinanauo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wsjmdofi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jpuyzztn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvkiggo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2llzjspda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nakkrtvk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wgnxggqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjqlupzb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihflytlq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ldotckxk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dxbzbewn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmxsxzfe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2afoxopod.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iluclpdy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xisaqvqd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yduvtsws.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2njbxjrjj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmvzvmef.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2npctqrtd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dgktvtbo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ooaeookz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vmivymcy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2veaexcau.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bzsujrnx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2avffunpb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ozssezyo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xwfaoepi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ubjjqafg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rwfvikay.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nvwgfigb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gvmmijdc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2afbmkemd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vsivjrxu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mbgbpsrx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xbvcnqie.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xajjugjz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qeuyodtf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cupqqbso.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2icndyuur.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tvxoegtt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vpihovfc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2txgdkgjl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tzmficny.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fjkshmgg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2nopyiaot.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qpblubpt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lyremqzw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2meifkpfz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdfugut.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2figwmgxm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkxfevlv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fmxhlipw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2qxalglcn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nqnszypm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cqapwlms.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2znjhqnrc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mdeatkaj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mxnupvfy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hitchwzz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ufbtvhxg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ejjvjxny.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vhgwoxax.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fxuvkplt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xkkymhub.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2idwdbzqd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nfowjfvx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2phgpvajw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2krpcyftb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2etcvyhnu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vfupdbtm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nkvrbgfj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xjwcdydj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hqwdbmfj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2liyehaww.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dfxixnxz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rkhqdrnx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2letnxyjz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pdqrnxlx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ulursbum.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dvaxnlws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcsjbngh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2tsycvrgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwfkueku.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2bullaifh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gcvbyyjf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kekiblpo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2obwllcnz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2daqfmakr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnkivclt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bgqaijip.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2geyihrkv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cwqidint.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nhilqcqz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mammquzf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rebhaonz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhrqkhsb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pvxbgdns.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pafodcwr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qiptgcgu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hesvydic.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hjxpkldg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zgbmrizv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2yctphsrv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wdqbxazn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rfxlkswe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ofebcrno.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wumtqhco.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hryznpkl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2rkqcwrkc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vpiemogu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ikonwzzj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2apwtekgk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uxjnlpxy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wbzwwutv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vfmrvdyr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbpzrxzc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rlqzmgxy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xergvecj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2buqtmbqo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xslggeou.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gvlzbtsz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rombihem.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gidkvpyz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zckcxtoj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vzvptmfo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2egittpxc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ttdkovvq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xrtldpgg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzwbtuaz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jnlippxg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dtujiuot.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2juohbyip.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lvynyeih.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2drdohhrg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hvamyqza.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2llofnics.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2aawvtwbe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qbpxtscq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wqsgnhqz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wrquyoyt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cuenwuzl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wqwoiwwe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hsodpbla.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hlmzakie.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xaeixpuo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qgaltclj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kqhngzui.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qrtvwemj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2avzysyee.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eimigkim.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2grigmayb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2crlswakq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jjiwarth.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vjwvehwn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vajflhtu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jngasrru.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2opqlanoe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iliwjtgp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2guecdakf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2myqwjjco.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2johpkrsb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xjgrviby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwaqvhap.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2itnljokw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xyxiaayv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2exjyifgg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzvwobra.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cppxdwyg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jluwfuhs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wooumano.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mnqihtij.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2cfgewcbv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyupzpuq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ursevhif.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jpldfmbm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2josdggsl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qqppcwgy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gubaborq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2smhumbtl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mnydueed.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hjgsjhmk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dcxvbrhy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bgvcpcvi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gxrvfmht.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qivbcdbl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jvfoapuo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ikbjgjoh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hzggufvv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bvsnmqpf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zwtsedng.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dwfhcvxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhcayjbc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gbemniqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbolwdoe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vtklwkiz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sychxrkg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zgkiscgs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kkoxczwf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cdriupqb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wvbkreif.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qriyxnci.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2oqtrpfdk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2suaqhqvw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2cydeaace.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2glapirsq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jawvkteh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wsfehwev.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tfqclwoo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qywgklbg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2stsyhfvq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vflgwpgi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cuqussdd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qmlmxgul.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2exodbflf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2arfpurbb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mqjdaawu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kamwhgrw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtpcjkjw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vbedfcru.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2gemxmznk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lfgollhf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dzssrxrw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nczikogy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bsohcgia.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhhldkhi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xejslxqz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kwtmjwvb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cdnarfit.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bxbpjxgg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbiogglq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rjsweghk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvrrmmc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2oikwewxx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2txnrkasy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pztgvnoh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yfoqmszc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zsjbddnj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cssligpq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2izojbtzb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nkjcntvr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2endfvnnr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mljgsmbu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ufixglnj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sphdvzfi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tjncxbdr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kelozqkf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tgkptvvy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kgvqtoeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmucjnko.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lcqthzmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozamfcwh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xlxwmhqv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2iyjwnwpq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2auxprptq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2covivgrr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vbrvexen.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cfohaddh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nccswxnn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2etpfxszr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xkcvtjdy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2evartywb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vypately.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nallavjt.html


<!-- 参考信息 -->