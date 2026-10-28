代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.hywenlv.cn/gtpmpwwmff.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtgagzzjok.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtoqfdgldc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtshnafbbm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gteeppjxts.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhixingplan.top/gtyjejqfsh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtnngoopwf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gttreokggc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtlzmsnogn.html

[L04] 设置超时
来源：http://hz.gaohongyu789.top/gtvmozwkqv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgufenzy.top/gtlvyfmxuo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yongpay.top/gteuzdjavz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtelpgfqgz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtlecuafoj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtlbxdbzlc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigufen.top/gtduuwdepb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gteqmjbrly.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gtdtzgbksc.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtdzuegkkc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tian-w.cn/gtgoodifbt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gtxzdtylug.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtdeqiwjhp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtxcwwaqge.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtsbjewlev.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtkpbiyoav.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtdwtzuuag.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.9152youxi.cn/gtwseuiecj.html

[L06] 解析响应为 JSON
来源：http://hz.yongpay.top/gtwtdeoddi.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtxyzjvrgd.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtmrxtbmwq.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtakqeerkl.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gthhrgfeal.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtqipwqgta.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haohaochexian.top/gtbqsclvio.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pycfn.com/gtjzoizofw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gttayyayvr.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtgahbjkuu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gtghgvqfwf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.c1oappe.top/gteskebiny.html

JS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtvyafrycp.html

TS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gteiyxuwli.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gthsynonwb.html

Go:   resp.StatusCode
来源：http://hz.aizwys.cn/gttbxilbyi.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gtdtytplkj.html

C#:   (int)resp.StatusCode
来源：http://hz.xinyue.icu/gtawuraufg.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtkvfchxkk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shzxlz.cn/gtqnlfeqzp.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtkneihjun.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtekjicnus.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtyliqutmn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtnhwdrcbt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtbveeednc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gtffkoadbx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenlongwang.top/gtstzwtbit.html

================================================================================
来源：http://hz.52xcode.cn/gtilrwtizr.html

M. 命令行 / 进程 / 环境
来源：http://hz.cqqwz.cn/gtoseifkec.html

================================================================================
来源：http://hz.cashguo.top/gtiouusdsc.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtrelcmkxj.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangtech.top/gtjjpmvnfm.html

PHP:  $argv;  $argc;
来源：http://hz.hongshengwenyu.top/gtqxrkhcas.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtgleqjtzm.html

TS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtcwxbcajj.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigufen.top/gtclpntqvd.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtgyqdrquh.html

Ruby: ARGV
来源：http://hz.pengpengdd.cyou/gtxtiwcygl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cdnleiting.top/gtvkgdstba.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtuqdbyttw.html

Py:   os.environ.get("HOME")
来源：http://hz.yvedp.cn/gtbwjxaaky.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gtqzdldrhx.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gthvltnhuw.html

TS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtgiiqpigp.html

Java: System.getenv("HOME")
来源：http://hz.sufxvd.cn/gtqleevjiz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gttpjyhhkp.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtqxenidyn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtdjwpihps.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtvamtvxdh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtfglaefso.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtlyqtshtp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtltihfgom.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtvqsxagqf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.redwolf501.top/gtehpoaiwl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtiphebibg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtouqjcgxw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xziqi.cn/gtpizyzxtx.html

[M04] 获取当前工作目录
来源：http://hz.guannengcc.top/gtzekojust.html

Py:   os.getcwd()
来源：http://hz.redwolf501.top/gtpfboswlw.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtppvsniyk.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gtvkijfuub.html

TS:   process.cwd()
来源：http://hz.hfpthk.cn/gtlmvplzrh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtwlgbzgas.html

Go:   os.Getwd()
来源：http://hz.ybcxt.top/gtczzxaeus.html

Ruby: Dir.pwd
来源：http://hz.jinghuilouyu.cn/gtknsjhwwi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xingfuxueyuan.xyz/gtqidlfsrd.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtsupcrexw.html

Py:   sys.exit(1)
来源：http://hz.sysykeji.top/gtdyuxkyxu.html

PHP:  exit(1);
来源：http://hz.havefunace.top/gtuokjfzch.html

JS:   process.exit(1)
来源：http://hz.sysykeji.top/gtwhsszzro.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gttxucqker.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtuamyxffa.html

Go:   os.Exit(1)
来源：http://hz.xziqi.cn/gtwsmjtwtv.html

Ruby: exit 1
来源：http://hz.yueranfly.top/gtwvcspyra.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gttjvhdfbz.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gtdwbqcgcl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtxbbbesaw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtuokavdps.html

JS:   console.error("err")
来源：http://hz.yueranfly.top/gtkkycwxvc.html

TS:   console.error("err")
来源：http://hz.haohaochexian.top/gtbijlcaul.html

Java: System.err.println("err")
来源：http://hz.meibo888.top/gtzfqefamb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jyoumei.cn/gtxyrjbnfl.html

Ruby: warn "err"
来源：http://hz.shanyushiyangtech.top/gtqieerswt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtbodqfmqm.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gthlmdsofd.html

Py:   if __name__ == "__main__":
来源：http://hz.redwolf501.top/gteywbarrr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangdashe.top/gtxqtcizfv.html

JS:   require.main === module
来源：http://hz.yonumen.top/gtkhycjlau.html

TS:   require.main === module
来源：http://hz.shzxlz.cn/gtqgerdcft.html

Java: public static void main(String[] args)
来源：http://hz.shzxlz.cn/gtbgjbrbsh.html

Go:   func main()
来源：http://hz.cdnleiting.top/gthqiifqnw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zdqjudy.top/gtbpxmcrse.html

C#:   static void Main(string[] args)
来源：http://hz.xuetiantiany.cn/gtbsnorfzn.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxuanxn.top/gtczuhjadj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtmprgatzh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtteolgdhd.html

JS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtoezsabfh.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtplkgadqy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhaomingkeji.xyz/gtdzxubasu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gttxzzrtck.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daria6918.cn/gtebanzjbk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtopkhcjqn.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqqvbjgqj.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gthjydnnuv.html

================================================================================
来源：http://hz.jyoumei.cn/gtrhnxpvbh.html

[N01] 二分查找（有序数组）
来源：http://hz.andypj.xyz/gtgmvgtlar.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtphsvjtuk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigfzy.top/gtswgnujne.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtfztlxttt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtyhhfhutw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nwbrower.top/gtvnjqhzzn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hywenlv.cn/gtnmylkrcr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jyoumei.cn/gtnizebjzk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtlghdhifl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.birdmap.top/gtbnpqelma.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtqlvanscg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtnasunjuh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtshctrilz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtietrwxua.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gtonhmvhdf.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtmqhgujzt.html

Ruby: arr.sort
来源：http://hz.nanxuanxn.top/gtuzuchvxj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtguywetmb.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gtcxxntmdc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtodowmryt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.52xcode.cn/gtheahzdjo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gthvtgyyxm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtnfvigdtr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgufenzy.top/gtfvtujtvk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gtbruxyhxm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnqzz.top/gteeayplnq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtanvcyqls.html

[N04] 斐波那契数列
来源：http://hz.chenjidiqi.icu/gtawpilvpg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtsokhcawn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cdnleiting.top/gtezbkrdhv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtrbceisbb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtylhcderj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenzaomai.com/gtamlzmvzz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxuanxn.top/gtkummwurv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtpyxbmirr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.redwolf501.top/gtnwmnphrx.html

[N05] 最大公约数
来源：http://hz.hnqzz.top/gtyondcvls.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtchmlunwc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daria6918.cn/gtbkinnjry.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtviqtrcee.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtsltvgglx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.c1oappe.top/gtggxrjwft.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.aizwys.cn/gtyfutwllc.html

Ruby: a.gcd(b)
来源：http://hz.jinqigufen.top/gtyuxpfpft.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gttahdvvak.html

[N06] 判断回文字符串
来源：http://hz.mhx1999.top/gtasjpdovo.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtyjjsyizr.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtdwbaixoi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtqmqucgtk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtfgezimml.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.havefunace.top/gtvfuusywd.html

Go:   // 双指针从两端比较
来源：http://hz.jianghu66.top/gtbckzhkxp.html

Ruby: s == s.reverse
来源：http://hz.nanxuanxn.top/gtiytzrtdb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtvddgnmku.html

[N07] 两数之和（返回下标）
来源：http://hz.ehwqpu.com/gtilvfobuq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuetiantiany.cn/gtiiiwrxzb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gtrnifzcjr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtycampxnf.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinghuilouyu.cn/gtvhdjmndw.html

Java: // 手写 HashMap
来源：http://hz.zhengqikj.top/gtqxrxfhof.html

Go:   // 手写 map[int]int
来源：http://hz.ydjk.org.cn/gtgyqtzqsy.html

Ruby: // 手写 Hash
来源：http://hz.chenlongwang.top/gtdcgmdqvm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.52xcode.cn/gtbodzzilv.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtdvtlbavh.html

Py:   itertools.permutations(arr)
来源：http://hz.fzhhl.top/gtlsecxlnz.html

PHP:  // 手写递归交换
来源：http://hz.gaohongyu789.top/gtikvugjdz.html

JS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtibuoberj.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtdddeqxgs.html

Java: // 手写回溯递归
来源：http://hz.pycfn.com/gtpjftdjjk.html

Go:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtghtojrwk.html

Ruby: arr.permutation.to_a
来源：http://hz.daria6918.cn/gtxqiiraoj.html

C#:   // 手写回溯递归
来源：http://hz.nwbrower.top/gthdnqiddc.html

[N09] 栈与队列
来源：http://hz.shuidangran.top/gtuftocokr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuxming.cn/gtrefxbjto.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yonumen.top/gtlljdbdaq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.kuanghao11.cn/gtgvqufmqi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinghuilouyu.cn/gtvtsvtxrl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenjidiqi.icu/gtbtcweoga.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.andypj.xyz/gtarngopds.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenzaomai.com/gtxrybwlyo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.9152youxi.cn/gtdzrytrzy.html

[N10] 链表节点定义
来源：http://hz.yj202588.top/gthqfjxrqj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jlsjyb.cn/gthngyijsj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gtkqfxkreh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtkrzpmggo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hysaishi.cn/gtwtfjreca.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtgoluxvtq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gaohongyu789.top/gtjsnlyago.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sxryk.cn/gtlabprzfl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhengqikj.top/gtorojvxsn.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtljhmpumg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.quarkkingdee.top/gtdkrlfaml.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gthursibmc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtpgltavwj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gteuaqtdwr.html

Java: // 手写递归
来源：http://hz.gzhubu.top/gtnzdjoujv.html

Go:   // 手写递归
来源：http://hz.chenlongwang.top/gtpfqzxjsl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258.top/gtiahgmvds.html

C#:   // 手写递归
来源：http://hz.redwolf501.top/gtwsxgjknb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xingfuxueyuan.xyz/gtdopeqdrx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dianchejie.cn/gtkyjvdbyu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gogol.net.cn/gtznmnznas.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtilbkaudu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtfbeinjak.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtfaeasixr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zycfv.cn/gtvlhknxsm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jyoumei.cn/gtzxpniptk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtpojtgcys.html

================================================================================
来源：http://hz.gzhubu.top/gtrmkwhcke.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtketwmcbi.html

================================================================================
来源：http://hz.havefunace.top/gtbgomdmtz.html

[O01] 启动一个线程
来源：http://hz.cdnleiting.top/gtbmabycof.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.316326.xyz/gtdxvvztzy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ehwqpu.com/gtjsajgqis.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtlvuyctfh.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtwtyaoyoo.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenjidiqi.icu/gtgtipdhbw.html

Go:   go f()
来源：http://hz.xylfe.cn/gtnzoqvumg.html

Ruby: Thread.new { f }
来源：http://hz.yonumen.top/gtodlngcjk.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtbhzbvuyl.html

[O02] 使用线程池
来源：http://hz.hammf.cn/gtcrthiqhh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ywan-chungtsiang.top/gtkgxktfxp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtmyeweilw.html

JS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtudkxieaz.html

TS:   // worker_threads 线程池
来源：http://hz.zhengqikj.top/gtfnqupqwh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhoulong.xyz/gtzwcdpklh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shangyingyoupin.top/gtzxmcfsbx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gtrmyaynub.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daria6918.cn/gtybatmohc.html

[O03] 加锁保护共享数据
来源：http://hz.feifeiyinyue.top/gtreiojvyj.html

Py:   with lock: shared += 1
来源：http://hz.gogol.net.cn/gtaksnbcpt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ywan-chungtsiang.top/gtlrqqabog.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxuanxn.top/gtlhxzztjw.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtkdztjmlu.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhixingplan.top/gtnxfmgidm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtxgkavgay.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxuanxn.top/gtpnqslrfh.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtczrahbhz.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258888.top/gteqxddqqs.html

Py:   async def f():⏎    await g()
来源：http://hz.snrcjt.cn/gtespstivl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gttvxagtqg.html

JS:   async function f() { await g(); }
来源：http://hz.dashuyun.cn/gtklftnkjk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yangfankeji.com/gtvbiujgso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aizwys.cn/gtrftejcuo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtvfadzzmt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jyoumei.cn/gtnfkkqsud.html

C#:   async Task F() { await G(); }
来源：http://hz.xylfe.cn/gtehoqgfqv.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gtkxxpxdtd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.fengsongda.top/gttpxjfhto.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hammf.cn/gttbrnqjnw.html

JS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtkdemiczy.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangkeji.top/gtewbupakm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydjk.org.cn/gtyehqzavn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jianghu66.top/gtchgojnso.html

Ruby: threads.map(&:join)
来源：http://hz.yj202588.top/gtpbcagdmb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sweek.top/gtetbwugas.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtnuyavmqs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtilhoyyig.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gtvtnqamos.html

JS:   // child_process / cluster 模块
来源：http://hz.zhoulong.xyz/gtgtaannji.html

TS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gtzlrpnlaq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ywan-chungtsiang.top/gtowlijpva.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydjk.org.cn/gtppsrpipk.html

Ruby: // fork 块
来源：http://hz.yuanzhike.top/gtervafnpx.html

C#:   Parallel.For
来源：http://hz.zhiwuduotai.top/gtpewoaumf.html

================================================================================
来源：http://hz.zhengqikj.top/gtivpnnvcc.html

P. 常用工具函数
来源：http://hz.cashguo.top/gtbmajoskt.html

================================================================================
来源：http://hz.sweek.top/gtvltjmpsi.html


<!-- 参考信息 -->