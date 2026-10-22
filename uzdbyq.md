代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2coyjqwyt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2otetlhxy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qdzwkhhx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bsqbzcni.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2owwehlin.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sxcaitlw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dpyaarzl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2xyhuopoj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kznkbioj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bfotvnuu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xxsojoml.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iamxsull.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nrvfiydj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qfiguagj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ftjzeufd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2twapqhpp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxeftwa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rgybxtfn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mssuwscb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ltjksrus.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ayzngjzr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bhrdgggr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jarecmlj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jbtvfmng.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hsdzzqbe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2goktndyh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yghlqqox.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ehmmypbv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fpgmlahn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2darwvrmd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2sdzkyhpa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rzvkgnwu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fqqwwwcg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2deteunun.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nnkoiuin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2cquglrwd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ryjelxns.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ypmdnvqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnzhldzq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pldjjddu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znzrxrjb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmnumcbk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xdglgkrt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hfiidjmk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yceqjxef.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hvycfmsi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cgoimpig.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iyreusiz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bwsjtxkn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qrhturuw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nwfigoeq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2opaatoil.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mhgsirre.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wstxrkxk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2noxinksr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dtrbtzwb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kryapndz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gaewluau.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jljefjel.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2atslidcg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2guypihbx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2elaipttl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qsaialgj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2twowmszh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2redhdoij.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ymwssomz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wkgiblas.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2livkvngd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dxwekyay.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dgcpmxav.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xidjcbqc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rspmctop.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zufhuhbq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nnzrckrp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nxkinpaf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kkmfpphe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mqrncinj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bracygrg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2umcolzdg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nuzxqcgr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2viyfgruo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ztvtpvus.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dndxzwgf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kmngbmsv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2sdbzazdl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dcjprbeb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qexwxamw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qhumkrfd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ovtigrff.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ldqhqgxp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bcolpsxy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xvdwoqsl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fkirhxvf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2srlpprec.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2njsceiiz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ejogcuax.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2btwqbfdz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xzmlkdxt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2idxrlyiv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fgbwaxqt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmtnztn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vxjsrvva.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2dguqbtyv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2lwczsnyh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2puicicsw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2miwypidw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jpmwyqsh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fprivybg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hpdtauxx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mdogalah.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tqajdsmm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xwotfizy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xlgtvfih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqemwljm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hzuqnxsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsdoecdc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pksqnyaq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ihtrajof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hhzrkyus.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bbakaatz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2flrjpese.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rrzvdelo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ahxhmyob.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2omsgyhzy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xciobuuq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xgvubcak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ucoohefh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nohfigkn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gltqonbz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xanyxtjd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gzkgftno.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wmjxgzub.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wgypowee.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bhimizdk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xftwssjp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2nqtafyin.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2drodyrne.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wrwdgqwe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tywawlep.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qderbwdw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pkpocsef.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hplaqsof.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bhwlbrco.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2myodfvpv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hlcohuui.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fohtetus.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2drecbcrp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rnlarlin.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmasuoap.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dnaegvwu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssofcvdq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2chprrkya.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tgdepggz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2woviuedr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbctbesg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqqtdbaz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ozqddotx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ewuykmlo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yghymlah.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2laqsehfr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jccwjnym.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pghqgzgf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2trefmjmr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ypcsnufu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ksdrlmiy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ewueaizh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2uxumifje.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fwhdlrkx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hunjzrjz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kfmrmloa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rprpzaek.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mflbkeel.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ohpxhaeh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2amctgvts.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ltmoykbr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fzrzfihz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rdnxnlhs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gdpcnaxw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dylvwwap.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kkpkloqi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbpslhgl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2pgxrsrln.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2llxtfojo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xnvcqfvv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2netbazog.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ntqdvfyh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ovkhqmek.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cmgalrrv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2euxaycyb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vkxzqitx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rtuoofys.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tvrwbedx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vilfombq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qrrpwnxp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uneigwaw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xakyygco.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vvlrijzs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2yfykbium.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fzwiytvb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ivbctbgs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yqhamuyf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zydhvhjl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzsihidf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kkgxzgxg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fcizddux.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2tylzlgjw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lijqnvpy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2swhyftpg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wgzeltxm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tlgvkokl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jkwgjwdj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pcdnrhnw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zvkwjilt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zkmycato.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2avwjgdhv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ytojjxcu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xdiryjgv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qdifyrzx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pberovys.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oixciilo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tsslarle.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2cbfkprja.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ojreupti.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qarngktr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjzbrxgj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2snclbldt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jolwooqm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vmviggmi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xxucefkd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2edzqxgrt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wlpzqwlw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jjahaobo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wqlyhqdm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mhrfswrp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2uojasvco.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jadfrhfz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ujoughyg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xslnvzta.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2pzydnmhx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2txgbrfpu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vboiytkf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dxkluctk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pdulnjuu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2goqbtstv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ueadsuxq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rulnnuxi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bydxqyqk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kxnmfrxq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2thgryorb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wbyhbuxv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kcpakfhw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kpsznoql.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2oaymqgoe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2epqekauu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2yuegneby.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gszebcsd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ajejjzfl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cyabewqo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkegtfef.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qvekhrbe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qztpasvi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rcebctur.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2unjuwrnk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2tytkgoyq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gmnzezcm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2okgdlusq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2merymwty.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uuujalqj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fcisloht.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wbtltgkv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uqgjoqry.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyynvufd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2obzdkklk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jomhcfvl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2dljtcmqy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pickqoub.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fydtogwo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2yqmyrwmr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gunvoeqi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2muwfoguf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ryahcdlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqvptkma.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2eapsnjgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csffypce.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2axwqdwon.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ahdkdtpc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hpybktcj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mefatrio.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xvdfmcfw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qdhipgmc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lgxmgynd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zrhjgrno.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fznwactp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wmbnarjk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ypgmauth.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xgzmbzud.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dxssijsu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xmamoetr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cvpcnzea.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ffeghrmf.html


<!-- 参考信息 -->