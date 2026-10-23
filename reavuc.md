代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3shzxtwis.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3afpbxsxo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ixjzmnmk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bnzzfapl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ixgieojn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cljzmfuv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3epgfnkpg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wjumdxkg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdaaovkh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xseaiojr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mivtkypn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hcejjnld.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ybrjymze.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ztdkfojs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3opjzyehq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ewbgusut.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dbewnklk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3irqupzkg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3phoegwoy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wfxfexcz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3udofeqvn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3akxxlpdq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wyupiqke.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lfyuygcr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hkyagbkj.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fimwtela.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zlleejvs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bgiibxjv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kinpdjgn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vdxdwsjx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xdfxtagx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gxxdxdxm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fgzdocqv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ptkhopuv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zqpmxejm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lznipcxq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yvreerfh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3npbcoyms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soilbslz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3suykmcne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwlqdqzj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3meifdoly.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qjuwahml.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mbduijey.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwhyfazg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqqyhfse.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lcethzqj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3usaigkea.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vgareysb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3balpfdgb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lnblfouf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vocalofn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hkpsophb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qkntlgad.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mwbmiwlx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gsufwtan.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tjizwscc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3glpzqzmw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zqrqawbx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bamlamvp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sjzlmnnw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kufhmxss.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qveqcvcs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nuuhooso.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bnjxxuoe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ndivhedt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hicgpltd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zffkrejx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3icqmidxi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yzbqoasd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3eoypcpyl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ckbyamrz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mnkrldfw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3khudrrza.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lxusjtva.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pvtamqjf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dtglurvx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3utdohxvr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fthslvgq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3njrvslre.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okfbswxq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gxilhsgg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kpmprwjy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3raprecto.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ndgiebai.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ofwnbpjw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tztbohgx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubbnnsej.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mlddbybi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lvizzghx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ekphqrhl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xutrhxkb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fjtgeaxo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jedfnilw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vcrbjjzz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wmbjdftg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3aqhwrmyj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vbjuowji.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hvxjsexg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iighzbla.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jlnwzlgg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xhivjxzp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3iqkyyoji.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ejtzkepk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cjvmkbqx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rdxnzmmu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3premhgcm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3avhujnsi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rpghwjfv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gmkfmgww.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3teoeijyq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3brlnjxkg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3efqzhbec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pogmhnqs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3plnjijft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmdsfszh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ybjyjntu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uzunzgkn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cajzkvon.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bqcspnfd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ldbllsbh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cxzhtdxe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ghasywmq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3rtfqqzvt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jaogpwyh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3exvpplsx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zdzdbpdr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dnnqxgvl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3umzyxobg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3slpilsnz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bthodkxs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfglqgep.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uweghjde.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3odvqzkgy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qgxajwca.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vayyydza.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vjubusfc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ycpplzzh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wjdiuinq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3digkcqdw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hedcbtnh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qjfpatky.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3opdfqqwc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3swbghekl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yctmoehm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rraftkqh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xbixunzt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cxzemkjw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqwgcyqs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qajpdehp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dolicpgv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rklirqvn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3drzjcgee.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pizndvgk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvpqyflg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fntkienv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dsovaabv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3aaddhhbc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3urhbppdv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jratvlqy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3iclxnedx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3emjtjshb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3blkohbuz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fliaiutl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdxnwmoc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eskweplm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3roeiklyk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yucitjei.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xenktwbh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jkdwtmyx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pqugtdcu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3amgiqvzu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3awbrgocd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qwzbyoma.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fkqzzrcn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vdmpcxnl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pghlfgvq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qmcfksdm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vditvnpd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wehwmyul.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3eoesaaic.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mjvxmmmz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uhmqffbz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vytiqwgb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3izkiyrfx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mhnmfjbg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3fdicskkr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yosnxehr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ydtslyxs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vujdyomf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vosnpzqg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zbendule.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xbhyuiow.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rbrgpphd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dkmcnpqg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3awkuenkh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vhsfkdfr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3doqutebj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mdcfvhfn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3boqbbgvk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jbwhjfep.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hqpealrj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dwtaawvs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dtotseaj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rmkdloxc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kdzbslaf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cjwwovpf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3hwnptast.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vvssvuoc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vodinakl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3npyoixjj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3aixjwxyr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cpmssajj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bdqneasl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3npvhydsq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3dmjjvxgv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nqeqejyv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3klswzhww.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bvifrqqf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xbiikowz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3icuitpka.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fcjybuhg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gxynnrbc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ajpbldht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chhszbwj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3dqrswxhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yumrtcmu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ztwjzxub.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3yiwlvuls.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kfctiiru.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mztjbbfe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hyjydcww.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3emjazlez.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cigotjos.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3prrooulm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ahzxwpie.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pxqcpqeq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mqxmaovg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3htvlkzus.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pfuruwon.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pvsiebgb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbjanud.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lvhamhpl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3iwaoicsg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mtyopthi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bjbjikrt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dpvegrff.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wfcbkeeu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3phlnzilf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jxnepvnp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3heciclpj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3meuvodsd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yosqaweb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3grrnelcj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fttvhszy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fnqajnre.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lbjkyour.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuwcprut.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ohwufqnh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rwshktgs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fxcpoclb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bdqmjosq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nffdmvsl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3esivdttu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3aietyxih.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hwtmwoft.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iuhdpkkd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nmcaaxzf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ylltsvhe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3pfruzuwx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ssvrirpg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ucmdwise.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ckvuhzsq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3zpuaowoo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mcgwmczg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tmkrjrqy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bcifrzkd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kuglfxhh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tamrnsxv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nagenial.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3uxhqfdcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvjzjjge.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmqwfpri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unswgcyy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pyakidkw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ifxerwwg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3igyiuome.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jkumnvlu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bfwgxter.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uymuraxg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wzwmzodz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3epnqeihv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gdifyequ.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vzlbpuwx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3msbjfrqy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ezavwxem.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pbmabjyv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3uykjntop.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yyafnusk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tqltqxfx.html


<!-- 参考信息 -->