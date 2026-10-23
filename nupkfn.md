代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rzjfwwiv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hzzhdcri.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ulrmzjfz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3eaqvsodu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jfkzollw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3qdfttvpk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yoksecxp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xespmwvo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zricdyrv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jmunmjin.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3prqnmskl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kmfzvkgw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pumiaoam.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xssffkjl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wrffkcpk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gpiczuvr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3quyuyggg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3aduguwzl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3iugkvwcy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3iwoyeing.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3htxlnajd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3iibcnbrv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dyyswjlz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3runkhbld.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kyzugmkk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mghmobkh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3opoalgbx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qgoomoeo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3drtkrhii.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3upiwiflh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3nifubdnw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ywyxmyyo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bucbwemj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yiddlhrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjtdhrsp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jqrpekbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcnjmdnj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zytgyout.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3opimrwhl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3icprtmki.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gumpygho.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sibkrstd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3taoegelp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cboneghn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3fzgdluwm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kfrmzgyg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qovxbhph.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rsvmrmkd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oxbhzlpk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gajlwrwc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oreppcic.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mxhvvwma.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3setjeict.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3upruwnde.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hkbfjbvd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zxrgwcms.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jnjljqrb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3taqkexvy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3emopxvah.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3toqxuedt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3oqmkesqj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3aqsfvlnu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wgeqbmxc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ndwtaeue.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qzmrxwfr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rbvkghbw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3khwopaig.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bfucivws.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ynsmdiwn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ovxqbxft.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3clbplgtx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xfcnibbw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rghchrou.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3umdchibe.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wzceusxq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xzdwbrfz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3charhphp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3frtroadr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wjdjeeun.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmqdisnc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ddocuspr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ojaknysx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hnfkayal.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsqdjmph.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rwfibezm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3utzwxnch.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hwarsrmc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ofouxwjw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vcmwopbm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tpbdcckc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pgplfkok.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3juabsfsk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3stigkcil.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xbwlwrgg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hlbmzskf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fmppyvwf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dnvcjqgt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fenyihsx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pdpeokld.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cijugpba.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3aqjstnou.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fscmcqmg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3slwkksrf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nphjmqfg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zrapnfhj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3baiddlna.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3iznjtlzg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kxizqwap.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pajgyjbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpsizfrx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rhvpozrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dccpfeho.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gvtmiqcg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3urlyohpx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ldqsyxyr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kvvcmgrj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3inzektno.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tijhfgrr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cssijinf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3rlsneynw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dxkhnvkt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mhqmdwdg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pahqhxwa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3syjgmhpm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xqesgxab.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ozognaqg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mygggvow.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lcjpesmh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sygrbivj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ychtesnk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bngnplrj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3nrvmxexe.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3follejfx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rsoetxjf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pbtgmmbu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dwhiwngm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ujctkshd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ujrvicxr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bosmwakh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cbetcxve.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjinvuwo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3guvemcuj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rmfnyhdf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3folshcwc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3balqvwva.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3irrakhic.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrigqmlc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rsbemsst.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3askrfjyj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3upkyyuyk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xxluxiob.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lanawzub.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kntevuyi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3phbrrtvi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gmdbwolo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3djmjukna.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3azwztzxv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rqhwpoxu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xffinyne.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ydcgralh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3loomoxal.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3krhmgpdc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kijvtlvb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ibozonkv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3adnzlmja.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qvzfwxtb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vklldpeo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3etnhdaow.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kexuraqe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qqrqogtt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mxrwhqmq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3iantksyg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3tgunurfg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bacsbbpg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hajgfhtt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vxxsdvww.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3opkouhcc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bwywzznm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kvdjqmaf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3higxuvjd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pqunbuts.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wozxwcfh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pphdzgop.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nizikqvw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yiftijyf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hlfkkhkd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zyiuvqkh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yxzzmbma.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3srtenicl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3edetxdru.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3oxpmkfti.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rmevqrxv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3svrqsjme.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3oiccktyu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hztkcdll.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gendeors.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vafevqcw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pggodwye.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3izqwbqar.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3teugkbgf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3sduyvlzy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gblvulre.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iowirynt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mrzsktxu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3yymjydnp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3myjuqxxh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3doqjacct.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qxhsoecw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yiievpdx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3efcqnewh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pezrvhlv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3tllswmkq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3brktwbxa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kqvoytuk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wggrwymn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dipmqffu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lmjldlgo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nqepoomy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qqhhfijd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3usheclza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azfxnook.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kmhadmss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgyolaww.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pflonbgi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3igdzgagm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fuqfijoc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3djunbjyq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wtsjgfgf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3spcnolxm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fosyjbsu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3achboxen.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3oqtxxgva.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zzposiys.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vdcaoxup.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rqcfdmea.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mgnmurdo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3shxycqaw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ymycpbtf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fyanwiqx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3eeptabvr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ceddpcen.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ulquovji.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jpiyviql.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3yiauadgo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3flkozqyv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qaeejigv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wwgxeetq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cmtrxrgo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3svxbgimq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hfdklmud.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hqmiiqjg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gbjiiuyf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ercizxpw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gqujbava.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xfkdarwe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rhvyzuly.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3cmvzzmsz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hfzevdic.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ahybjfot.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vldpmhnp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dxoarjgz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vndgyjfe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3velbjhcg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uhsagzag.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3siuthyow.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3yjrncwdh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lztjxfok.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hyprhvew.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3uokrvwuj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3xuuwbeea.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ogmpptht.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ibgpurma.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gpsxsjjo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bijrczoe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3yyyfepka.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3tqokrakh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jdhztnib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3latjznhm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xshmqybm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slbazfgd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3djbpyrfn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3irpmhyul.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wdoqseqs.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zsysfpcj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3flonkjro.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cpmsycxd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3zkzyyeos.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gpfylofm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zotnfcjv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ykjlkfzg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bfhdrhou.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3flwptvnk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jnzdwafi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ymidymhr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qlhjqexh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pdevqsyf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hqaxtsti.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ivenoqjt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3midwhsxk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3yximlxoq.html


<!-- 参考信息 -->