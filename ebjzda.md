代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cuuoinxw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3iqijvuzk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ywuxhhyj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3daukwxvd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hgfzkexv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ytpkixdw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iacrfxae.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qsgetpjo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3qqrgtggh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ffyqzhxw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pcdgwiqk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aguxbfwq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tnabrqqi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3erdoddub.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kadnegfn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3urwmdwuv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tfsbtzgj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ixrjhmtl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3yaiumxlv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gtbmrlpj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jqqwglmd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bsskjskf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3afgadofd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zgyairxr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rvdjplgk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vooxkaie.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dwihtlvr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xpmzhwlh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yzqioyou.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3foyexnbn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ctirrfvv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gfbcctem.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eieqgqdk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qaqvlfmg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qmvzaioe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tltwixmp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pbkoyxkt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3eswdqiso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnmbzggn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3asbjhbkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbidxucz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3psngdarv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dbivxsvv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3pogsfzyl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qnkocblk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3artysgig.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3togoirtk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rqtckttv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hekklqzc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3osnhirue.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mffkfagw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wyynvnhk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nydqqfws.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3niiqfsnd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zzgmoxjb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eamrodue.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hrjzrlzd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vibczbeg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ghrlktlt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nddsjfgj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vrzibqxr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3htnjjjkk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hhjbmxaw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eqedhhvg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fokeushb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kauzlfil.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3tqknjtri.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jsqrcfgv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gltrhlut.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jechfjzl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dvktjlru.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3izkphlbi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zuhbzasu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hbemahor.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jqgdbtgn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rlpbncun.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bwbqmwul.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3upxtubgx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgyapxgp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3afcirdrd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wcltwvzh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wbpjtofg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfvebyzv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxgrtvps.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yohqowks.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uxtivwuh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cfplyemy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugewjelm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bnuurryi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3legoxxqg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dhapqnff.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ypqklggz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wwwzwsce.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3clkcromf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iqqlojuo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sxsgwpcn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pxkeswcp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3didysgtd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hgraprmm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wmxxrxsh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dpdscdqp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3etraothm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3txhtgynp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3idjqarqm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kxddfnom.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bmazbfys.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lwcwvpjx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vhqyawgr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ncuunavc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nwuklvmu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ehsthyca.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hsaasbgo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cqavkjvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzuenays.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xhusdbms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpzlcmww.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pkdigtgu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wdktnnmh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qsiwqsll.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qtmsjexn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tilhlzli.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nokgsvpq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wripdmdv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3suhlxixk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqxmbhos.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ydqytftv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eguagarx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hczzlxzi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qaencvdz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cnezdrnh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kjmxgvwe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hexuwhja.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cyacxxkg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gtnvneiq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fwkhtmgg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sczihdcz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wxzzbmis.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sakdhhjz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dgvjsiuv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uqfncvmi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uryegrie.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vdawbxen.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3uefwddfq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bvbsbxdw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zallhuaj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wwupaaty.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fkajmkbj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ipuynims.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jrgghrje.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kepeosiv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckuqaoes.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ceqvbdkw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rstqoada.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzjgyqr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3elgvaswl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rpfwvqdg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ktfbpfnu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tpqmwmxg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3uxzjgwuc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sggshdqf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhkpuxhx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qxjnkcpc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ovmgkkwq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hnxpnwok.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jxwnbflk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nkztkzmm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mmzuduxj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ryubsctu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zcybizll.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uptniggh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vfnttklj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vxoysmkv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3miqrcnni.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3movfmcnk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3aicjrefb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3iedlxxem.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kbdbjugm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3eazamsfp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rfdtxuka.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3nlchyadu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ypdvziug.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3myfhqrho.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ygiixveb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3febylroo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3azwoyeyr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wqlfbsek.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lbuclxqh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nktthvfn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vjqtbian.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eseudcxu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3emttirsl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bxgkiovu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3acpffdiy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vspmjrap.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ixoyjsun.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gmszkxlp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pdlywljl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rzrjjjvs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cfpermjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3knvngopr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kveliyzq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qkszqzrz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqksjcqa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rjszkiic.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ivgfaxvx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mvhkduoy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3byirzcrf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ieyenart.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebegzarw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3srdfygtq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jjehejxd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lkalbktp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ghrygmwc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ylnvgmjb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3itvpiqsp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mrrxjdbk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wnmmnjho.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ricyoxnh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mvpybcmy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3spomtjdx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vpmdldlh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3afmsngji.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wpasibin.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nfpizfhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drgfqfhw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3smptiwpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebhtwwzh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cfoneesf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tasdbxyb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3undcrqhf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wgzukmfb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jxigikuw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gsrvpvqw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bvwtdxbe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xvjyjyqk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wsvcibuj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3crgxqhrq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zlyyaujz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hzyuypir.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hrncduwc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fdbvxvda.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3akxsrmmj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gdpgiekx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gfivgukd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qamcxnzh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lytyshke.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nevmpdgv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ynukruho.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qvbsggni.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yoflqjus.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jjiklmsi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ynyjkugp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mqtlpttr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxtrknjj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dmnrzdsr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3blrphdzl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ylfhedyx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3emikpbid.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxnbwqr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3atzpjhch.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ocmqcrpt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3sktteuub.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vjmjpuql.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3jdufzcsw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3skmqpxye.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tclubesa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxyzqjw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3turdyjon.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3dhhuubvw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3talkfvlx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yjfiikas.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zhewegns.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3inbbwiwl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dqyiieic.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3gulfmojs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kpjbtamv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ycskfawt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ryohquuo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3oojrcahr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3cdgxmxzr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bvyreaeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pljgipzr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3uimurxoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjgeihmw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mitqorij.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fplxhjaf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3osbddwwl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iahxmkkq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3izqpdwiw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dnvrutje.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3widamfux.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lbcmyzge.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3degqkymc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rmtmckoj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3czsnxgik.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eeyzrqgi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3obfqkzwi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3euvihsnm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3knnumncw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xuwvrdqo.html


<!-- 参考信息 -->