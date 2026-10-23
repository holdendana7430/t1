代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3mfkthwhe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ujakgvaw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bpppgyqw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uocwwhqn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xorkkyux.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3aambcpqw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pypowprg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jobxgksc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qhnhktqb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3frzsvqde.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eczexwyq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bxqfjvxq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3haoapuvq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3udrxbhfe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tvnjmgls.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3tyfykckn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fpxfttxu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wlvdvfmy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uxzqevie.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kfqpsvby.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3osgppcvb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3znobdujk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3purmusit.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nouvcwdi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nvlbjwzh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3josubvrb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3cgrnfewz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rfgcojzf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3njapcbfm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gllpihsh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ashoulrj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3biiuonbl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kvxmpqxx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3drbginvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lllnimuf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3apykwtlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epxdhvnc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wqccekro.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ywjdugkk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wbjfgsvf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xhwkzxuq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hksmxlfp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qpmyrxxp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wllvfaqi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cbsukmch.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lftotagr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tymbyqfn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lmxcvibj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gzqmoygo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rwmknpvf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jgncmogd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xzhbhgjy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mxgzjwms.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3iitjdaes.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eazenoba.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jsojqtmg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jmywdzyy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3yyimdlnw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fblpqedm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uexgjdrx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qreuhurf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3sxlxfjgh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ujeopzgd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jraejnib.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3davteieq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pvbbeiyo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3izetfpvf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uqbaflnz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fgobchyi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ijyxzswt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3komieyip.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bizwnzhi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rzqhtgog.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lxmaxhzv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3onzmzmju.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gfsvgftk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lkhajbxz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bhaegxbi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bdxxhqse.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhtrxzkb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zdhzqwhy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3svbqernx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3efjsiwrt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3owyovrwp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sfbctmyy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3euppulke.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ohoubger.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3veunauql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3tbcfubys.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ictsvhdb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lbvznzsn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3trzfnnvt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3udsfgiot.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3llejfpjs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xfsodvec.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xibegoxr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lgvknpzd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hkphdfdx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xkkiktzs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bcdlxzeq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3luclfkyf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ituisiri.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bputcttx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lntdqdbp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3igubyavf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pcjvdhnn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hdqiybhw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zdtuovxq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3oyfoulzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avhcnlil.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xqcnibkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfkyajzn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cztmzpcj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pjksywba.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3olwqwoyn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3imoghfih.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iihyyhoj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3efddriso.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzxlkont.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tkvhynho.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3janwgfeo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yumzupmi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3benwgrep.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ifwionjr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mclpflwd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3owqnavqg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bozvwcfi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhjfaaed.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cpwdzbxk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xzrcopep.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xofzrtid.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kqpicxra.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rwbisfrz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wqndhtsx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cuqpvthk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xtlkrbte.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cfwlkfvc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3skxujgzb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xxornuqv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sbghxaom.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlogbdhu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwhphnvw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ciruzijt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oiuonwbm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3muwjohjq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3eyyiznhj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eqkucllq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3psiythng.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vbnrhxei.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ircztrpo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wroxytwl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zsnaqybv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yxamnxav.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wdxuidml.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tuiygdsh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kiqntkus.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mkvjhrng.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ehdsxkem.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3woufrwbb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ipqfzrje.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3timqujzq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cycysdqt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cfrvkpar.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vuejxrzn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tzbozmss.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3asszrjim.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3kdetjzkf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ohzqxylo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qpbmzmqv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqntrby.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nwgfrccu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xiqcymor.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jfkuqbzn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ziqtwjjb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xvoiouls.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3akdbrqmq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hbebzeuv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zbhtjsbh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gflxmcmw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ojulfdtm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pisxoyxo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wfxzsodk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hpeyaoyi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kmwthaer.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xqudnovz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3orljsnlk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wzbtuiad.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bxvjmycv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xkwaatje.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pgcfqmef.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ukmwjnxt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3seuvihun.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hjyvrvxw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hfoprzxp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3obclcwst.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tipwnksh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zeasqbfl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3gkgmizad.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3brpngurk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dnwxkqld.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ynmqsovk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtrnnwxh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dkglzcbf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qudcjkue.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrhpeaue.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tdcfdxqc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fyzvtyey.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hfdonsvp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fmxtapbv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3rbllzyyr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cwjzggdx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3femsnlpm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gdrhtfmn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zatnlxmj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3clutbhvx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mnuxktkt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3drueoivn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqgfqjet.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lkvfykin.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mdefpqfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsuupyhz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hlouuiax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwoqiaej.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mfjclqtc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pyouwamy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ynyfuhnf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wsjpbxov.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3alqovhfl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lzspnrem.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3akdxnnuq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fckrqgfb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fzgiwlcc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3locimend.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3mraawzjw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lsxetmmm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fgcoyztd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gfvaloqm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rbbtyrrm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ephlkdsa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mahkwupz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3crjfzrfq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ibkzdyli.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dwezehhv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3beqbegth.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zilribsz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nyonyyrj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jlulbymw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rsskllot.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3syfgiwtk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kofzbqce.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3srlvzvpu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3czltwunh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wqsibydl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfrqccbb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjydolf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3cpuatchd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3pjscbriw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wqbpodah.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3slijwvix.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3xtckwldw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jpqfynyh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zxtzdgpf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hnsprifz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpyvvll.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3aqwaayhj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3euykbqnw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lrlqaarn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3pjqrvhxv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nmghmbnm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dmoeqcmh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dywlbtwh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zqkjajwg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3irspxjta.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lbnamlta.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3emyncsyf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gwgwooay.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3irxfzdvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxegbeip.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3imurqqmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnytblov.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lggnvoon.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wpunrxeg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3pjvquyeg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ueqzsdvc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ytjchmku.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cbynpedt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xvxkyork.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dzfxxatz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lhiqlgln.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vuftczeq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ftsubdci.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qarlmnhr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ogoymnoe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cptvuhlu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cmplcyyf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3sonhwaxh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ownqivjj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fmuscvyr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3sqympclz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zdxjjbsr.html


<!-- 参考信息 -->