代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3omdozvts.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ubzhgrdk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3aowbrcof.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3pfavknqp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cebnsfat.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gxrguiid.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qhwyojis.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3yrfwtdgx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sqrkuvle.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ztxokgum.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ocbdifez.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cohakono.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yegqvurn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ajswwqvl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nlhiwnjn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3joccyvya.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3czbdmaes.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kxjolqbm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cjzjqvav.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xdcgbkhd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bktshzgx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ffjwlxuv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ajerdvud.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3syzzpkyi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rzzmwkjq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wimydmfa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rmeffpqy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bairqpcj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wlwplobv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3etxjsymv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dhrbpdgi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3postnqpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gjavxnon.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3aiyjzpnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrzxxxxy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kutoectt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxjnsnfl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jfwxqedm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jkxmqevn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ufmfcvzm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzrzkspa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhwcwcrx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kemqzucs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cvjydmbc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tcgerlxo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3txqhbbcl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpexapus.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qetqluft.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pyfqhook.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lstlpoci.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ggcqsfpo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qxemkhgd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3regmvixp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fqcartqq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mgfhwyis.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ndexnfgg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sghejwhq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ogdcopek.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iohauqku.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3icfolozz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3oendblkc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jqudhykj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sohlmemz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mibeykba.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ukoosegd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3exrlkbus.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3avlivywp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eusxrkhn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ssckaqfn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3pxldoajx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jntsegjy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wzxhrdfz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3phjuaago.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vvjlsljj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qsnrkavt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xihaxhrf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnyyzvid.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qaymkwbt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jpqrwokw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijtphejg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lqxijkhk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qzbeosfn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vtwocyat.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jvrabtid.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zjaxomac.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hfvrcqru.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3brasghbh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ajhggwze.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mxinruus.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3onmclfnp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bkuuqblp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kfilbzkz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3udqcmdvb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3pyqvekpw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lxjnhcey.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yzkmspll.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yppjytzi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mmynaydx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qcecfbpk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lxcqjffo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ipmwaopf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uaauusfs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jzjqjzpn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3abcibymf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3npodktjq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3skcoxqnl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wiuymhwp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3oqsodpsg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3lwhfzgsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vubbdnmf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tkidvxvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzhvcxvv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rilzysfy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlifnfd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yuiiupex.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qjwkksqz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3llbmekbw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cxcyvfiz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmqdcatw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yoiljcex.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjirkyvq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mmdzshtj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lbbkmfjs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rmvosclw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjehrvr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ofpacbwh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hibketfe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dckyfmmq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jlakhfdn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ftjqkmyk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hqeyclxe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zohejael.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wyvmuqtf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sfxfdrft.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3glecycjy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3axqqvseb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xxvxtbkc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xoeliwao.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lpxhpmkl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zgxnkibn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kfqmewmu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lolutdsb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nyrgbjvq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3papufcyv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rznlgidp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kwfmfxtt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqgrvdy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3smsqqnmm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vvhposle.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3twbfgvcx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nvgpjayr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbalwpgc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbasgwbi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xytssvmq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwxfyshp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nysdfyvz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmgxfdev.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wvabjvtk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lailwmfb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yjzaxtve.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kbuldvki.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3agmnvtfk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ltxjqnwe.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ngbwgwsh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3trwdjimu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rfbqhlrn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3udnvazzk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wavlqzan.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3alvojwsm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3irhmmbju.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3edewirab.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3putyyoeo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3adiaksmo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3eeztxqdo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tnnkvuor.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zhqfkmdd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pjjusfwm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wypaoumz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lckbwboa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zrkubxwd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3exbgzwrp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3abitjwsb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jczuqkif.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jpzbzuli.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cwhjxqnp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qnvjicbg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ajarlhwg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kebmuyev.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3enjhpkzh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lbwgezkz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mhxkrqmz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zkvmohbh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wyzgweke.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rydkqlzs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pnacicfg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3eshpuhir.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwomwhm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ryoqzwtz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ercgybzy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fyxwfyfg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3noexpprd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvtxpnft.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iiwmtgdb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xezlyhrx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3iuzkmkak.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dptckjkk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mixvsbyk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xhgjuyyu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qqqmftuy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3eqhudwce.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3crnyliab.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iaipylca.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3oarvfsod.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3meddgqrl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rdsbofdy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zggflyds.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lypzcfdl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lrifqyrf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aunpdqjd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ungtdhke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbnhwdgw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ccbexyrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwhxhgmw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3szmsowdy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zdgnglkt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vhszgvhv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lrkmtxfz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pqbxmvcu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3prrlykrt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vmspxbhu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3laojelsa.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bcndcasd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3iadcnpjq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3blzdgaaa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vhdjwmch.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gqbltgax.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tpoypyfx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vbpsxevc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jtcglrbu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3umojlyes.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zmlbvdza.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qyaxvbxo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hwnmsfua.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3sfkznkjw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qyuzvyru.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bzufrgpr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeruykix.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cvzzhuec.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ukfpscgv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3letpifcl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ukquvldc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3edfemxtb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dknzzyuh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsjoxtnq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnvrejps.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mggdojdv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qzvpireo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vjbkigxh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3snksiuej.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ksvclvad.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gctbcvmv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mwjrggwh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hrzhtzpc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zzbnubqf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qjdqxjdw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3femtmiwu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3djfaabti.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmgjfikn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3sczxsbqe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3iwcuxedp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ljfvegbn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xfunlapa.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3chjlwcnd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3baasktnh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ktnieelv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ualfovyc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tivlqzxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itapirbo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gmzxpeon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3autxdtml.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rvgtuojt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3phimotrw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jkthskgz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ydzrexyu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gkcbsrfx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ygehxkqw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rcjhkpbn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dpwpadls.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fkiodbmm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dbqeefvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ldgomofs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cslnpwmt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3garggolf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xexekelk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cnvsbpbj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3skoiyqno.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oirhcwxd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vuiitcdu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qrrbfwbt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ulbkexjs.html


<!-- 参考信息 -->