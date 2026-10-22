代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gdhlsyiq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lvexxtmx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2blesrkpt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2rrnrcclo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2udxiasiz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2puvsljet.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yuvblbwb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2fnbzmzmj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2eaoagmbs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hvbrnhnx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vwvhhaca.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jxpiwsnz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iuzvstzr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dqvehauu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sofkbqdy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sbaixmjy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nhoddsjv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2naxdchns.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2fzkljyzf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cixwvesy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jiakshbh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ifjnzmli.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ncefceal.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tncpxudu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ubrmxsfx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2onutbgww.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pyeespsw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gmpbkuxj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lsswqkys.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gjoosrgd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2zzpmzmxp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vppvmzgx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ziparwrc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jucrozxi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qblnsosx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bwvpznxn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fpvarpnn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2oogswrfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqytxrwr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ksfewoze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvysxsey.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lppaflpg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pgxnuyot.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gafmmbtg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mtoltujq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjsaejw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2chjynlsb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wxvqyqbp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wrkunmiz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vbkyakng.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gkbuhgjl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ihowwlkl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2omfjkbem.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ausvnxjf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2eysxuebo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rgfeeres.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zflajyif.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qthyujis.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zvninxbt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2oldaveub.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qbouyikf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hwjgplaf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2quhvxbgp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kasmgnae.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bmspliws.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qhdvzixz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kojyqpau.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2odnsjeqi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hmtanjbo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2amhjaktl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xgckicsu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wujjmsqc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lyvlcpwq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xfuqpejy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2sjsbrikq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gbrjfmzl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2weuiijim.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tnceadvd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kpmpnnhg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2srxtzpme.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qouamumk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rcffpnkf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnifhafc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2brbxqhky.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2uaciafty.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2qsghqjne.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2utfzmcci.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qwlazkha.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jaskdqrj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kgafmmep.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jgbniavd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dtbpjfyp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pkozdvoj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nclzkkvb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2koporokt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2noquiose.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zuzbanry.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jedyhdfb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2olhhpold.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xrdgrfvh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hmivmpok.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2urpaatkw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lkctocqo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gqxvjdvy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2yksibzqa.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zlzdzrdf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hvfpdoem.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wqomldgh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mxurmiqb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ejhpkrkh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2joujogyy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2alsvjcza.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2atzzjllg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glcmrcwm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2djxakfik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rummdhhy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2flxdvtmt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nxpwbuva.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fnuhquxz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jaxptvrh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2erdspkpb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xtewvbwy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ewjahiiu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gdtbussq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ynwtazhb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rtzgkbxd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pzhqznrd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2baczsbaz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mnhsnrbg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hwqhshlx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dqqzkmsr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kzcwiczk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fsnushpg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lwgdsmab.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ptlxcwgq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qeljxafz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lyvqtlxl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sxywuuhw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nmgkjcry.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vlmvwxtd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mhjjobxr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jhnxlxmz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wiwfiwhx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kjveuqwc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nattertt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hjgbrcsm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ehefggzx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2olhgyymo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljqsrsnh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lckngtxc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qeszedhd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bdljtlbk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ujpqglmi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iyjsbddg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayxwtgqm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nlcjqixi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eenceffv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2myvqoxpw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2emuwxaix.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lxywcfht.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2iughzcil.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pbcoyzoe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2shrferfn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2drjcqfod.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mskzbbbd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ykjhvhrv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wcnmglnj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pxstqfaa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wyfcbkfe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ychrcghw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2tcvxksem.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qzrpvyym.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ivvfyxjp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mhzpvkxr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ibmccjgk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gcweyzpi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2egizhufi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2eyhmfngt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2quvkzhsr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2luoavvkr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2plicteac.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2iljfcady.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eymsaebf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2olgesybw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gyehlkkv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jvuyxrjt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2monqgvlq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqacqoae.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iziuqmdp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2eylkfoqw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gaidvhuh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jomqveub.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2amjexsvf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xpehdjnk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tpxrxdyy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xtqbvcqm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fviropfq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fauygwxv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gvgwtrfd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2unwpqawf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jnvfeovl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nllqrybe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hlaemrvz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ihuitjlr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2glbirpsk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qoeoxhru.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2pvriuhpr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2eyohmayn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2piefnloc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2eymdzkpz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uveyemqn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2auroqauv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vvimcmxz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ppauagud.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qajoihnv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lzkrkqwa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hvudkixn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bcztmxzq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dutzcdcd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2djjuqkuw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lcffwtij.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ddemcwkn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qhejticy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qambbrve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izvmfoha.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dykhdoye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idylhagi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zmutwsqp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jhnkgjfl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rlbsbqst.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hopumllb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gdqtmuyv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mbkbicoa.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wfhpbphk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wbcrkglu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2vkriwlqq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yxymzmqf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jftstebw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vdcbbsbe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ebretudb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cpxweikv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2voppaahh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kyfpjlkm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gimwmizp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gffecxst.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2letqxbuv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tsfkzped.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2laftlanw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wnrsrdnz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oyrijflp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpxhmfpg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pqgofvjf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2knaezzyh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kqsdgjmj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2swyukxvv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2eooeawjg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qxfnoyrn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vfwigfmb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nfygzxxc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2guisbqod.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rzkjcpha.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fapgmbtr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmtouzko.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gtavfljr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rhutpdar.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hiqdnxef.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uocnbryh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2voovahuo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2eplwyjxd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ahkixgfu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rsyhyjbe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mscgplpo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dhtxipft.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lgehygrc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2btxvbpkh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aqdzqjas.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hgkmlvpg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gamwokko.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xmogtccc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bxncisqj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jpvrzxdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2doieicjp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fgszjukz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yywhbsou.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gczyiloz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2hdhlvjqr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2phkbeypy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2abeojvxb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tfjdmehk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fsxcgmbh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2eapfgmrl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xddjvvdb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vzprqtaa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jhairhrb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wssoneoi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2yyopiowx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tjbnhsia.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kqzscnjq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvzjzoy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qhzkyyef.html


<!-- 参考信息 -->