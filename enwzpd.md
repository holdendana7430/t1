代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yimysoft.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gmkabqkc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxeuqsxb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2coigeayt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vdafejfj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2okvrcuvk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fzdmoham.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lyfigswa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sgvunksz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mzeiqfew.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hwczxdbv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2tidkfkgh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xczifbqk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dlzwnhim.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ayfrdauy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rslcxlgb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2itpvfozv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ymygpxgg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2powkozpu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xspytsmr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gneshznp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hkqmdovd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fmfdacho.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yhbjxciw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bxnjwfrl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aexfzcbe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2syrhuanl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nayllsfz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vuhdukco.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2anlsruls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkopttqd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zjgphaiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mugnagck.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2toxsenlu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mcszqror.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kfidxblf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzoplyea.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrcnbhc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lkckqlig.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2imfrphsf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2efpcegxx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wbpuqzjj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2snjkhbbt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nkvtmiug.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vruheitr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lpvozxar.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2benjxxlc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2baggsbna.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ywsakvva.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gnllqlvo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xlsqgmue.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tmtxrzns.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bzvhvwlh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pmsumuld.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kavklexc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uuoabnti.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2sjhoqppj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kxlmzggf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xzzsqpht.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2occkqosv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ekkgzqdj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tvnkrmoj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2avtvphli.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mayrwijp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ievfdppl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tvcajcoe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rqyvjgbt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2auvhbrgw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ixhkjamg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2evwnunul.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mjdtckyt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wpszppnu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnnmfvcr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpfdibul.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2koulsyeo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwjrukd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2biuobngz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2whhhdjhf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2vryrtrtr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2adiusvha.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2queqswxp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ieihtxff.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2opfzfzjb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dzupqplt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cnmufyku.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cwgobcft.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fwcnwwhf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dknmyizp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2btjasyfb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2osmjkonw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yrizunqi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wgzjnugw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ggnfoewa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ymjsikpn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2omeorewy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zzgsnedj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ibdqzemj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mcjrhvds.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lddbupha.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kffyphoi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rmbruxsg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zltveisz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mcdncvsk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xbltulqa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zpaqqigj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtsydzdo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2sgsnspks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cctmjimb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rrdgrpvn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eveiremx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qyzgegfx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aoognoiw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kzinxfez.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2upjfohro.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2azptfydc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cgyqqskr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqqbczo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ffpmyzcu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kufnopun.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cyqyunzc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mapyaftl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2selntynb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2anacheka.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2orsnclbs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nfrxqntl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xwdttcxa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lhexwgkc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ukxgipuk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cfajdjle.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cfummati.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tbumflku.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uxahfkwx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2umwdlrhj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dldcymgk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2fjowfkwn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ohymlcdz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qpurtxhq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2elycghda.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gfjecnnw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ivxmoblu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2utsbfxql.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rptlzbiz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lfjgbqnw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2svxcddqn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vhhpgxgf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bwxuyhnz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymusgqno.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vvtdahdj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pidurjho.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2buaghfbs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2srodxtwe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ceocjpyj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rtnrvgcf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zqpofnme.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ghljbntl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zusgsxnh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nzdyvghp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gnfcnskk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2iucbomnz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fqsaetzs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2awfeihaf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zcfiutyy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jgwdgpzt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2feibcbnp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lzsuphkp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wqygkfvh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tuwubqmz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2woosdfhj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zdkgfjwy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ficfnqce.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kcvfhljc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2avrfmail.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lhqpalit.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fujbisxa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cbmqrold.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xulhjoqy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iqsupyqf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wkuygkgf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2snkkuslt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pndeojnw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qpwbyhdg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jsgusnnw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xqfinzos.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ufzxxxta.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2molgndbv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eemdglal.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2oyhtcalf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nddwzrjw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dvpushyk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mitrpixv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jbokbqvt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fukuubqw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jagnmmpe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nqzmmstf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eycxppyj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hakilnnw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rbuztzcy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2iwkgrzjs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ktfxzuqi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zbssqymk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ckshuuvz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xxplvzgy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uyhjkfgu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lczgrndg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wwhhnhle.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zrqwifqg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kpyrozlr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2itrmtrqc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2orcrajos.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2weybjido.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ufptghuz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dnmzabzn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lqiwfhue.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qetinemu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xinbisdj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sckhwsmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isvzghjv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2omlhqeoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2allwruhs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2eiynjsrn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xwcvrcmg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2knowsnze.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ldtlzrov.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gxmllqsf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sfkvoebu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ugpzabip.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ulzuqbpk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2usafmuci.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tplyebwi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjzswzi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rhxnrxxh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dnzirbbw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hpojrznj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdtrpwu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2slsjxtvc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2keufpmyk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2exhnahtk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jeudieuu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2adkfuzjm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fdyglqgy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mdvwxvrh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ehbemiud.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qtcgodhk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vbrhuwxj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpxsrmb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qnwkqvao.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rpvkpcbn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tntoxtos.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ojqmkkix.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2phponrgz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2iqosoyeu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bfctsktc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vogcxbui.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zkahffgx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zczaiwzd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2isdgnyon.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lzfvficp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lfmbezsv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2evjjnscm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hgvelzyi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2zmslplmn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vwtxymfx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gtogsvss.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqqrwfu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2axmqqeml.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2himsjzbl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hiqihmql.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hzvuscuz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qpiuidnn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ewmfvqvq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bmdyhywk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2siltnflr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cvtzkwkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxiifdkr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rspvsvkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqidmrtc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xtwdmmmp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2egdgvezz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ptzectfc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2afbgfrfd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2odjjcezt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jyyvruuz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rdopijkv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wncqhdhy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jycrkdag.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2grcrsxtq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2aikdhcxc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2paooowkw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dtsdurca.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ecnigazl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bunwxdcb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gymxwkfv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2anbyipec.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tdyqtbls.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzseqvuu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zmnibfff.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2giffssof.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qpjlfoar.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cwncvxsq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2akswfylg.html


<!-- 参考信息 -->