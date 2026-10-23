代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qahtmkoa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vnnwmccj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qvcmmpkb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ufkegftt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3olqeywlm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ahuvuopm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjwxgvll.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3cpxbtaho.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nfxbjrtm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3oxlvejye.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mrbfdxid.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3msaylxgg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mxhvgmxz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kegbcbzg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rzxkxumz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gltjhtiw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vbgoqvzc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mswdoxpy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ycsruvtg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3thwzklbc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gxeikjlb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3sbodktga.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tsxigwyq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dwqoytal.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3eysmgfyj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ekglpmch.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3iwneanot.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dinscrgg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3latiecma.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uihbskpz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jgoyqakx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nkxagves.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sumdmava.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ayxzxhtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrulhbcf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3atnffqgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsxsaheg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3brqgdbxb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3uhbiucsu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ljjhcput.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eizjdytp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3srknlszj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lypvsued.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yfynxsco.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xrljmaom.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cfoapwxf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dopkqyar.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gucotzrb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ineugoph.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iqqkxqat.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3izizhvyg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3byojzzet.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tvksxxru.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wfqnqtrh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hwoooyyc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tnatbzuz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bgusdlzt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qgjkkdeh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ggjvxxod.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wksebojv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3akojwxfc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wxkkvqhb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3efedkwzw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3goeepuiv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zlzbkidh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lwlnhhtv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tzivgzvo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gpyxvxfl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ivydihlb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rkrunatl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rfeanwbp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jyiwhnxq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yeoysyap.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yysdcldc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqdjbtrw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fnzwpelt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qjwmowbr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ioaifdfc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3akkrxaee.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3juohnusk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nmfgllce.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xrglzmhv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nrdlnkra.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vknrqsdj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cthulvod.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vzwaakyb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3daipmeer.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tftkbunl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wjaxycij.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mzctkitz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mczdcudq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xtdjmayd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3akqextkp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ytrqknmc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gmgrgmdy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kmrwcbjq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qucdhpcv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xvmsdwiu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3teqwwfzs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3strntgwa.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qjzrjiyy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zzazyava.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3szoqqxjw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dqmgomif.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wskelqqw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wxothrxw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kpamovoy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uxinoddy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mteywcdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsbqjjel.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ieoupqvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shqawhpv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3vjnbciuy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qprbxixk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3omcaqqcz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lorugtzn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eidhweys.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nndzjdtx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcolyjlz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3srxjiqzu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lnyekcfh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zzzqdxyq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tnnitaix.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwsfotm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jrynpnig.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ruontqxp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mlgmmjtk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzggaxsk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tcoinojm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gvoryzob.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yenogfik.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3uzybpbgq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lbqhuqte.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ufbrlexc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lidfpwts.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jixarppf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uojugcst.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wqjcjpuy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3atgsuumt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xdhomidg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzpdutob.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jehbcbkz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aadibxfi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3trdaeokr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3weirxxsi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ibxxwlpi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvzqdjv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vavtgauc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3seekzawr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sggubkfw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vwqchrdm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rrtzxctx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eescmmzi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3yuczpyen.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rlymwjvo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwjvbjk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3grzjzqhn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bdpdykev.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ylsyueiy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nhoptefq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lehdbgjf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pkhrjckz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3udlsydrz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yelomjem.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kncujqsj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3risasrha.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kxvevjxt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lxnsavfy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dhzngjee.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bttljouy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gghzgpbh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jsuldrmy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nfhbdybn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uutmvmol.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nxhfevyq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xxbwvkrh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jueylifa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zeqauvsd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fyaawtin.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aymlazap.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qyfoukpe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gwqqbvim.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ftdugxqw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iotcwzgt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3chlyprtr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ywggzehd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3adwwlwdi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpkkozlz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wrfjtpay.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nophzqaq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3bhkufrqn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nurnrxcp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bkpmkvik.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3nocittgm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jzconrbj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3myjuwjxu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxwvvmp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wzydvfop.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3htypzwcz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hzfzofxs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lrcfzshx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbrkkqjz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qahmbbql.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xfqpwhno.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tfpnpesg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cqjjqtiq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eaubsfwi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mkqgnxbu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lolrulfw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ajriwquq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mwczdzes.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3puabkqag.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dljdomwc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3djyjltsc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3unjbwnjx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bnrjxwqz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lnuuqtfq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tiwejfzh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xljjchmn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pnjulbbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbhnxqvc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zklewrvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plszpgav.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zkgmtjtb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3afqmqqku.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3adfquifr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rofrpxoz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3atrzeakz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3iezpaevd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3edassfin.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qxlhteee.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rkccqqvk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gpvmvzzl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pndahxce.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ifdxhwed.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3amyxwgre.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bjbtlpgx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3hovczlkw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pmstmfbm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tvjjxwoc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zzpzkbdg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3yfhklwtv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymhfroau.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fxmtojol.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3enefmjcy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pyvwjipp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggfdsbcv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mxllwgqs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ujvdcmeo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gjigrddb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aubbybpo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3dnahbuwo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vcwioyft.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqvozbrt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrmwqvxl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3clvhwwci.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3iunbdrpm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hmrdolot.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqmopmip.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nuwbklxi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fnxikftl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cdtzapbt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rspjaodf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3efywxcij.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3bvrqbeuo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3znbanezj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hbdbkvlc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mumarmcc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zqvnxaij.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3irrdxjqo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jzqvrzhr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ehglgziw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ubjozahi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yggahprp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3spuwtazd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3givlzcrb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wmpgrbpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nghbtjkh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3oflpaals.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqawvccl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lxneckev.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ipbxzmby.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vhpbpnge.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sykmvpxy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nimkvjin.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kzuvcpag.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3drsmmvqh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kksqvmku.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pgtavjks.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fgkxiupz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vwmuzqxe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vnfxpxyj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xiqivkzf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vgkecdms.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fgpvlquy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3flhjgxjs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gyslicpz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3uhducryg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uummlnmi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cxndlowr.html


<!-- 参考信息 -->