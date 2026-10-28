代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.zhoulong.xyz/gtzeczakne.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.kuanghao11.cn/gtsgkrvqwp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gtukitweks.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtjgemewcd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtayiuofrk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.andypj.xyz/gtcohtbwww.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pycfn.com/gtcnqmjjdm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtsxdeumge.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zycfv.cn/gtmknyaxuq.html

[L04] 设置超时
来源：http://hz.hammf.cn/gthvsskvzs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj202588.top/gthxztaulz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.iojbl.cn/gtzdmduspi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtfkhebmrz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtrwfaqmak.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.mhx1999.top/gtnjbxwhrk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuanzx.com/gtflrmksnh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gtkzfkshmi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhengqikj.top/gtxvivmlzu.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtdqgatnti.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yangfankeji.com/gtsuhvdtlu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.feifeiyinyue.top/gtaxhnsvtz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtxnjeeovv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtqqbeabiu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.quarkkingdee.top/gtqcaovvjb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shuidangran.top/gtpuobkthh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gtggrwhfgv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.316326.xyz/gtfmcbempp.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtbxbtnsys.html

Py:   resp.json()
来源：http://hz.gaohongyu789.top/gtgnsmajhr.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtozuzehql.html

JS:   await resp.json()
来源：http://hz.nanxinkj.top/gtpzpezfub.html

TS:   await resp.json()
来源：http://hz.316326.xyz/gtzdpduify.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gthdjhzrdz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtjkdodcjf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgfzy.top/gtvwsnofyx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtdnzfmwax.html

[L07] 处理 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtgqhdljnh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jlsjyb.cn/gtkjvyprmf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yongpay.top/gtyfqcycus.html

JS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtwymefmoz.html

TS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtyodhlpgy.html

Java: resp.statusCode()
来源：http://hz.yueranfly.top/gtmebujhqm.html

Go:   resp.StatusCode
来源：http://hz.sufxvd.cn/gtdkflwzqa.html

Ruby: resp.code.to_i
来源：http://hz.sxryk.cn/gtghsbodvq.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtxaxsmgvk.html

[L08] 并发请求多个地址
来源：http://hz.hfpthk.cn/gtcekqgcqr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cashguo.top/gthuprlzzi.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhoulong.xyz/gtznnuxgvh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtmznplszv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtwhchyaoc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtfijfpepf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtdciaaupl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pycfn.com/gtgnpgfgvo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtxvaneypy.html

================================================================================
来源：http://hz.jlsjyb.cn/gtuzxoaokm.html

M. 命令行 / 进程 / 环境
来源：http://hz.gaohongyu789.top/gtdoujngri.html

================================================================================
来源：http://hz.jlsjyb.cn/gtwfgftwck.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtyjuvlsel.html

Py:   sys.argv[1:]
来源：http://hz.chenlongwang.top/gtyuyhrjqw.html

PHP:  $argv;  $argc;
来源：http://hz.shzxlz.cn/gtdrfrxype.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gteunfcpiw.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtjgbakatt.html

Java: args 数组（main 方法参数）
来源：http://hz.meibo888.top/gtuzmmkyjf.html

Go:   os.Args[1:]
来源：http://hz.daxiang520.top/gtagksgpta.html

Ruby: ARGV
来源：http://hz.hysaishi.cn/gtxzmqwdvf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yvedp.cn/gtsvubhkxe.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtceibmimk.html

Py:   os.environ.get("HOME")
来源：http://hz.vqdsnc.cn/gtpqpyaapm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xziqi.cn/gtaleqetxd.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtexvfrtbb.html

TS:   process.env.HOME
来源：http://hz.yonumen.top/gtlfrfiffh.html

Java: System.getenv("HOME")
来源：http://hz.smart0.xyz/gtpzydwbie.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtrpzgovfv.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtzeaunkpg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydjk.org.cn/gtqxtrdlhe.html

[M03] 执行外部命令
来源：http://hz.guannengcc.top/gtlbtaxpoy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.316326.xyz/gtzdtzodef.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtzvtextqx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtzwqbyhkd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtnipbymbu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtigcjjeyw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258.top/gtcaomcdts.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtwzkyemdp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.snrcjt.cn/gtzgyqfjst.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtmbsotdlm.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gthsdjnciw.html

PHP:  getcwd();
来源：http://hz.ywan-chungtsiang.top/gtdsazqtjk.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtjrigagry.html

TS:   process.cwd()
来源：http://hz.yongpay.top/gtmbqoafgr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.smart0.xyz/gtweceubsk.html

Go:   os.Getwd()
来源：http://hz.hywenlv.cn/gtinkvjmmz.html

Ruby: Dir.pwd
来源：http://hz.sysykeji.top/gtyobnnbkq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtsriutdiv.html

[M05] 设置退出码
来源：http://hz.ydjk.org.cn/gtoqonnnui.html

Py:   sys.exit(1)
来源：http://hz.ybcxt.top/gttjiarvsa.html

PHP:  exit(1);
来源：http://hz.9152youxi.cn/gtxombljnc.html

JS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtkmrqrjns.html

TS:   process.exit(1)
来源：http://hz.cheryme.top/gtocktxzdu.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtvtxemphf.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtsmhdesty.html

Ruby: exit 1
来源：http://hz.ybcxt.top/gtcgoqgplk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cheryme.top/gtbvdundca.html

[M06] 向标准错误输出
来源：http://hz.cdnleiting.top/gtebnciqik.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gtyxzznodr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydzc1.top/gttiviinnc.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtrhkegacq.html

TS:   console.error("err")
来源：http://hz.gogol.net.cn/gtwuljpxpd.html

Java: System.err.println("err")
来源：http://hz.xziqi.cn/gtiqapciuy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yangfankeji.com/gtoanlckyz.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtivhanwim.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtunswsfrh.html

[M07] 判断是否为主入口
来源：http://hz.zycfv.cn/gtmyciwfxq.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtuzhmpdkd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtxbbetwab.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtfwimlbwo.html

TS:   require.main === module
来源：http://hz.guannengcc.top/gtnqibmmdg.html

Java: public static void main(String[] args)
来源：http://hz.fengsongda.top/gteyyxmysk.html

Go:   func main()
来源：http://hz.aibaodan.cn/gtseqviafp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtzbvxxxzo.html

C#:   static void Main(string[] args)
来源：http://hz.jqgfzy.top/gtmskgeacx.html

[M08] 获取系统与运行时信息
来源：http://hz.bjfxy.top/gtbithltav.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenjidiqi.icu/gtnkqnyieg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jlsjyb.cn/gtjuucgjmz.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtmkhbzfhl.html

TS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtizjcwbgp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtlcpvcshf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuanzhike.top/gtacotnwif.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gzhubu.top/gtuebaoirf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gtehrqpbcx.html

================================================================================
来源：http://hz.52xcode.cn/gtmcwsfyxv.html

N. 数据结构与算法
来源：http://hz.dashuyun.cn/gtozvqddza.html

================================================================================
来源：http://hz.tian-w.cn/gtuazgcgec.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtvkzhctfq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gtjysjjhkv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtqkctjrut.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtziftyntk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtjndfyyjn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtulqgynzo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.quarkkingdee.top/gtecwuudaa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtfehgmmhg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.mhx1999.top/gtnkeytigh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hywenlv.cn/gtakygrtid.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtaryyjzre.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.meibo888.top/gtildmlftg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gteymrmqjq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtwzuieusv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.quarkkingdee.top/gtwuimbyjz.html

Go:   slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtxeyworif.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtnysetjvs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tianlin.xyz/gtwaugtwet.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258888.top/gtantynikt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tianlin.xyz/gtwjnrzhbo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxinkj.top/gtpyvxtbqh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtnsurkohj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gturqrbyjl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.andypj.xyz/gtsdzedkei.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtcujsiseq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.birdmap.top/gtnhwexspu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.daxiang520.top/gtvyeeowgp.html

[N04] 斐波那契数列
来源：http://hz.zhixingplan.top/gtdinijcfn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtrrxhupzt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gtcnarjswi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtuiafkycv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtsesyqjkz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dianchejie.cn/gtshsdfoiy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuxming.cn/gtdysgjdkn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtrepqhsmp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhixingplan.top/gtjvdkqmwp.html

[N05] 最大公约数
来源：http://hz.hfpthk.cn/gticmpplel.html

Py:   math.gcd(a, b)
来源：http://hz.vqdsnc.cn/gtawwqfhpe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jqgfzy.top/gtnpiicyjt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtpwiipzbu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtawvhkfad.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gzhubu.top/gtsqfgxuca.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hongshengwenyu.top/gtufhqjvdh.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtkhqmuqet.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxinkj.top/gtxpwdpdgu.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gtdgrrsnzh.html

Py:   s == s[::-1]
来源：http://hz.cheryme.top/gtbwlzpkfm.html

PHP:  $s === strrev($s);
来源：http://hz.pengpengdd.cyou/gtpkrnkvdy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtoqruptwh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtcycafprn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuanzx.com/gtigfdoygu.html

Go:   // 双指针从两端比较
来源：http://hz.jqgfzy.top/gthznnygxz.html

Ruby: s == s.reverse
来源：http://hz.gzhubu.top/gtqvmapgzg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtsdghnoxu.html

[N07] 两数之和（返回下标）
来源：http://hz.bjfxy.top/gtilggktdp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtphfahvgj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tian-w.cn/gtffrosfqb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnqzz.top/gtusvjidrm.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtjipfcsfy.html

Java: // 手写 HashMap
来源：http://hz.yanxiufei.cn/gtlkxjqqku.html

Go:   // 手写 map[int]int
来源：http://hz.52xcode.cn/gtwghnctin.html

Ruby: // 手写 Hash
来源：http://hz.shzxlz.cn/gtlorkfiju.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gttxqwwdvx.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gtxsfemdqx.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtpkmncwtc.html

PHP:  // 手写递归交换
来源：http://hz.hysaishi.cn/gtieigrcyr.html

JS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtpkrwfkxp.html

TS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtzmldrgol.html

Java: // 手写回溯递归
来源：http://hz.nanxinkj.top/gtgcgqlfbb.html

Go:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtfnfddmqg.html

Ruby: arr.permutation.to_a
来源：http://hz.hysaishi.cn/gtxkhebeip.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtyqfpahhg.html

[N09] 栈与队列
来源：http://hz.birdmap.top/gtzpzvtafj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.iojbl.cn/gtinlkkpnx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gtcvivqtsh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtibahrbqr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ywan-chungtsiang.top/gtwfgdufvp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jlsjyb.cn/gtbsbtxuus.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hysaishi.cn/gtoypyjuzy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gthwhowodw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guowangkeji.top/gtpumuqpcr.html

[N10] 链表节点定义
来源：http://hz.tanke756.top/gtslhofyah.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.mhx1999.top/gtumhlveov.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydzc1.top/gtiitlcyjc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cashguo.top/gtqknhpjmn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.fengsongda.top/gthedczyuh.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtxgkkdnju.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhengqikj.top/gtkiuhnoqx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daxiang520.top/gtzypvtfod.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yanxiufei.cn/gtjiorqoij.html

[N11] 二叉树中序遍历
来源：http://hz.xylfe.cn/gthwfnxgqf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtseutmaom.html

PHP:  // 手写递归函数
来源：http://hz.jianghu66.top/gtfbklnjhe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtcddyszkq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gtchhasfml.html

Java: // 手写递归
来源：http://hz.zhongyouzk.top/gtljdxifyt.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtuzvrznuc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dashuyun.cn/gtaqleeybz.html

C#:   // 手写递归
来源：http://hz.cqqwz.cn/gtrgpxyvbf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuanzhike.top/gtvonvmmcd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guannengcc.top/gtofvjhtef.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gogol.net.cn/gtxlnmntys.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtivlwhmzr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtgcnpcutp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtgpobbokd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shzxlz.cn/gtiinsmqyj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtktfgsroa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtmeghyubc.html

================================================================================
来源：http://hz.yangfankeji.com/gtryqhuxjv.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gteeclpxaz.html

================================================================================
来源：http://hz.yj20258.top/gtycaxubgn.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gtiwucsqdc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhongyouzk.top/gtfwxiqbnv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258.top/gtltenhbke.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tianlin.xyz/gtbmbmetrq.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gtpsifdjfl.html

Java: new Thread(() -> f()).start()
来源：http://hz.yvedp.cn/gtdpsljsjt.html

Go:   go f()
来源：http://hz.zhengqikj.top/gtrmjdyioh.html

Ruby: Thread.new { f }
来源：http://hz.yonumen.top/gtpddieliw.html

C#:   Task.Run(() => F());
来源：http://hz.zdqjudy.top/gtjcyqzmws.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gtxbjernos.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xingfuxueyuan.xyz/gtjgencjmb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cqqwz.cn/gthyrogioy.html

JS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtboygnysx.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtqfgevouo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shuidangran.top/gtagrtwpkt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinqigfzy.top/gtgyygkskj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gtiywiiuzz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.feifeiyinyue.top/gtajahyjae.html

[O03] 加锁保护共享数据
来源：http://hz.shangyingyoupin.top/gtwareyrir.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtxcoixtpm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jiagoushi.top/gtcbndiknq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ybcxt.top/gtncqtnohw.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtzuuabemb.html

Java: synchronized (this) { shared++; }
来源：http://hz.kuanghao11.cn/gtgitxsbig.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gaohongyu789.top/gtxfpvdeby.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtmohzgqrj.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258.top/gtydhkwnfq.html

[O04] 定义异步函数并等待
来源：http://hz.aibaodan.cn/gtfaejghrb.html

Py:   async def f():⏎    await g()
来源：http://hz.chenlongwang.top/gtylsumprr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtcjlycenv.html

JS:   async function f() { await g(); }
来源：http://hz.snrcjt.cn/gtpkdptsjf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gtexowfcqt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xylfe.cn/gtvxbrrqam.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258888.top/gtmxjppygs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtfmlcmcra.html

C#:   async Task F() { await G(); }
来源：http://hz.jlsjyb.cn/gtxteqzxds.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtowzvumvx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtgtujzqzw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.vqdsnc.cn/gtigcyltik.html

JS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtljacdbaz.html

TS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtiyarhoyc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nwbrower.top/gtwtpitapi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pengpengdd.cyou/gtxlkrfmee.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtgkuqcsaj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtcdjhgtef.html

[O06] 使用进程池
来源：http://hz.wangdashe.top/gthkiciyai.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.bjfxy.top/gtjwlixkff.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnqzz.top/gttdxznyqm.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtycoputze.html

TS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtrurnyyze.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtwqzznguy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.birdmap.top/gtvqbzbpnv.html

Ruby: // fork 块
来源：http://hz.tianlin.xyz/gtvcgcavqe.html

C#:   Parallel.For
来源：http://hz.chenzaomai.com/gtgdjdkueb.html

================================================================================
来源：http://hz.smart0.xyz/gtvhuulyjl.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gtigdooqvp.html

================================================================================
来源：http://hz.aizwys.cn/gtzfmmxdsc.html


<!-- 参考信息 -->