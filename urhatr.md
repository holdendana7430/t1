代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dtbrshgj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dwzkjxvs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3vewkqvdb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3nhixdqwj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3empwfnnd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ulfxebdz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zcvxhlcr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vmdbgwwu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ulwizyst.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bhjqsigd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fnxjhmgc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hafqwrbi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gppxbpgf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vczhymjk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qlzcpedp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rsyikdoz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmzjkzn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wyffulfh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dcqfteag.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ntibtonr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3noqwbgwx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ynqkpzse.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gtwvrsyn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vkggggyg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hrnrtwzt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3khzhwsmd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3igfyqkbu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tevkpeof.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fjykfdvx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lymnolpg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3iqfmjemz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lcdpsyxe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3advigkbp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wazzfyzg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3enslzvom.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3sqxwblxb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qxrjauci.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pgvqdnjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddijzicw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zzaoeyje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjncclzk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uzbvablb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mxlxttkf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3huqcqegg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvzgeduy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3raozyntm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dmmbbrgg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dkpairux.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gjeglday.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3chcudpgh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hrdtctmy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cvzdylri.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dkyoiwrr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rknewzxs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gisyqlqx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3feffiagc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3icxfvmhm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nazraccs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pfmfpnir.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sfkectgm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qinpzrtp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lzurevav.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jiwhubbg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3plexydst.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bnpfbamg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3uqhocrxe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3lrxtxmlx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xzlldtnv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wwvqbikq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3urhwsvmf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ezutgtoi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jmjzimvz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fjfakrfk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3grbwilgs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gfhhtbtw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3htmozfcg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sxihpfmn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rlibsype.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rjrupgvq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iubzivms.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enhumjun.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3umdasmtw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chbvanms.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hnsggarc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xinsgfga.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3czjifpki.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3taieejaw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lftrkrag.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ylfqpzwz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dlmwzkfv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ebggnshs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ybcbjkki.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3abytrzcz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nbgvbxqm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3siykgqmp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3amjexpus.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nazkzhib.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zhalwdss.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cskyxbso.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zhucjgck.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jwuasgxt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bkdrrwge.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3umcuiirs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mejhpnxl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vlgwvwii.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3knfcwsgy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3sauqqhcr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lpapdcgr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jvhsgfsh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qquxeibu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kyqbgybn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bxwruosw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3irfowmsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sybbbpss.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zvzlcmbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpwdgkoj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dcqinagg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwpjblgi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hvaccrwq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xpgryxhh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vjpxcmkg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfpiqnb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3onpdbtkr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nkxushuh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ptdgwadr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3oehpkfqk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ounrwgit.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hztlbzvj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrfbjxbg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nlzbezpg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3iqcjxzpd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iebbbmrt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3towqbtnm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gpjyepes.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hvdkihro.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ncgfubvr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xongflfd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tftvofev.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ztxegmxo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fwfnycsq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wtkcetml.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vjgrbwyt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3groxpctm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kcdvwbpe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nzksomzx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hlstauzd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zxkkrhkd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bqiibwbr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ktihsdmi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nvbcmngj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmmxeyyl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rlltzwkc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vnpqpmnb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pqgfopsj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fmlthaua.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3drttjpte.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3frnqmyqc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hepmrgho.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ytncgnpn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3knylgjbn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgmhomsh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tspqrizg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fhlqwazh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mjautwyp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fhlusjpe.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3smcksmxb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hkynepte.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3neqnlrdk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3molpouvr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lfwtinrp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pfkydepz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lkgcmvjx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fpllflfq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lxihstwl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lhcdyxee.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ofdjmtao.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3razydzwe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3yjhzygyf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zeyviazr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tpkgmljz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vczghnmm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ucmijkqz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3upnrqtfs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mdxwdxwc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ihojizlu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3idvogvcv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qmfxcbsy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cyirumge.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xvchhiml.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fwcvjdnh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jnwehtrg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3whtytunb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vrlkggoj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wczqhaky.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kbmwaewt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uhipohrx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3icyrlwqx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3iabiczeh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tekixzdp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lgsvvvev.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ogcmtqkc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fsddxybz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iebfzwzo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zcgenzfu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jprcgnuy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lezxhtwk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hipxazjw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qxalvkvy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3eyyxdsgr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3glyglsqb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lavzatyk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qyladphl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3npqpqkqx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rlokymch.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tpbsykdu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fjloiqhy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gogpocji.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3tavwqsmr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3awajxppv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3flnlqoap.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gyahrlvb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gnixwvkv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kdkctfja.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vdzvghlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3occjucba.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gxmcgewf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjygqdfv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pityquxe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bgomxlib.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3twdprmta.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3uddfhbcf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wxjhrfvt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pajtvrco.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dqowxppk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3uwrtdvva.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ykcnmixq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3enwfugzv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ainztcww.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ijogqijm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fwrqirhe.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zxckgfkp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wbsovbfa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dtkslfok.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3lyswlnve.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3anbiorgt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3idurqldm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3eonkpett.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3tmvnxior.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xxvkfbfh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3awhtuvvt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqocwkdk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rxylezlu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3brsakffh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pagxcekk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vxqaywjt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3eqntpnnf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lehlufkb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sizghthd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3znofalca.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3sdbffacv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ncsmcniy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ktuuudla.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsyoysgl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jhthkyhy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tcbzyvfa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nsduhjlz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dztijtub.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jvuuvavr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rryivjjh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zblxozbv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kcvrygcu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3enlyzybc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ihzdxrxf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cchgxkbv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hoohkdau.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cugjqqvs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wtzbzjez.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eaujtitt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zkluhvcr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wmpbnwhh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3pjhdjglk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfzpdcms.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tbtfnpcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tixeiieq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kmwxzyfb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hhfacsux.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3lxtyarzh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tdgucuha.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dhhymulu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ebwhdiwi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qpyykhvo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ztxndwgs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3drglkswg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ywogqesr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bhduhyvp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhfeyiwl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3envfkeyy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3botwxnlp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ipsvdcei.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mrnmpbrj.html


<!-- 参考信息 -->