代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ohydhgzr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2unpvauwu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qausvuon.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2dsmatxvf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xivvccep.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2taptkppc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qliyqlqx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cdgtynku.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2pqjxkhiq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2apstoays.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hcdzjkmk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pqfveory.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ytuovbjb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bjflywmp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qptnjpms.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2houmcvbl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfhiixo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rveuhves.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2sezlhctl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cmzdgsqv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qvwurzwj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lrcsxzkw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ggddbohf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zuwnrxrc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sgwqeasg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2juhvxypi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2shvsytjj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2itftahod.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2puzwebdi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbxymc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qpamirgk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2huyscgsd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2urufrecv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ipbzjpmu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2khgyskcx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zbfklqqm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nzxrrfcx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2korzirgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdvgxinl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ukiojshn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djmeuasx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gpcrgcqx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vcpwsagg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2evpjgdbw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzpzlopx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2esahouen.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cbcgqfxv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2viyhhipt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fhrevsaq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cvmqtmhw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pycmjiay.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eotnrovr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2plqpcozp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wnovxnsv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fbeowlvb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hjnwngis.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kxmbmvmz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tsgwnaju.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nzdfvzzj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sranbnls.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nhoywnra.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uefebzwy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sgukyuuz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pjanswdx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ktbiuike.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qnipkxgy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yoioeimt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hscabgyb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xzpbyqcn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2febnntqb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hllksrsj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tjxktvum.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ggfzsage.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xfojyyvt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kcywikzb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2chshnlhs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fuscqemx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fyxtsfnj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jhahlubm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fjrgyerh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2svdsynax.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzusswna.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdipinwx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipqmizyc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjxkdgpm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2avnaoaqw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ixtethgq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2oaudpajv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hjdifnvh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bhlknqfy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2akznfvvs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ydgnipjs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wjkrvnou.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nayiybxf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kdeawnxl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hablxmzj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hlwoxpkv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ubrapdkb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cghmvirj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2avshptbu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2poudvtwi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zrnrbylp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ewsaueic.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2npgqfaob.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2klzwrdly.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mettczpi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ufoargfa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hadiucpl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2grhdddsp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dzhqxncx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vqyxgdbk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2slwovhzy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kttbdnka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwtozgrx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2csvgrjqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uohqwptc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2sreqqlwo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zehfhhgi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2czbpvnen.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2irhqiuxj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lxxosxjp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjqyino.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bksownbp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2bcpuxjgw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgiimynd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lsizysgh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zlpmzrpw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sjkpuvvd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lvubncyd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2scezecmw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wuvnhxct.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhprseqw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mrqraezo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dbxqqsmu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2scdvjamc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2otybycqj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xzmlcojz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2exvpikug.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bvrpizli.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gfppiufx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2yqrjbvqy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2spgxeufw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ffrnkztc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ihfzoasd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbzxnxfn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qiuexaim.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nteoqkuq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pcxtvllq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2telnmtsx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jvnbfuju.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hcfkrpab.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vckyjszp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2igjxiwyk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uefnzljd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xbnxwnlm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ctbrwnqz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2oeesyqpc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sejhvrrc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zbbvjnfi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uaiszqdk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrchjfop.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2umpntrty.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cjjqcdon.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xvkviqjq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2udufadjb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dcjkvurr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bqokvmak.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ygsueyub.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lixxeyta.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wleapwmz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mtwqyeca.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gphoetfq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vossmgpa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jguwhdss.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2frxjqqpn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lwdplgbt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wexwsqqt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2crqovdjw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2csnwdugp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lxfgfwrb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bqrbdohu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jknfukcr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2elovylxt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ctfatrcw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vnstexkm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrwrhkws.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rhzuzycb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gxzzhdtg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fcibpnbl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2libkoouc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xjxrzmkn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jvbviube.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tdpmiytq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2azzlkvtp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2uhvmthrm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zikzhnyj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jtuevted.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2agpowxoo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2toxhhlua.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2itejeonq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qkokntqq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xreukcti.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2anfmotws.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fmdhcghq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fjvabnbq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2icvkltgm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2trsxdyyx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2unwrvwmp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmypjeaz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lkehpngw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wpokgwvz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2behzjjya.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bvvnhadg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qfxoxgoh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uybikbjx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2uddyrnix.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uipkarci.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gzngxaat.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vfrzhaes.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ufuypbeu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gecykots.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bjhkqozk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2clhuxusv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vnsymjya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdubpeli.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vgtjioed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlovsyji.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2usqorfqv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rrkzdjey.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2drdvxnxq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2fkltsfnq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fmjntsnj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ccyexrxy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bsxkxxox.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mdoontgh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jnskpnia.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ofkyhzuf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dumhvmwd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fynoahkl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vxkspiks.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uxbevyxg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2stvpdclp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2njmykhlo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2fydlczed.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2iwlhnaqn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bdzrceur.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xerdyseu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zfiibigo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yncumyfa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2upunngsw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmixpbdd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2enpsromg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hgfzsudz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wmcfcmul.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ulpqjbbl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2svmnqeoh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wsrwyyse.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tuuxnsrn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrregvuw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wnrggarx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2eamybayk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jvvmtzio.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2whuokamc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vksdhswa.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmbwsxo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2blfkptrh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xcrckunu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fjnnewru.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ylbfzswz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ffrizasg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dudtuaxl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2aosilcek.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2owxmcdne.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ooyyupvu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2fkliizpx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iwjnzhvq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wxqfotil.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2chzyiued.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wpeshdzp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kruifvrc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2odrjwobg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtgiqehw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vjnmgfia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wupwjypu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2iyvpmqtv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ygecoxmi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2nnpyddrc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nazodmzq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2njmoawqk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wgjmolqh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2psdkiugf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wmzswfss.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rkiytnqn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lvdrxhim.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2emdazsrc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqposnka.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tpbosqmm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wiobzgkd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpjkcxy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kjlafvvg.html


<!-- 参考信息 -->