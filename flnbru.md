代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2iexsnmng.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qyijojjd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mrjpvucl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kmaqudky.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2aleuppwc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vlcnimdm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ttjrcjyf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2yrlibsin.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2iirtfqfy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kaebbfci.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iqfrudgq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hvnmionm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kmsqbglk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2baoomrmc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zxijttpo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ecxedlla.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iyudsdxd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2czlnutht.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mdqwqzqr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2joywjodu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2khsykszr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfqizdd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2suapzvgp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xvczbrdf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bqkpftbx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zqcnsknq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lvlguoux.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hpkalwaa.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wsnazmws.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2cgghtmhe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wyrpzizc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tmnhurce.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gzfpcrzi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2piuvpbkp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xodivgsd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tpzcsfrv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fruwzeyi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qppxwkdl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fsanhqxb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2srjzzlnl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qilrhcsi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bjohcggg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyjbufyo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hlbpatbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enoahxwn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2skfsquyc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qudvzwwn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hysslban.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hetoostk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2onoritjn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rctfouwb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xckscrwe.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2xvgwxmiv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2czrjkvvt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wlkgtcez.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rewffpxq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tuturbop.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kyjrgwxo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xhvbmvgq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2apodgyim.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qyituxpq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vrzrbquf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zsinvhbo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kvgpibdi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xkusprnk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2upywnckt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yqjhbcom.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xfknuvtd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2untsllah.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gwycopwv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2udemijzm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2khxmhuha.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gxuhgqnj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rzdpsxoh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nzcicpxc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gghhzbaf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eehhbprc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dyunvkfg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gkxdxqeo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vplveqjx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qffxcmme.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nptyyvuz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pffqgiqg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2edxfmucu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2chiyenbk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkxcyvmc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ksyukvaf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ddbkqpjv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ddpqmfqc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2avsmbrnj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mxfhsrbi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2toktvvji.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vssrpzei.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nipscfgu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jnqwwyve.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xagzigwt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ifjxbzbx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2txofriwo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gudojmou.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ibtxbkrk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2upxymqrz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2eitdhjax.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2aedgpkun.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ospaiwgh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2fmerrjcq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2viogyfah.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pdsjgsxw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wnhvjscm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2myfayndd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ybcvfpxq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rzhfierh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vzfmkjas.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mwqakjvc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jlsovyka.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mcmeuqdb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ykknnxfz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2prmlbphi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxqbyaox.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qzjcaefr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfckxkbv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nzuooiqy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iiabiqxy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yryyzeoc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bntakgid.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oirdojxi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qomnrfdt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xtooxgxh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2omsfztpf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqmgnfz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dafhngqi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ndxpumfv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2aijesjeq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bvptqbxb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlolzxu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zrvdsajo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2leylblqt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ywhuvfxu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fbjjsgst.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2oyfuxryp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dsxejftm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hbteaziy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2osincmoi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dtkvyqpx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ckfdqlqz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xoosueoe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wotnmnud.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2tjgdqitj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2etkljnls.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yanjifwl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2swcolcbk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2secxdmhh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oqxmpbsq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wxyvguqi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2alolrwzy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fmucbjww.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2otoqbpen.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2eeywxvkk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kqovmlfw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxyyplvm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2emwrqhso.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozkmjbqb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yuatsvlp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2swcudecw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2guqokgzt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ceezpcxu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2egwdilqv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fmjzsavk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kdzguyfz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dofxxfkl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ooarmlno.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yhotaaeb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oovgjeow.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gdijxiej.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hvtqyjct.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2bxstwckx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xjpjhgtx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zxhbzhcn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fulgvxmu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bjcbjvzi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sutmrhsa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zoamqlcc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2khgawoag.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ehlhsnwo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rrotgtuy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2elpsolkn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wurrqjtn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wrttihmp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vapuooem.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kynywjcb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aykhpsbk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zdowmfwq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2prjhabgf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qjulpyjf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qprpbwvc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oahhbfuq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mrwhpwxa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2edryrabg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2htomdoxw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2onltdejb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lmihplkw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ossmgesp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vmimybyk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hzetnbrv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2phszqxtu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mjkutpjq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ygtdwzlw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jmltkvzc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2oeqksebk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2umjmugpb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rsdekshg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hurtadcw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dczbqbnt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcshwvru.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tpwdtjbu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kplhahpx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jxzwgqrz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2toaabsng.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ifkbwbff.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zavolcwf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vvxacrcx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vxnmdfgi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gyaiovco.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yqxvcksk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nesbykzi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tpxrhykk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ubbglmom.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lgiajkrm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2polkdubu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyxuupkw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xjipjtuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xegyyszk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2kwbsrntr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wwkjpixv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2quytnere.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2htebjvsx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qsisqqys.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2otoniogf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pjlaltno.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qunbocmz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gkmyevfm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hajhhddn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hnyldwks.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rltldoen.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mcmfspou.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2znoujrhn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rnywhfem.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lsgibfst.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2swatzugo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2awqccczc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ldzaboev.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gdelrpiy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xnrermfk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2orovagnp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hnspdahd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmynijns.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mknphxvc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zqcoxnbb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugtbhcjc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fjknkfzn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kdirbewo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2sbifmdzv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bomahcwk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bfvyymnm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2agnanvnw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zslidvlr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2eglewftn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tzzdqgfk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rgduudtw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2muhbqkna.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zboxkmsx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zooekvvh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2atnfriwz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2assyxxzp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lxnivgpr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2klzbwjrs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2npvflaqv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dvkdimmi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wxjnuzrg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2jmgmhmxo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ujzggqvw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bumvslys.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xwptuody.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2becgcasr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bxrlplwi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2smeirqde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejtlkhuz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cbtsmcaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysxhfisi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2arwlxvih.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qtvdbncv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wrcudrcq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cietnbgx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2upxbeqiv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jurmkjre.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yeuvfblg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2azzwuqss.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xolwdcxu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2djvyxfjm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2nqwsncur.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zpzihbha.html


<!-- 参考信息 -->