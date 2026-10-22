代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rdahdhyx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zehuxgqq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jvnfnanm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2igikznrf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxzcepno.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wsukykkx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zxnspdwy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2eryxwmkc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rzfuzimj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jqaperki.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2njkvnszb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2cbioswkl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xcdpgxlx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ydkczaxs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2urzsivjt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qaqmynah.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ctsvxpqm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rtstnqla.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tdgwovjg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bclrwbmi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jofwfzdu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wgyjxbbs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2etuexied.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2drednkwr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vkklimoh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dcllzfyh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2uwqxfsty.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vaxdeyyy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pgutswdn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kuzbmkmt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ffgizzqu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2azxjcooo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pztivgse.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zqtnvnpo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jglyazms.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jqqnilbo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gjixuhwk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lmjnicfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfflskuf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vkkmoamt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntirozyj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qsijsqao.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sitmhnsc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fdpiocet.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2syzgaknq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zioeadoa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dtheaxfj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ztdzaybf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tvvygrmv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bvygqbtk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2stitecmq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2swnsblnv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xfqnauff.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mnzbtceh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cylgkjep.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jvcdboan.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2njxdydjs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gcgsykrl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cofgltsp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tvgotpzi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pibmsixo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2sbxnsghj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mmsquujh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sbeoaimr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2npbbvndq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2twriechr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lbcfzdkr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mjihwkze.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mdaqekhz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ynpjrwwo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2akqmxkci.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aqclkqxb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nvdfcgaq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dreokajh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2agkzvdrb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xxhkvhgv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kravrndv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2axlwrnzx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmdwpgbv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jdazkznw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2knzekhab.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzvsiynw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sbstyrfh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2grilurpi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bzrnvhyx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rbwjmtfd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ovqzbmpv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2esaypsyj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fbsdkhob.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ppujhlew.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cwzsfuip.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2khdqvtbe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hknsmpnr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cyxbbmrs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cpddkxsq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kicgmuyp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2emtczypv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ciuijmqs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2upwzdvoj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fsbzbaxc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cyjnzgio.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rjggekqj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vdgwkzhp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sobzktkf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xenzvsqk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2octrpemy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2iaijuwer.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ucyjhiji.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fpupwqtz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vvorhagr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zyzslkga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vpfixafn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ppaootmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hootejbd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jbjuktiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrvtpaif.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tpwqmadc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrnfmvqy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2glcqqbqr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rabjobxa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hspdmtnz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qveffbps.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2opevsctg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xafmvqyg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzoqtjgw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2gfxynkyu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xlagpcay.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jaqlmyqp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zrgewpjh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2glimgzht.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vzvdvmxy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kdycwsuc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hkjourva.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pophioms.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bnkpjrwa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jsemerch.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xfpnluuj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bkksgxwc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sdpnpkwz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rmocvqep.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2edolblvb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dylmwbmy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bjdithke.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2yewnvxqa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dquqhulm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ezveakcy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2futnevpd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jtinhhxy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogbwjqno.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ggvjfcpp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2shbfzkfy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hwgolsuy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nkzeadqg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tjuxvkrg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wbxumlwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tjxtdwjd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2shtujnvm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xncphvdz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2blruyelu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubsxkjcs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vvrrezsf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jgrdldno.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yybnxhqs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jwpsnbpk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hnsgvvlj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gtdjpkud.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bdtxserw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2cnwpbsor.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zbgoslis.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2svwgurde.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kravzmow.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2crkgzbva.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2blwpzjsa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qtkfvzvs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ptgbuurr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2turohcqi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ectdhflr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wjzhmztp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lhnujlyu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lhafshqf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkyriqn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lujiufko.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rxmqdkwo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kwmuuqgl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gqtegndt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ndkyrldx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ueihcapy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eglkwymo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2irdpflwq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iqxiwquw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sjmidurz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpgvwbpd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tsrlwxly.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bgaorqtk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mdxlgrlc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pezoqgka.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yskulooj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ctffkctj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2szbjgwhw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuuveaue.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mavmqzlg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wprmtcto.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2iagotimt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2uyjgpkpb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2idfvtxkd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgjdkypk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ntwwskvn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2navfxjct.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rhazsurj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2khxaeizh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ahefnycj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2usmjgqrr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tomjjkha.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ollnclcq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uummyvws.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lfkmktha.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qjjkbeby.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2pilbbdvn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sfhivxow.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2aksjabaz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xpuykbqg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vuudvzkv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ctwmtjbk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ykdaesel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyukrxwz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2erexgnpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqkchrzl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2luuonfwb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vulzwzdp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xlrqpkhn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2habzdqqs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hwropbpg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jzajyuvf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kmkdunsp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2iyrrbylj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2cedznwyh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ggpiiwbx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2nbvyknca.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vbfznnap.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sylladtf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uslwrqny.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2luzeiirp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vlitzsux.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qgaxycit.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xdmyslky.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2annjcvrc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ludqepty.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gdtdhrua.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mqwzbfby.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qhimhmuh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzrmwsll.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2grixsvpp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2gqicqwsp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cpdbgcvr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dsfuzjxy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jzxdvxih.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wlhrskkg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2receeabu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2colhiwhy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ndaqkmlq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mslqpdnt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kaaxnjxm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gvwgysxh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sdxrmxfu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2noxiaisj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wbggzesh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2avfzakqj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xsjunoft.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jwlhmure.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ajehglbf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2umjxbzvz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2uoghoxfn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bzrxrkqe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qpnvehko.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mmsbfkdj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bqjeogtk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2souvmtmm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2yzfpgysx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wihzyqma.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ihtbwhlj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2utzdddxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veiwtrjt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2yiyajmyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dszuckto.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pnrgxpdl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2aomdfwel.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gitipklk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bjvrivrm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2egcauvfl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2flenxybi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2muzkuksd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bjrhabsj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mjflywrw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mrkrpdjh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2xquoalmq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mfgzogqi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kdmgwwyw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xhqboufz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ajkqelpk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cwlxzvuu.html


<!-- 参考信息 -->