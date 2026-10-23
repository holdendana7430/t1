代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3noibysgu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xsnwacjw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jcqzvafj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vzmsueyr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3soqierkq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jvileoqo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zeydlnrs.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mvfqynds.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3upvtmrni.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gidzjgwt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ovgbhoue.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ydxwjlvu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bdfoavoe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nvzxnuzq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yqojcqhe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3usvsebwy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hckacato.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kkhvnqhn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hsgppsbt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qvllrwcy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iriqhpuc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fjppjfar.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kpitgoys.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ekipphgn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xwttfnto.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3woitjjjt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3sfawyerb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3nxyrdriv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kbahsaaf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wsrbtcqe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hcrtvnzt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vlzpdhey.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3odfarxau.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wmrayucn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flsvbmwv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yjfqgqct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktrnysqw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3onmdndnz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vceqlrne.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rozhglip.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpmuighl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jhlouedl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pffhcpad.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vxtxqqmg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kvepgmpx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tpojaeca.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hqtzkmwa.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lkuxcdng.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vykjvgbq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ioghnxic.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ursipcrv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qexegtaz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hvhtghcs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pfmbyyrz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3msrbfkem.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3huwjcibb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hztsgrwa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dtukstni.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qnbiguqm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fzlqyjyg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3joahswof.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ykfbgwmm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3byaajmqi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3yjdampwj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lzfsmcjb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rktcemyt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3iriqctjx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tbhomcwq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3etnpined.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3raujyfzl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jlpurcsp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qdnbynwf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ghdhagqb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gculcxlp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtqzyred.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3paeslyhb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cuydodxm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kiyqfcfg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cmegxlpt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gcrncovx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ghjwvqqe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3afgstxjv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ibrcqnha.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bpmmdvig.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qpdavucv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dbmalnie.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3epujffpk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3svfytmwo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hozlzwdw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3taarqbnh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3frlyoakh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gejfbgat.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3phwrtrva.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3nulzhwxi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sxmmskka.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3isztdmyb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sgggxxai.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3deqyeqer.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dlkgxquw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wuugvemp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ealwnski.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dvoiroja.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3thpvxszu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3esvjpvrf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3knakkams.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3fuosiext.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fjomsjxf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kuqxysni.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fcxokefg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epqzipux.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ufkowcqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aakngrmg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qzjeycmi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3odrwstwn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3arxemyrc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3otyipzaz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bjpysuly.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ubddouab.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gsvnocnv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pjcldrla.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkeuzllr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fuvurcfp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cmtfjeac.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gyygqegy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3chfjgjlc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cbohfhiz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tonbbaik.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xfnuqkya.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3icrfnjau.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3angnrkab.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mhbwtxjx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3afwyynkr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pmvbcffw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fynegfwq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ezzfrvzn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3yhmwwtyb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3eupawiey.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wfqkrdpm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jihiejxi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pennxkgh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mrymvrol.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcyxqwvj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3utvutzpy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dfbuhhqo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtmastr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3udewtuqz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mwrpfogm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3txkyilvj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hskkbhwm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sgsgsrlk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rocqgdda.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnspwihz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtkinfmc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3npkkaxxy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zwmwwdxf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dcdoldql.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jqarlltb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3yocbnzhu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hvyijuje.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zrcqzxlu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kuqsgsnk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3drgvoxfx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kzzqxsvs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3edtpqhkt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3adwkqxvv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qluimxqi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3liazxkxe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dsifnurb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3uqntuqqz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3otveevxu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wyuenwfx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mbkwcnqi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3goawkrzo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hbsljoze.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ubotpzre.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3cledntdb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfstpsha.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ptipzqrz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cwwazcux.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pxzvgxur.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tylcsyfn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lszlfwcy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ikbqqvnv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3umziroub.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3plgqhegr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wvevbpax.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dnrejeeo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3crxofzkg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wgvairvs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jlbvzdyl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3vgdwauvs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpnefrzk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cjrqjhrh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3edmartre.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cpbugdzh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3borqpfak.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3aznlfggn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qglzarih.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hufuejir.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zfqhxuyd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3stanxqwo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipiqmonc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3eitqjsyv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fsvgfznw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kvxvomvw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iwzumwxm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ynoavcci.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yivjgxuf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ctfeyssn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3faiphfni.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uhmobcms.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nxhhuvnu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ixiqdtjn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pdwddebz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qwfinemg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ggsdikjr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bvdxouue.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3asrcvena.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cwnmmmhl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xwoovzhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzzuidml.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vyaqoeuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxkqzpiy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3sfniigwk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ugzsopil.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pqrhmbsz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3alxrhzeu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sqjjmhwq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lgiuvyej.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rhgjrosw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tjnwjlkt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qfmmdsox.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wuzdojbd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dzicqbtg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3blpdbfuu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oibavsnq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zmcwkqzu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xupibkoi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hlyegvcd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kxsotrly.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3htdoloza.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wogyqmwp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ovbpwdgv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3polygtke.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xushwysa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3brxkrgtb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiolcoes.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ebfkgugv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3flqclogz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dhrqzdjy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uasvhtwn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kesdivjx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hediiqrj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulxmjozj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mdvzuodh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ggdarfaz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3guwwlcoj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vcbpfise.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsqbwtdh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rwyefspa.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrhwnhd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3lnbgaptf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vfrqnofe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fmmeyvhq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qxaymuet.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ydivztob.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3btmdlxgv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjgkjnd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3rmbljtfr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lngitntt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjywzcpm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rijgdhhd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3oprfjpnc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qmcqztdz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3azyzmktw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ruegozwv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jtmckmsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bggrvfgy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dcutwagc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvdxojrw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rbfwincb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hcjpfylh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zgfufsdk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bmsjjful.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rffkxoig.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tgmhaadj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ivxqducn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3oyjmjqsw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rceklgbu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gbddrnpu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wgeeblat.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3erowcvvi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jcypezvj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lldckmhj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3puchtucs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3oomdkjji.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vshwqzcj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3iuturpry.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zhfxjjpi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wyilwhkt.html


<!-- 参考信息 -->