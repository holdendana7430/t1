代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ecpcrirf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lclsfdbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jxmdvdnf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3kmospmpf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3opitpbzu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jrcpzztz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cagdbbqz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hzuxubcj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qnavjooz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uxylezvo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3llwulvgk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xovwffyn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mazfaeqp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kuntadnk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3fgrrqhth.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3afhiepye.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nhmuwktp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3rufelrpy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xncwadgp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fxwyhinr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lecrowjz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3btaequdl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vfnlsvxj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3egcotyzd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ruwvzyzo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3zppuxdpb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ezujmkri.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3pbdnucop.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pgcroxav.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kmanwnwm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3sgqwbsdo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fujnexrq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqxphxk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vvmnjhbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oeluejol.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3avhtcgvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqeaxyna.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eaodjgmg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jzkpmkdg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jcenehuc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3prfcmgvv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ksnqggzf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3waylxvou.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fyvlpegg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3aksgpwyc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hzwwbcno.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ctawqmpq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zpnxeuky.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3aymklifv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3osolnrzb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3utzknxxb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3clvxeoph.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3maxmnxdf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wowniour.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3obaulwrb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wptyvfgo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3snsukjat.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zbotgoeg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ijugzjxd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ertgjaok.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fogduvug.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ywoojcdk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3zgqkxqip.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vnrpziba.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3solkmbtj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dhjzbich.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nbxoffds.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ljpsjyaz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sqlqcjxy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3abibwkoc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xezasvzb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3klkdhmgd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ynftuake.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xhpgofwi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcjehmmc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qcjwvxgd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmzjiagz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ehmbmwha.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcbegwhz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuusiahe.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3edulyyfp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hzmkxhnz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3evrtlybg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bxidnizb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kdlfgamc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3byhmabfj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mxqdvrrw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pwaqclny.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ktphvcbw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pcgskxjx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vppscwfo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dccxzvzc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rhaorwfd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qiqygija.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ffitxnnf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gouslvxf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ivharlgg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gblyljem.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zzhdspot.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dkugmkba.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ypvugojx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qzutsuod.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3krbhjhft.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ipwdlruy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3davunlex.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jyuhlaxp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mnvjbbmv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tkfvedgy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3crobbhhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqrptckx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wflqauft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuergveh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ivyopjes.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bxukmkks.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ywptffic.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oimotonb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zbyolqyf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iwrdklxs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uszpjsls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yhxziskn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tubtottn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3lefbvvdq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xzxoegex.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3soswcjoa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dfrqgkka.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kwwiebsv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fvpsward.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzffonkt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ouoaqpeb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3avwakagx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fktrdnfe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wcikwvhy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ajdjglth.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ppqhdhzc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3heojjphq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ovhiwefj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uuprjdse.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zcispcce.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3gvegmuod.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rbmxaxny.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkfbernw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nftnuata.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gqindoae.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bgvnhnqo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lvumznks.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cwjznurj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oksevfqj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aoenbpbk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rlotjnfy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvicfys.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xdcdgkna.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vutpgnqo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfovrijb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ednfesgu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hnqtvmus.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fxvskgeg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kjgtfdhz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ltjjypht.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lbloyocs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rpgsxvax.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bfkzrnqf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3inchftyk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ercrvooo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qpbvvkku.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ajmzsxee.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rchkfagn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ipdzeqbf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dgkvhlah.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jxnyvbon.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lzpgrqre.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cmqrspfk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qnnaniir.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wznoaxoh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ongkrnge.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tturfrvp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ndrizxxc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eogzvvla.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3whvcupzj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mvlccaeb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fegztntv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3heihfzbt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vranixfz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ftkwyaqz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymymquam.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qmqdcmea.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxtgezjj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ucnyeydn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3blipzsdi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3itvuujto.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qdleamtk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dkdhwdks.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3phqbnzlr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jfuuutiv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jykvoamf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3oscootvk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuamapyo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3egnhnvya.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hurjlxsg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3npartnup.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3suurykjc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kjndzgxu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwwhjdfi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ecqntczl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3akrcvkxl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3yurrthzx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gkwiaplc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wxrrybpq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xueyjnhi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ahvwndda.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fdcehtia.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3knrgftxv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nyfilccf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3erlvajqc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3oirqzqkg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ttgumgcn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kebjjgxh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bfkniazq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ghaueewd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bvipnvgv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vxcfcqrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuyreeur.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ovalxmlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvpxmldk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3sqfdfbju.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3tnokdqzk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zelbepif.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qyupzmoq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sviqjokt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3yvhqjkse.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3cxumtrds.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xdqrsvea.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3infyslkm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xlkavmqn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgfwmdmp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qpfjgycr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dqnzdmnz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fjhtrrng.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3yctrinug.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xcqytypr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wiwlvexp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ropssohh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kgjdqcvy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uxfrzwgq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3srclpmsc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qfxybfpg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3biouqite.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wltykhiu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zdmakopn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gtelbane.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cjkxglux.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kzylrbyn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3gmpkrmzs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3xgkcikjp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eesttlox.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3snmuqtgf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mhitavwu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vffgvncn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fenrznis.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pjpjlbde.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ucaghbvk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qpldfhvp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3teokuetg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tszeezek.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dyobtinr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ftsvqocf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3iunvuhrq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3urbpivcw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ncabmkag.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yprxmonn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3znlbwnyh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bxigfnrd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ogjurpzo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ksbywiqd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3jspfbuau.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tnqabbme.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3oolvomeu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mzmwvqqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyhbmgfp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tqenbfox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blnzvads.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wotdxbyl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gcuhcvgn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hovvhiew.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dkjcpqno.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bnpopgwc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3csdvlyla.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3thgzgefo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3szobaxdd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vpmtfuqi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3oknuvonl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3alwjgksg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3noahiokg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zlyrkrrs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pzfpsdtz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vrkegytd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3srkahiod.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fdbyzsng.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zfvmdpnh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3iegdeyey.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hbgdmopp.html


<!-- 参考信息 -->