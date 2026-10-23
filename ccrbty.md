代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3owgvsfbg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zzljglbi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stjmtdqt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nheawhvn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lmndlrjf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ssshvjth.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dxtsosdq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rayrodfy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vdjbakai.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3amvmvsjt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qojcxrsf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nnagckem.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xwitkpor.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3whflihch.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3niaofvxl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lmymqfor.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wszmkhlg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ldlbzmac.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zufwxbnz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xvuaclcj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gxvmivzy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xcscazqg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3itaicrni.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mfimztag.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vycjtsfw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ncsgnxce.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3fvdpnjrr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cejeyuax.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3saldeuir.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qhnjmlwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phmavlaz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qywvjuaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bafkvhqq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3enhvxytx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3dunzqvtg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vsjeaosc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fghtsiwm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nfbdgstu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zstomuft.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wkvfenex.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wwqmguyp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fjmxoxna.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3spzvgdfx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hyzyvvcq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rnmbzxlz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qrdpndci.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cmgnirdx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fseqdhtk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ewuvdoqo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kjoxpfni.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gmxeeoqt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3aanhoruc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mgujodah.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3egylfbfu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ayvbtzbk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3baipcgbg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bzrzftkq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jnpghgiu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dygrgvmk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ekxlrbnt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ozuaxqur.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bahjtfni.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ejtjemmn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3otticsgv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uevdkyqr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jzskulqd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qceagiqj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3idzqjxib.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3kqjentrl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3endepder.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fcgkfiad.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3csaistlf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdcykzla.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nbcdbepy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mmsvtjuo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ixakwtyx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3opmoazui.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3phrmxkkq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mqzdofnx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ldvgzwzo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tieyutcw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3azbqxtbn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xqbvrbio.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qzgyktie.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wahscpgs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bsgpmfkw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kerybmjo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kfnmcfow.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nsxdbfbr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3sjcbnriu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rpayjegv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ppjfmffx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mtchgwlb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3btulfebi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ltduxgez.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qrccpysz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qotiadlo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vubereyw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3eeszbsfv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fcadlzce.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vwnbnoqq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3foembopp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ijhxqncd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vxecemim.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3yzcqftxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtkdhlct.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3texvrrfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ienygorn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rbhvxsfa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wsekqncb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3swxdgkgi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xyffxkxc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ffyquega.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aphpelgu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nudpuivj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3cjsqfqaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptieqzvd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zzvokjbx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zqybytpn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mxveptic.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ghtxuotv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tdaxxgxq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3neaktvaf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxiosoq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wrygqltv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hdbqrhbn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vonzhrnk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fgweedyt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3btbvvqcp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fvwpdenj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ykyjaeqx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wkqcfnot.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zniedsbt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hfgcivee.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dzfjhiwt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vwboznbv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fxlzukln.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uweunbpo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wzpiisua.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qethmkas.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lxodxwhi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3aabudoms.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fogsgtpv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qpdfwzri.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gwpbvelc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pflukxwu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuiuzwgp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eppeuldd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qewldari.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mtmcyyfk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3whqjlija.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zubnjxuk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwwakdna.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uyjyevoe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pypnjnbr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3duovluqe.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hhbmuphx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jfdqipjc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pmrfgwcw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3oukpuacz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3izbcetny.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tiatymqj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3epoqofol.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mowdsgbt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xfjmhhks.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hsuafsyj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nzkpudvj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cminqlsk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3bpbxcgkv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3yrkbvmlp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3updsorow.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ggtmxnzx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ikmxhjvx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xcyybbqs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3znpczwrl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hmfrmslz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gpyvbmud.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yclzwsrx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3punbhoey.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxrschnz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xkikjhrv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tyxnajfs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ktvqbheg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3npftbplb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ibddkofc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dtudzdug.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zfrhqsnc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3belipwfy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gwjtlhbh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hxlidmdv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ahvbbczh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dgvohjam.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3abohblfj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3trsixslp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwlzzshr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zzmcudnb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3sofznsmo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3joyqjpbf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lrjiacpe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kjnkilrk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjcjmavj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kczsuypp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rfvrzkmb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nbjvcoic.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iufmswpk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3oodlzlko.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bkvhykyn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3gtxcyxpf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ezedhvcv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3koiyvkah.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ocsskjkf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wbcxgjos.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tnxdtxlc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3prmryldk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oxwfwuzt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ywjbjgju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vewhpmfo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lodldqoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zehhilgz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ujresnyh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3esmehjyd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vpfzvqfi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3aauqoxzg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oldsnirv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jaajbjqg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wamjrbso.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3esmxamgp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zizvvcia.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3raudcban.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bfjhqqkm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3miyskhnt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qtykpoub.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fvggsnku.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zxgctxls.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vbnrmutw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kpfbasfh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3kenjbkay.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jbhhxlsq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oghlcdfe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gvptlxwx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fpziatfx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qpxdsqsz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehiaqetr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hcpmhlfn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3nckfjthz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vlsnpain.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wszdzchf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bjcbvrcm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pcegjmff.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vyzysenk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfloglbs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gxpnaixz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qlqdjsql.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wfumyggl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jcbozqdq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mmadvlmc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3danbettf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3otarwmeb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlicgtz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dlhferjm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3njrdbrau.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fmllzyne.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qabevckm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xtfjgrqi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wkfxcyiy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jemrqiyu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nogcezzk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vglnhfqv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yxduphzx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vkyakjzr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kbpvyjgi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wpmoknoq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mrmqwrof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqnhuqtz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zuboymid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txsizqbz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3azcytbcn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hbgouzdn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jwzpqtcr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oxtunqjg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nsizjtte.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zwilvzhb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xqvatolq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ihfsjkfz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kpuzwvpv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3joiauxdt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rzdeyxzd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtqazfa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cvfqhlgn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kedvlgvg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lupjanhw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3boxwopsr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xjsanevh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3oeykclri.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rafcxftd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hqofchye.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3aenuywhx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jiywozuk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yiwqsirf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gzxdzurx.html


<!-- 参考信息 -->