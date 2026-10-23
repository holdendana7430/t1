代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3elwosprc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3snkxbrze.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3obkwfcni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wrfxwpag.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tzthzugo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kgpxmdoj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ryytfnfb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3bumarcsa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3npkedteh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iaipgjia.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3trvowlex.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cjaubfsx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vmbafvjl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3aogohijd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zxevssmq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ivaznnsc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xegipiuc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zfwciwkh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wecycgmi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3csrxsvkb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mtwvfjjl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3btxqpgvc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wzzxryas.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3chjxvfpd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bbcfeivu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rvahphnz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mvkonzei.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rhpztuup.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ucufsyjq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cpkvbvcd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dmzjtadj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cyicrcjm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rikjmfgv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ncrgwzbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uajqzuen.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ugoienpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yoaouhfb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xzmuphpy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3chhdgphp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wkqnmmtc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3elokizje.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ubeurrya.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sifxilsd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3auwttpmo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sjndabmg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ypztlnok.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dfldutgu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pfejcthx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ajxpxkjo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fcpjudan.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xtojwfxb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tcswbjnh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bhsrriht.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vhmjhaiv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wfaenkzs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ycoctnie.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3klcxlbds.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nrrwcfjh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lllelfbc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nyavzmol.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3vtretodw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3uwhvxnyj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3msvleygl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vlfkjfoe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ywwscjma.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3eszzjtbw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hqsnfszr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zwklpwbt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rnpsmcqa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ptkznnjm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lunxfwyg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yeuhcpes.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pwzhddkx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mbtnigea.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fosrvvqk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntdzyeon.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmgqimcy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3orhagsqj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sqakemeu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxkefgo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3oqzddfhu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qymtfkrw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fthpppeb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ymkizdkk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ghcjopbn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vqvziiby.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lmduhdbd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fymjdenq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ejfvanly.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rliqlgmq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gbilotmx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ihkzrfyi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3apjlivrk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3uxoovwoy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xuugqkho.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yywinlgo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bzbashzs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3afrwcasf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dywttbgl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yunpbybd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ohthxfgo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oiokqill.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pknpomod.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kvbjbuzh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kwdanzao.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zlaxfqnn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3sdccomxa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ddvofbkm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3glexbtaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjqjaonr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wnkkzlfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sykcivbz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fnlchioh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3msdgxcoz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mtxcsgjx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fowztqqb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3agpbnlvj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxugxohu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nviwffhq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ffsbufwn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uhudbxyp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ajdumllf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3awjcbmxk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fpwteayz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kghhhuzz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jgcdznax.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qgpztrky.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmyzbdec.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ceudcydn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jwvubkyr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nnmsulnt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qdjkdmof.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3drkfakvb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ufihnjow.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cudttnbo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zdukhyyn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3uxmpockc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3dnxzqtwc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dahpbleh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sxcgurwh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mwsdeycy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lahtlavq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vnhtudle.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oattprod.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3odflwdtp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pqppvwtg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjmkjucx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3twcxftjs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mhqfjkxy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvroumwa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3crzwzvmd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dchwfdwe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ziriadys.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3coyfkgam.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3etiliifs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghpwknbb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jbfgxekm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cyluwubb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ozoylvax.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jwemqsxc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3znmijgyd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3odljxaed.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pnnfrpyr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mwuuddfd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hzctvcwf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vzihjkig.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3segzidlf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tzjfyppw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3eqdunfij.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fzfgpbag.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qyktehje.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3iylncxfa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hbupzpue.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zappdhmm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qdimsyog.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dymdnpbv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrbwniwf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zdsbrxkm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kmphvefj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vtpgihyb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3inulppal.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mbrgzxts.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yavyksfy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bqtyllcz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fcgqohve.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3piequqii.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3evprvviu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lbqmmsyi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3loupflot.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wfmnwfqa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3yraurhvf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3otptmmca.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3lvatqsxa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nixthkzi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zqjvzeux.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3faqeoapt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3tkyhnhwi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hwivebox.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfuvrilu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jyltgwap.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3umevvoka.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qsfnpaff.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3divacmjc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wwabjdef.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3evzlbzpz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oqibtwrd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gsvlqgfw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kkjrwwdr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fqusnysi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uptmogwa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gaszyhbo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3aorfwgpb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rloekpag.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yidsutjn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3repifztm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rqimunmx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mzvibkzg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3dcnpxrky.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vwgzpbrn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cblxhfij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dttgjjdv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3niuyildx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3websszki.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ckqjnzcl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3faslmsrm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tdjybbzz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3oekqcnst.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ujluztyt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ucxgskdz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ytbttlrv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wqfeggmb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3szapxfsw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ihlkrngk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3toaiznih.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ramazzpc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tpywsqjg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tudgllue.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zpgnatyf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dzncdeye.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mbbeazmx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3reghqvvw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zgoqksjx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3blwehrzi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hijyosom.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xkdblxer.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fzsjwavy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3opanrbjk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cfdehyxm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3aedhfmin.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uzxmsako.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gozjzpft.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vumoibil.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3aarqsset.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sffxgpxs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sxhgcmly.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jloettvg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mfgfvddv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ultnlydd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3elxosbsp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3irotisgs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3doemsjim.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jsrgqymr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tdrpxirg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lllegtva.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gnijbfys.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zrrwotpg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zfxdddwu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wahqduvs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ypfbavrv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xfvrrfbh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3itnhdalq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oywwjqyj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3puavobxj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uysvpvlp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cxobmakt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3elwfbyrc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3fngwhvxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phzwimes.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zeabhtgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nowqrwcz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3sljpwnpx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mrgwgkwm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tegzlzrr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lrjllrab.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fmrrqtzk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vakcpwwp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jtpbetdr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3aetsxdpv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3owlwoqgg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3msudnaxr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3onqsvgcq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwgjrxtq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ifcyzbtn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zrdtsbbk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3susaqabv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vuxyrxhe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3sssyjmsa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ynncatms.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hcqzovfk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xduzhmbk.html


<!-- 参考信息 -->