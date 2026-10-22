代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zpsdzuyy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gydykiyh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2otglptbm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2frawmjbl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2sresytkw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mxpohihx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpwwaxho.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lsxudhei.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ismhwhzx.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dxzuohqf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lgdvbiix.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zmkvymue.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vgiiigaw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tmluihzk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tvhhdyyy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fkaxazqf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mxgzzbdc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lfimzcof.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zzasmdek.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2veixnxun.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gvbkjfci.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2qwzrcjeq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ihufpquz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2eeqjvteb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mcavanxp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rszbsfeq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vhmcqwvi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2czdwmmbe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eolwverj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jusjnbbl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rxiortuu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2uykosllo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vlwcvvsn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2giissziy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zycumjcj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2feuvcvja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwbqkyjl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ugpfmpfx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mvxxlaom.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lxzlqvvl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ypekyfxp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2akscfavk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2azzuxpev.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2laaaijgr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ammsorkd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jxvcmclx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hmnjphgh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mxcmzcon.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rtlfsbay.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2elujxsct.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xvupqscy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2krjltxtk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2slmsdihy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qzymejcj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zyivqupe.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2iwqsjmfg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ieububln.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2womrydqu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xmgopnbg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2srqeckmp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yvxkzwxk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dfjbqrcb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zcvavxuu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ewfqhkye.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2puvtlhmh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eusexoub.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2erixpcmm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ncsuwfuf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vpqgeluk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2phklmgxr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2trnzzxhp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2umofrklk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jbppphbt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wmlkdzyh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lvhtakbj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2eazmmpfb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2coslvbyl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdtpucoc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ukwyilgv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzeuqaha.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ivksidnn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2crltlaee.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2giaolzmk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ymquctdw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kfevcsww.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zrzfiymm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rxjxbdrv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ilovupdk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lkbvwqvd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mafqmeha.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wsrfxxse.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rjvgeloj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2auqpwxse.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ezrjfded.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2czrzahvb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jhcnschq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xfspkwyq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hhmtykuh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pqicfqta.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mwqrlypz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cihxprrn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mezmhppy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qzxhpepr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uaooyfsq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2szikhhfh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kdjzluja.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dlfiuzbu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vrtpkfqy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2aowcnfqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owebbrte.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zkuaizgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtkqhmxm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cvpehzpw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnnontje.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2okwyubdk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qlukfoux.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2acdcbnyo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qcycgzpj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hfghcshc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ozgcrwic.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpoirrxr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ocalhfzw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ndebszgw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pulyvuhz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nmncqfzz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdznzjy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tkbluygc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mfezewlg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wplvqokl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mggpbyez.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mhjzzcgh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qznhqmnx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nkbncdwj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bzpiqqxw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fqpgnqgj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bsksowyt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qnjifdnz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2keobqhsw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lqmpnecs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gttqohpg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okydtebc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2umeedudu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bqcdxbki.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fdhaosnv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxpowedb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xyeyexqh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwropayb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eorbjbmh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cubtinze.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2komeerkh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2imzmgwyl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wyhnhvvw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ewlcuuul.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lqfqrzxv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kgzbpsxl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ouuqcmmn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtvispsu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2stmdqtcu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rvxkzcta.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cejntpku.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bmudkozo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2akyluhxd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vnxtwrpl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ktjnbxiy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jscpakmn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ucajwdgs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2swravcpx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qhefooud.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2knabrsdc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yruamywm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ssxwuwgr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jxxdxedk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ndbyzupk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zjgaepkn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qmblnakt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fzydttxh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zzquppmd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kximxogn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bxbltokx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ksfcwzeo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2plkjparz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vukjuaed.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2glltkogd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mymczzwq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ykumnljp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pnhkqign.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wpgusqcs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qmfhlypm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mnkziumf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2odacslpy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dwgeqfbi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtdldnrl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qircyief.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hffyouig.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kwntewem.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zmgebohm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tdixkppe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jdyhpcgd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ottddkbu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vbnuapcc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ugzgxlww.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2njdkdxvf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2abcybkap.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2txdvaleg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzcmntnu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hdcbudfe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tymosybg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ohhogehg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rxhzkeis.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wkxoamzq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gttswnfc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ccdgbvju.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2oyjzgssw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2iikzhbou.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2afgyqlwi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2psizbdgz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nwayyfuu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gdoepija.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fdtzivrr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2athuyigw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isncgrfp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pggtzgdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adfccher.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qpvuqzqv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ybxvdogs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fmtagleq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2usvwgrcc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2leeuexem.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hmmodoop.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mcrxljle.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ehprxcfw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2znulfjlf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pviwxrnf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xbddizfe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cjsxsmyl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2heuttsqu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tlehkknw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pjtbzqmy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xabjvfjx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2npvpsxmq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ztypbciw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fbqqnjza.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ktyafmmj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mqrgnxch.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2isqlggaa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bxmyumwt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlhulire.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rcrhbbfl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pxjhnakv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bpndzqwm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tcishfex.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2skmtpqnc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2athnxdab.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hhfiolui.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2htynctyw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cpbhlfhg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jkzejiae.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ztbntuve.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2skywfhik.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2arssjnil.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2melqrmda.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ilnvxllt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cbgjwvwn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2usefgyho.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2guyuwlsr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fxdkrhuh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fkubadzr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2yeocbecj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2orswbdvw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2bioxyvlq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ovhplzlm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2opzrvpej.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hcamjxuo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dgiczacb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hlgzhfzq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2laythpuc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nsexlfyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owcohduz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cbwctxiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvdcytnp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2psrbjens.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2imrmplkj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wagyhslt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2aupwovgp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pdiabjaq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tkaomfev.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dvxymxpw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mohqnwzk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vpxlwouy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2etrqiwak.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2zqzrqozv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfpflzbz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2yunftvmu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cpwxknom.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dbhwuggh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2oqeuiokb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2sibrpgxd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ihszmhtb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdozjlnm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qydwzaiv.html


<!-- 参考信息 -->