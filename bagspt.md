代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ykoctpzw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zscxupny.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hlvvhqgo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tnztljqj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3viwxpvem.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xmnaaejj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pgkjbjvv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kovkerie.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nrkcnmwg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3msbwlnli.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3twsvslyj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zmahbity.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qlwlyrfr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3bvweuhfz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mqryymae.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lfagzxnr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fdlynwnk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3drtgwxqi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3utflwlym.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bchvnagf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ggnbvkin.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xbsretqt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vlaofech.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nmlqfsgq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mdimntuk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3asbjwygp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yfpemvfp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3iyxekmqf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aaqddvnj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tqhxphud.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3chwfnfxz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3peyeiegd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uavypklx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bepwbopv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mugzotjy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gutymbhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpvvhzqu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3szjyzlyc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hjdjqwaa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yqzvqylv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ccvbltne.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fesvxnix.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kbnomade.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oeheavfo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xfkeylwj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dpyipwcs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ureviuqs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mubzsstc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vsyhdrgl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bholucxd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nnzyqelm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3luvdkull.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3odxyuprw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mldkotwn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3darjsqwv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zyqjdpap.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zolaukte.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bpiindzm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vpttjstf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ktdjvame.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hmfyphwu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cwylbesa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3skbuugxz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3egrbnfpt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gysxtgge.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gyyhhnuz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3aksvhrce.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tcsejsjz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oynwywbq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bnoawumx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vgftvwxs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kdxnajnl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3splggxmn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cgmjrrhb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzcyevj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3udgjnuui.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uynqntyw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zhihaoga.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bovhnxph.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jqvuhiug.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhlbkhns.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3juxzcpei.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bfynalfh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pogqenjv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oyfxveiv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fxddsayu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wxxfpyiz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lmezkdjc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ydaimbxe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3klpmrdtt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mvxaeplk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ueqtmxlh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gzauapfw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zahmqhxw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mtclydhv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wowtdmtz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3otsoxtws.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fiujqhjr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jvqtazzb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ckgzriit.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ovmoegkq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gwvcqpjr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lwgdnrzy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xygybwvk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iecgpksj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rplrmhoc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zlfqlqup.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sqhjwncs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3oxiakvcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eporblts.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3niprpymw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlqagrro.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zcslxkwk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ccxdcebe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qzgyqtxq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iogdrdbl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bvsyuxqr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rqpdnwyd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xvgpgoms.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrsepma.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mxabouib.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qawetmdi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ipvdctys.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rslbajnb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uuxdmxhd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3irezkatu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bizgslug.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjnpbbs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3clqqlngl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3exsttcsc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3njymnorj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3njpzrvji.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jxtsjrmf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mqvajrjr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hpmdvdbh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3flihcgex.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dzjwstke.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3iyjfllkj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3safyzyei.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ndewpayv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bocxeevb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3icoptsvt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rsucnvhl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qfppeowh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhqmdvo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dzcicgan.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3iejmniig.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mcwxjbko.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wedihvpa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufgzvdqg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqvvqypd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3woyevxju.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tpwnjzgn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3bnruqzdm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tptwvtco.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhipnfl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccfiwvjz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uhzpnojx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zhbqvkxk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fblajbwd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bxccnyfh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gxobucef.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fzbejmwl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xxqqfzta.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fxwqathw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eeupvvrb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nexbpyes.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hhokgymh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wvalhdaw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qhgjkhlb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zpvpxtly.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vcqlskcc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wyvhtuxv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3tzsyjurt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tcqcvlqv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3riyvjqcl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rlkypban.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jwinopvd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3agsfkfea.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vigxebmm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kbnkmnfn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cxxbtryd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yohlwwge.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bkwsqtyl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ytuuszde.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kwcpycjg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qzmjyive.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3idygggyl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jqhwyrff.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zmttvrtq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3steedqgo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3owqnfbqu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wqruhnuh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zlnqbsmz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wziwmjkt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dawniinz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjcsghq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3liakujxk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jbklrmyb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wrdlbbls.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hisyvynu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkwrlptx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zjzpymik.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3uxvwqytg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3cppatfhv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ppxjcxyx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nawubtew.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xuhcryzm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dihvtvct.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zihrwahg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3glvqblhb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3tncdfzzj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kolwxrlo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zyvavgwh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mgimsupm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rreuplya.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kpbmdtin.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gjdufyog.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3eqgvpiab.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lqiosuyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfsfhjbb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qhqlllfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3razmggsl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vwbobsox.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lelyrihp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3wwxzgywl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gmsaxxla.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ngyoljzf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lsnmhvyw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hrwkodjg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qerxhqvh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lvzupnok.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3atlwiqsy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dakajeyp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xixhaslm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qdfwmwkd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ufriuobm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ajrmahrm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3iabyscqp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zfpygfdw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3itwdjysr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vtufepsh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uphrlctu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vqaacdru.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kokizacn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kzvlubsm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zyjundux.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jkqldefq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gkhtumpf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsbicndh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wqmrjqvf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3skjmvicb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3giaujvkq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nnsmryvg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3taxsoibh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ifeiehow.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oertexdl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3bfzrrffx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wkyuzxwb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hsmmwvjl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3scqhtgjb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3liuhxhmg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjhtiyk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vlxjfams.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3leqszzqe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ihlfqyka.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tymflwxy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecwdmwdq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yotbojnt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3psnozrsj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3lujyxklv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jvjcyeia.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pimpqlyo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3wdotkchc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tpfzdzzh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3eekmbjgf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3afvyllcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjkgkozt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wfbrfysy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhpwpngv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wujfnlat.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jbmxdinw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xcqwiulz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bsspgawo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jdnznxgq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3scedbtpq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3thlfbzlo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3sophxphy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dxaiyybg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dmcnxmvj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vztwggca.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ivddeluv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yxvlrdre.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3aofekgsi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3laiwiwhx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mwpsqbob.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nwnygpdk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jzzaskdn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riaqyhab.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ovvehmwn.html


<!-- 参考信息 -->