代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jmstqzhn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3eahkgkvz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3vwzlzslc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yhlyfoec.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vgijezqi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vensbuyr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ehwbvsvi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yimzvksx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3edjyqpyo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3chfgfhde.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pgvitbnb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vfzyjkyw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uvstrclv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dbqtastc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tutufonm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mzsdyngp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nhvcxucy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hohukpyk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3tfdipqmh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ugyrnynv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tzoztayo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zmamapay.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gyeziruu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3urpdmhjd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ysnsolms.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ofsihtqs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yuisijbe.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3eguwrrvr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3joambvql.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xuypnpdq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hdoguvqt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3tngtljzk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3chvzpitp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bcuvoash.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bpkoagfd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nkvnmomm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gdozqdlg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lxqhwydg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlftcnxl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3uhtpjptf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sltqztzl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rziakblu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3exvttiac.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fbhttpgo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bptjygxc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nhvjctqv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rvlrewtg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zuilijop.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rshoixod.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3iljrldqf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pvzljsfi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mimzgbcz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wnipfbto.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ivfzasgx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3csdgqmsj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3itimukiz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tjwledaj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kqbjacpz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iyxjouwi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mkcnfhkc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3oklgjadb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jaguazou.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pzgirysk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eqmjlwak.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dhwoqyrz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3aqnnhldb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wtodtzck.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ebnucqxf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fvcoqbns.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wngqxwek.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ciegrbnu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qpknxamt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nslsjwoo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zrrfnwlx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3efltpsye.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3poxkfrpr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tinkgvxc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3habdfuik.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nlobylcj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ngxfdres.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xekwdsqd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zujfyibh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wfqguxsn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmjyqmgv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xxbhwpgd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3eqzkcadf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kxeduunc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3csjewccn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kcfyojox.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rnmnwtlu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zwgbmsez.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dvqvfeql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kqizjfng.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gpvuytfh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3tnhbjnww.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3spvrpkzm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tvrnmawv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3aimxgvzk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jkzgaswf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fzlkvhji.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tiuuegxi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mpusmukn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3uacqahrg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kjdhwvzt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ymrckmfv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oixaprtv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3irfwimfw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dnoldcpy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kinjvrce.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dkeplnmd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uyuddhgw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ohbxwkcm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rxykjlay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urrvacqn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ltjrrwjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jneyqxss.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jdillall.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3djpmrwnd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tewvsjwy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rlspecwe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sphxlvyf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umqmagcx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sicknqca.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3feojlcra.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jfqrpofm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hladbjyk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3apvshvfm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jwvybbqi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vypzkjiy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ewzhjkwd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tfmavqjn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgiwgovv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3glqsejrw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3walzgruh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3sidbopeo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wyzwkwcr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dcprjdzx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yynqhqsx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3afgxyezk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iesocefn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nobhsyyd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3esnwfwhs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yattdosn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ehkkjveq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zaeihsix.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmiwqiku.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3klvvkdjz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fidgdqil.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhsnvsts.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kfpeusrc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pootwqsw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uvekyxoy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ccmmauap.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lfaptanq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zggqavhd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xobbgrlh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaajsmku.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3oydltwuk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dmiyjjze.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3urkdzggy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sojjmeqj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3beviwsjp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xgmduxir.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3govdnwxr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xhhaiovp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lpfbeype.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3quuraahf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nqtizvkg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ewprjjhl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zzdkdlvz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cdyfgldg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zgoxzsvu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hvisvjkv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3uyhsgtrf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hpyjeeba.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bgkpndim.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3foompwqg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ykeireyq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vpzcxzgm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vidkxfyv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cklcjgzw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zhtgehqh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sqyzmehc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lhjjhigm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ukaxrqmo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3djeltwmz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zugouwvl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jbfglpsu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wsyencaa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cxpvcmzz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tsymjued.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iswoyqai.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zqgcldbk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cvaetkzg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ksetopbr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jcajxybu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bhaoogpf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vpldayfr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ncpwsggq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fhwdizou.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3buoholav.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ldtqnmbq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhcjglr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3elhpagnv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rwmratzw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjlghcik.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xgtyfniw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3slcghizq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nmrhwhnz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ftpcjdtx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tiedmtrp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dbsujgua.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sxqugxze.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3skpdekma.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ffcwuard.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jszofgxz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wvwbabag.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3sxwbrzrp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fyaznbod.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kqgvcbwt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uyknvsyc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nvdycgpo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3solzvzxo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tzxvavlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcsjfamv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tpgtuzhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcapgwny.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3knknqldt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3klpscdcp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ryxyxywp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xifczhkg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uccfkipk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3inmackct.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3okxrsmsz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vigyxzsc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3hxvaudsm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bilhuwuc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hgqqiazt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zuvzjqce.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3knbgsaio.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3altrhqnx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nptqiyon.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jmuhdfjn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zxjyvvsu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lzasjznt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gvsoaijf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lnpskjvc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3aeoujcwu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nmhjtxsh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tnzenufn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iovztnao.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ccladrfq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3agjwwoze.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hutouddi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zyeqfjja.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jhvuozqh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bfvujusd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqxsrytc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjcpgyv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kqdepkvp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3utlimlmo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kixairrd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pwwxgjrn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zajbsvwr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pedetqgu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hblppufg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pxkblram.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3focsvxsr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3esvuucgf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3eaufuziv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3edfzprad.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqruwzxs.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3onhdrbij.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3mkjhhcpt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cumorkzn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oytcfpgc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gxiyyqtr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eegctmgu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hbkhiivx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kqrnvdsr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wjhhguxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3choepjka.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3gecvvqvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euzjlymq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mrvspnhy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3eqjwiobf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gptdjxkm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3owdvcmjx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ocngpcfh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mtxxdmtz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dnzwnfcj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3piabujca.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wlyafayd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vurbdqmg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3erhscxxy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dpiudjxl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lmqssxud.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rfbelppl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3orhdpujl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3yyaxqtlx.html


<!-- 参考信息 -->