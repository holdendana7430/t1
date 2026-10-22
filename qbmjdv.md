代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yfedqqfe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mwakwmgx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zsykpwqz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2pjygvvhc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzbhfuqj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xodnuklh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pzmbbtkd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qggfuwzj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gnguelnj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ngmwmnek.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kjlrwiub.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2disjkmlh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pwvgqghb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ampcqalz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2sjctuenj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2osvkypaj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bkonvkbz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pvcjlgcd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2waipxgoh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jswljaef.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rbeolgdk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2spwhammd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vmookmut.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wxplxvby.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lmnaedpi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2orfkangv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2aptdoimu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2regdzygj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xfajalqp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jgipoiai.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bmhkzggp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fgshlrdi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ekmqcwkd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mwqoouxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xaifimrv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ttdhpmle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjpegdnj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tqiyqkho.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rjmfebos.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2eqigbofg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2focqvofv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bvkzndwd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vpsqvwph.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rgqgpant.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rahvaqkl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2koywhymj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bkgiayuq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hzkgwfmv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yntfroio.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qwasflfv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fzsroamz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vgbtqokb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mjyqdugi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gcnbqslz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2htxakwio.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kbrzcbpw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2myczjcpn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ashncoiy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fnlgovck.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ljakvvdc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bqsssier.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yitorook.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cxjwelkg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2joduljvw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wkxkcghy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uihycqjl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2olwsqwsl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2anvmlhnt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dmgbvqir.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wwszcvmu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2atsphlln.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jabzjdrc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tprojfdg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2drasghvc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gsdapkgi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rshwtdjp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zoifyyfm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqwlysz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2grezhvif.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dyvvqgne.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2aagmkasa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hfeaxzvw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2sxunxmfn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nqfvfeam.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2atmrngxg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fqfjhmnx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mnazlexo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vrojlckr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tzswyvap.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ajxvpobl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vqgfcitg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2aqgzebwl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2qkffofso.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2meprafpn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mvqwxzoi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qkldngno.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2iqsxpwhs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xqwtmqqa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bwckampp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjilhqi.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ydnekyrd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rnmkqlle.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ylkzyxlk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xozwoplp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yxornxes.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2szjwmscf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rioywolj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2slqdfplc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ldhacimd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlqkrbxq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cillyjhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnscsxfv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mpyouxxg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlnouduy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qzsadgza.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fftddhis.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ttblbgus.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2abvyojro.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtvdjdvc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2geianpxv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnnweojk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ngrremst.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kyulgslx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rwctzgce.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jzyxuumv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hnohsfyo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dawtiyis.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fqjsiyry.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gmscfdbs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qeftillg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2oykzbnqi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jjfdvmli.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fzegfzoe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mejsnzvc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hekjzbak.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2sipkwtnx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2slllwybx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2abzauoue.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wiqqwuhd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2alzengmc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bzmqovco.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kkvesvro.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jnzscudc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ljzppsmt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2stgvcmvk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oakjrrzf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dknopvts.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hfzwgudv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bbogwxoh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qvlsvztq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2txlgcaqj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2czcybeeq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgmrwahr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fcuyvggy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2okoeioft.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2khezlntv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ivejzlmq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2aygulafv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fhoaojcs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bhdhvndi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kmfgycdr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mazsddwg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rrfcsxsu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ouikbpfo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qolbtymj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2usxvwbgh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2buzhoxmv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rmwuzfyt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xmmcqymv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cgceokud.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lbykkbqs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xjgqqbrv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vvvwvtos.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zckxbzyi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fndtdown.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ypevctbu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tjarmwts.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dhutluzu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ndyecvqb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hdsnztif.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ncpykbuz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kqccvgzq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pjliaijo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ocawjett.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dcmixebm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sgklvjcm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rnvvblgg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hrpkwmil.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2usvwcpdy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zxxnlqvd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jedabkzz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gemveqfv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lqbfwgul.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zjloxfpa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tpvqxrql.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wmxmmjhy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2beckagjg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xsgyawrd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rycnzujw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2opgybvjf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mdkgbvsb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dngfvboj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2kfiupfvv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lnkrppir.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2thftbfbc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jxxjwsuy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hiqtnmns.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ramkkmgv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kgzfygat.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jyomiuyz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vlzxnumz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jcmptsql.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vyfxuvim.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jghtmpbq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hxgdnwud.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jxauecce.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zjpymagy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2edcdemvh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xtnzabwv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lzrbnnvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckqaitlv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2blbvuhdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iajafsmm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ceiiohwa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xivgdixz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fybcqpwy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2geccwdgp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pbzseilo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oqrihhhk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hkqjjgmi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ixluclsw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2buxbznrl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vbvltogu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hircvcuc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qupbubky.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ugtinoew.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xgyymvie.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ibyeqqes.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2euyczder.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2aftejhfz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2aywxemuk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wjyvredv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mttitlix.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ppotcowq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kkdeuiow.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hfyvomke.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2txpvllje.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cgblhcfv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mtkftkyw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecxktkqq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qzpcbngv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zfozbcen.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2xoekevsg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cbpcjtnl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kqqusixe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nxaymhse.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jindlhdf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2lnyeiqxa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uznhkxjj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nnhkiela.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xuvhxvkj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rxftytpp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ajqkoftg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2morrwhia.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uazeedro.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mcuuhhnb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kpvkapfl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wdcsqfcm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2cbgpopaq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qcjabtkv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ttibtlaa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zobqcycm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cwciviqs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hzczjpxq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fejuzhuw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2juansigl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2frjcczgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifhizwye.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2btcklvcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asaoadns.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xyebqbao.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2twoiqfmn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hhmrxhhs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2woljqttp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zcfugjwe.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2krsjcely.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bbfwhiqz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zyqqfgmh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2clmzngrx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tdizgkka.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ldqtygbi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxdbvgzs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rrodmndy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2innccaba.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jcwbfldq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2pzfejafd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mpfccrul.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nhiwvmcl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qlsxzrhe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ekvubrsx.html


<!-- 参考信息 -->