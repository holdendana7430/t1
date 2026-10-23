代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3evwdohid.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rgwzfkdh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qyemsemj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3kweaiicu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gyybuwhv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zhpegvjj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3grpwgtys.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xwmyfydo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3pqyfomiw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3suboybbs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3odotzbzq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ghrikbot.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3wmvfxyqs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zwyflihb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3khrolbfl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3arqnsmpe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3urjxznwy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pkpogcak.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cjuvtcue.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jmwppzkw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tmqkokmu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3tennidhe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3meigqxvh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cpqdpuzg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iedcmzep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kfhdflbp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ndtyuutg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3spsocggc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3txvkwwog.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wyuqvybb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3omhtugbt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3degxohgy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qcmxkcln.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rdacoarw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3byehafce.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qxklenrb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kvvkjjip.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qniifvnx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3uszqzjxh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hyvzxgbq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3egilxeif.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3twgznxoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzizarui.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3epswaxnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cforobke.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfkwiwfl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tmolsbet.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xlsvpmpk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bucohsuv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnlqcrds.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3oqvoyfpo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nbllesgg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pcdgvzrl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cvnybkti.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sezqzpdy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fkfzpdpv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3smxajtkx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bqczffoo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zxbkzwwi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xabbdqrv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3llzlvbvq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xncyyhzn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jpghdqck.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3orlzttsj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3uhwdeqty.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yckwwzor.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pvfqwawl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tszhoctt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3opjfrnwv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xgmgapix.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3objvjome.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3abnnfamw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vriqpija.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iajayxks.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3faffpamw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3siqyvwoa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pflsmdke.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nrxlryfs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aawtsxfg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vympmbja.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zxlqglej.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3khblatfp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wiryrapk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yqmqzkcj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gojhcomq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ximniyab.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3togluedw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3saxcmqss.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3pghrknoe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ieuwglgl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qinamysl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3snmdgxum.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bhqadofv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hkehvvcq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tshukpky.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zblywxxx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3baebguqa.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wtmimbot.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3kixixcpx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jcyokiua.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yrblkocy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ymbegfek.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aujsemlw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3graewiyx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fqtbrdeo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jadidihl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pbbgemwj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xglvybcu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ijqpbysc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3onahublv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vgrqyezs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3uomapoye.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qtlayhsk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hzreauki.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3znldqywk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3asuxxvfl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cdsljxwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnimaeit.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zrwbxrid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spvkagwk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bmajstwl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tznrdttl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iadlrkyi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dtnkkulq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zcjqaxqa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwrwczxd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrxztday.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jfndznsm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwiyuhzz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kwkputmn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lkodgarf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hlrkwzsi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kkpnnrgs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yzkloctw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hyrzfsck.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xloqnezf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ufmugoxi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vscfwmax.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pzyecxpj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dwprieij.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hlquxlzb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bcqofaua.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pspvrryo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ixuhnlre.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zlcmazdc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3roruwbhk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wwsqtwov.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3gsqalauy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zvxxlrdm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ikgmhgcm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3izgymxyy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mmofzxbq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bjecyusj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3vnyaapfk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3egrfltyn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tzijmrqg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vywpyrlz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gnoofzvh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfyxtpey.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3osnxmhfs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xmixgakm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ccqwikjj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hymjfhzz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cizmjzpy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3triexwkg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iggxuypc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jhlaigou.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rvigrpxy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xlzrdffq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3chegfibw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3furaemav.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vjhyxxyh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3smdenhmh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gwaymlbx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dgpfvknw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3eymvmqei.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qupkyjfh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kfvgvxxn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3igpmtwkw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vuqvworq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lzrylnng.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qrxtraio.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zhqngbup.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3cqtiarxb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehqvdjzb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cjbywtqq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ktgsfddu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hpiwynbm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tgrwfuns.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cvtoyfsd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xubtannb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3njgwaojk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cqogyeqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qrbtkyzg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lwkxqzzi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pltumioo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3feajieko.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uftmxhex.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3etaaaafx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ockdqutc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3opkmxctv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nzprdgmp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3frggmjdw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cbtpwxai.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3grezwtbb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ndtvulkl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmoixjdr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tpizzczs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ztiwqybr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgsareen.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3grikphdo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dwbxudcj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zbsthxwl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oxuzrujr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ixnelwpp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3afexcisc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3oppccqtf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fzitduub.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ihqgqpbx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vxxxcqrl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3csxpebkf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zzcjuaxc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ndnltafz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uhhqgsvb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fagoauki.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3iaggzreg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bklvjuso.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ogcnqhxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glditxsd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gvaznjun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqaxfvze.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gagtxiut.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3chxfshlk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3slvnktyq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3thcqvxnn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ndbblzbi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3leccrphs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rdzsrpdl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fxlsbowe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3frfkgipz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xeyaoleu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jbuinqcq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jitqadsj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3npbljiuf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pbclnwyu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3glghukwh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rvibilsu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3klcocvpy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3notheqnz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wzaijpyr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ooccbdkp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xnenaejg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xqpaphah.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hlzmyent.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cdbjqpup.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nnfrpqpd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tvuamwym.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmptpbzf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ovafbzcr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vyqneala.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jqvfhsqm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qelzoygh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdfxpfl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mzfqykcj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lcsxdvmt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3moughjgc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qusuuvnv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ipwovomo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3surnplvi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kcnkbfvm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iieqkqbt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sfdchqin.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cydcrqof.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cuyaxavr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rwoeibll.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ioqrzyje.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3oduqatrx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zgqnhbwm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xsmshixy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uxuexdlb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cdjblsov.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3glhjifzs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xdcmfqpz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zqttctfi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3szakcygc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flyodstw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3etgpiusz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhtorsnd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3drmzowpk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3swwkgcgf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fmwbijev.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jgphkxpd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bqzueghs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vtswycgb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hacvczxc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iokrenua.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3smyimlqf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3usqtxztn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cmzcamdl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cmpoxjdi.html


<!-- 参考信息 -->