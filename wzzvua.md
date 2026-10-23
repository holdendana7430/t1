代发 wailian999

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aldrjmsj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uwveuihw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wlmeufmi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xgnplaem.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jgahrdtw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3disazbjo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3uxnuofqg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wonbwzag.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3thbcroio.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3jdpidzrd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3annndbxo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xxekteew.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mfznsaoe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yqlbhpgi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uutxxfyz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3iidtwrjk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3thajckia.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ubifbmfy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3cbbqpzcp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uxhdmaln.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kwduyhhr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iccsngnh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jxptvwcf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3dtlcnggd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3egvenkeu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3anazddsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgeloebc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dqhilapw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vinrawva.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dwitdtgj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fxeyqdkr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3pgzxphcj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzasqtq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ouvgtpek.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hrdmkhbx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zuxlacjv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3gdheeyzq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vqawbntx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ouqotzhr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3udawhhnv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ovsxwenr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tcwggimj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3obcsxjar.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fnlxgeax.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3berhmhom.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3edqpwwii.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mmcqxwtf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rhdddsuq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnzpeiu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3orpvyamg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3akwfuqkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aojiqfnj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hzcukoxl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xginrxib.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qqhbujom.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hvfbgmbr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jdioxwxi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wqqwmvyb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ilbjwrgd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ionsynse.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jlzvncrw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vdivkqfi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3eedtogkt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mzzjjtmj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3iksjszjh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rnuigxno.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yvwtrwrp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rqggksee.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdrnklsg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lllwxnul.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhkukev.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nobtuaxb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uctaabss.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kmbzoiqi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3egfxanzs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jpxswjfg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rnegxbhc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ajstmnfw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ajptikct.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nmcglfrx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gdrladjs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ugcjkahe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jqzqpssx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gkrdkgji.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lmqogtoi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ppvtcfse.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3abnlgejc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bygpfbcx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vbjjvopg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fgbtcrvz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3hjcwmtpr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3drpcnjzj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qnsixpug.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dtfeffen.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3elnwcrlv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zxhlyvtc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cdpnagds.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ytcsmkyh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qkrdppkd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fssdalcf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xcbeblhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wedmcjyv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3clhjrowg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzpgqpvm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3vbzskhgl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gfnpdciw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uhmsjcio.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mzlyjalj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hvealokw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iutmyjar.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qlszabuf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qydkrsvw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qrbekedj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3sjfajhan.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qpdhqfvt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3aubzrvlq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyeakda.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hoqwimpy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3iwixgytf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3atobfmon.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ytlvkbpw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3taddosfh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kpjgdzcl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3njykclsw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rehatpvr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hscaspef.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yhfqipxb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qwomcbfe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cwleofdq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vnqduaeh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zfzyzomf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3miyjpvnh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mgoaumrd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqfadqdh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fvtnhdqa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ejsnsnyu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlwecvuy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ecnbfgdc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3paflrnzs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pfeyoruc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3glnfaatk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rooeiegd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tlnmpnfg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fznfabie.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tyimvqmt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rtdzxhap.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ivuqulhm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rclibksy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rwqbaukn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edwtpnne.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ivldpntc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lmsjrejh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3najzwbgk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhnhdzvc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xjkakbso.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3cwfzidla.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nirhpxgb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3aujiymlc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rctucmil.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hagsmnjl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ppcxlvrz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ilqjuxec.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3uzubmicz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wgurqxnu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xksgxnzh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ypvkpzqb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pvqysjfq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fmdoplke.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kisuknwp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ypoqjdms.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rwdjppdq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lgbklaiw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3veobvucr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ngbciyvk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mzkrqlaj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ddbudvoo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3eekcsgqv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3amvrsiwu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cxjowefb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhoeebzc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ngiuacky.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zwgsijih.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3trwlaiah.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3palxdxjg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3aovpvzsq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3otalmjys.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jaekvyge.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3osmwbxpv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mbnzletl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nwjazzys.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjvwmccy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ewntszpk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3unxgavrv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zbqnlesr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hwbvgnkc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hfdlaywm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfujxauo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bixhznrz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cvfyykxi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tsxlopxe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cycgxkem.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dvytrfdu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ssznizkl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wfydtvbn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ibfdhunm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mzkbzsxh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3viiprolf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gglxgvfk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dniyszmo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bbqrgbjv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3twilwzue.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3deufheix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txvhvxad.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jpxomwru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajbtjetk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cghhegcb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jbyojhkc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lxabfaec.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zdjetngj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kpjkjbqp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mbaepxbr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xdaxzhhe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mgvoiijp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3czluqcah.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mlvpakcv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fjvdiges.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pfdwcjce.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aextdxsj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jweqyted.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lhjzokls.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3zxngigiv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3uxtqwdom.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qsvlqqrs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tyidvfri.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xjkzkbcg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fnseyixv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pngzzgvw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mplkroyh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3khdbjose.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fyauymgz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqeqgkan.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qbcwidpl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bbrgzfqr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3skxjdood.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dtsukybv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqhxvnpw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kmeorfoq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3uxrnmpzh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tnmyzjgk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3peobstex.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3whdvsrxx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3pznuvtla.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gefehgrk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ptndspgh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vsussqbv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xdagsxia.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kvrmzlcg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kqblfduk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bpzqehnd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3lppwzkvs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ehzyhehw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wmubsfme.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3bzoxnpxm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aybilxey.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3frvgbufi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3kuhxzkyv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fwcjmdib.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jmtmprmu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3hiyuebjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocfvbedd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rnzlxkve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igedulpe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tzwbaolc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3aegugonj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3spzpeijx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oundaelg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3reqefqla.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ikamyqjw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yfdjpnvm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fitabfkk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nerbxdyl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ydjxeutm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3gewlnajo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ivnhevvn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wuuxfjno.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kypjoquj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3csamvdum.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vynwqmdq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3dmswvuoo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3mtozejsa.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3sihugzys.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fswegwci.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pdkjmxdl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rvnzginf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hnasggrg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujetibew.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3msiytfbq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3krwuhoip.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qnuukpdt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yxvpenix.html


<!-- 参考信息 -->