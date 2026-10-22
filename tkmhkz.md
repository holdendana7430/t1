代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppkmtouy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xdrdkauj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2faimjmwr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zqbylmrp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nksqvfcd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bznrkyzy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujebnjon.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fhgvduia.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jiyzccnw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ghqaodzb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ogywxuyv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rncxnkre.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zlzvzdcs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ruktbayd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hufdjzin.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nbigmdzl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2biqsxrnp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wuvcktwi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2gdrgdchi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nhlzlkfd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2atlhqbqg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2swgxdfkt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gbacjwrg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2arkdmpnv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nsdezgdu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vezqmebl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mawgggxk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wruaejvn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ritgbisc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ojebbvfn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fyymulfr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kqkhbqvk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ejppddcw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kvdefwwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqmdidfn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rabsyqle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wigibfbq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xlodhltr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oiltpgoh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kwazrhla.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eldwjczd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqawdjky.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tfkquavk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gzkulurj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ohidiyiq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2utzzeooi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2raymxykx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fjixlome.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bnspquxw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wqolzqtd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qswtiufq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bgmkblrc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wendpppe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wsksxjun.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pgjiyfuf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jvqorjml.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mrjqlggc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rtflthmy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dslqdwct.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vpgnwblw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2sjtkugde.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2anoighov.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pizxrzdj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2fquyefic.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2uiknucbw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gfimuyjt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qvqftkgz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fktvtkas.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nyujleuf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hxrocxcr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mieadewl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2amqzchdx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fnyjazzj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bnozfels.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2njylqupn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zsogjnht.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2agkobhva.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edeosqiw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdxojgh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rydavcwm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zirzvrsw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kgjyrzbt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qcwsikwe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gsjyflue.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qtnmjlhq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ubqobwbr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aeqvwset.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qmxxxuwd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fekfnelu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fdqoomwv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mshprpqc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nsuwcxte.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2yctkdszk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lfhafoue.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2khqspalh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yhvekzky.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xwiohaou.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2lkgnbihy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kyyinjyo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gtqqcane.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qndatgwk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pepnzorv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zazuvomv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oowlqges.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nllshiki.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ypuuviwk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qamswkvm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2oktcjnrc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yieqgden.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjvxwrlt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ehooaaln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fszbkpjm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nktmmarf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzhiaknx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbpnxtb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xpfwljna.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mqmssqyz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxvsfez.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fwasxofh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2rcgxtfah.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivmikulj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zkazzeyi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bmlmtdfv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jntfelio.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2endlscdg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fgbajjqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uguihlum.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yrmqooav.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xpxqdzih.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2devklaot.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vseatdvs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zsewyuki.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kbqbwztb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jbuuvhkq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bmxvatla.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2yauytzmz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2eyaunwgm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uqlmpdqk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dgvzcnrq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2djvgvlls.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ndwwxpif.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sgcbiqfu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkncbksv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lahxyffg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ujwrnofc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2acvwhgxo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eusxvrcb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nzxsfdwl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2xxeqkwnz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jvctdnbb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxfjknq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzkoegs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cswaizvu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mrsjieiv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kyqessnd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fnthivlf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fzmmphtz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2awkddwbf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wndlyvja.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2shddswsj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ysujcvhl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2syjihjgr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oihbexlq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ugnpomfe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dibebndk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zjatltcg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hmozqynd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vronbuej.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zrmkulmj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cftlezud.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qsldlfnr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xmcksiyh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2chhtgisf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2incyikbd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jxybxlts.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2figkmavn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hwurzivj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ohentnvx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ywupmvxp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ixpcmioe.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2denvmvqc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rluqekgi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xhpxxlrj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lzebeuvv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uslkbswp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2atnjlfsi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qiuadnvi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2honhdxex.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vxnhmxjm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tpswhjkg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pheeacif.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2seiyccbl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qisrszka.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2uvlwpyiy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2toycbejo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkedzbbi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cmsjoqlf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qoavjeww.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2lckyiqcr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yizerfqd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2uvraeleu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gynssoul.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eaispcbi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2pcgnjrub.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gdvoimtd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iqulhbge.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2afnwgdkl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zplmfbvr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yyzciddm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hkfarqkc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ftscfnkj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2faihufbn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dtuzevlj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2agapydkb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nmmfdjuk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2owxegxrh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mgwlwbsc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zcicllse.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ujzofrex.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2omqstzty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epjcdzfw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lqxxnawx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttjfaobk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hhuinsfl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bvfnomrz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2oecqlsfr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aabfrost.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cerkpnsy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2fjcmbzzo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2szqflbma.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zxwfrato.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2eoazgwkl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nklzbpyd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qqopavqg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mjynnqet.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xlfbutym.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sqzdfjrb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jxizlcpv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ctvzqcbs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qerikuue.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vqbrmcqc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fmtxoqjk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jsprbhkk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bgyxdiwe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2eynxdpuf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lqqosffn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlqytmc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2eadggagv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jawechzl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mbhbbrsu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mmwxjifo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2whabrxzv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yyvsdmpe.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nsqjxzuv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkedgpuu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qvdrrapa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2whnfcxze.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qusxcpxq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzuyegkv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zjdpgosg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gaxynlfx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pjgyecbn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fddtxjti.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pptsxcbg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uulzxull.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uzmmpmiw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zjwlmeof.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2miltfusc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ffxaxinn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hatqkcla.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jpwojisv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jjmmsybe.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xesgrcvj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bfwyopwh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fnpzfsnu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wlgmdvjn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tjabzamf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orxeqtps.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2begylexm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahnjbezl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mqyvfddc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vwedglva.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2advdjssp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fvewxoui.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wfpmrkvy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2znnuydxn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yuglknvn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2muhzcfdf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gdfxqjjs.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xacgchlu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2njfdmodp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ckfbyzbl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2engyvuac.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2itkkzwbl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jludhhpu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rnypcbfx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2abdhuhlq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vxuqfujc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2pwafnxrr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2yjhxtijm.html


<!-- 参考信息 -->