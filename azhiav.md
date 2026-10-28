代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtqujyfczp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cheryme.top/gtuvoxsdvx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenjidiqi.icu/gtbdptuduz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtnuopjmwp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtdderipct.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigfzy.top/gtmcreajvo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj202588.top/gtofmaalsy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinyuanbaomall.cn/gtbknexsbs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtpiahssvr.html

[L04] 设置超时
来源：http://hz.jianghu66.top/gtquueybei.html

Py:   requests.get(url, timeout=5)
来源：http://hz.bjfxy.top/gtjodsuxwi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hfpthk.cn/gtnpkulbsx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtaxchavrq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtlhhgmkeb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jlsjyb.cn/gtmyfsdtme.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xinyue.icu/gtrhfihuwo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gotoacloud.top/gtjybyplzr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtkydcecgo.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtkfvyjwzy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cdnleiting.top/gtyiztnmqe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinghuilouyu.cn/gtxmlxxbxk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258888.top/gtdtkgdbex.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gttadicfzg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dashuyun.cn/gthvenkxji.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sysykeji.top/gtrylifaav.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.0kj1m.cn/gtvpgdriim.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.c1oappe.top/gtcqqujdjt.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtsuvlajcx.html

Py:   resp.json()
来源：http://hz.c1oappe.top/gtqvltklft.html

PHP:  json_decode($body, true);
来源：http://hz.hnxiangtu.top/gtnhylghpn.html

JS:   await resp.json()
来源：http://hz.mhx1999.top/gtnyxarjco.html

TS:   await resp.json()
来源：http://hz.mhx1999.top/gtmjdfdzah.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtescnmmzu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtozftludg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aibaodan.cn/gtzimqqifx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cucudq.cn/gtqmigebux.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigufen.top/gtiftlzzuh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtcbpiauxy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ppjwa.cn/gtngcqtqlh.html

JS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtmuhhilob.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtyekhujkl.html

Java: resp.statusCode()
来源：http://hz.jqgufenzy.top/gtbyhxptuj.html

Go:   resp.StatusCode
来源：http://hz.hnqzz.top/gtprewtcle.html

Ruby: resp.code.to_i
来源：http://hz.tanke756.top/gtjbgawjud.html

C#:   (int)resp.StatusCode
来源：http://hz.gaohongyu789.top/gtfxenkryf.html

[L08] 并发请求多个地址
来源：http://hz.yonumen.top/gtuapajcvt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtogbygzmn.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtmghwfutq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtjncwynuh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtfstvkgpr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydzc1.top/gtcovnkmot.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuetiantiany.cn/gtlawvctxr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gtbrpyfptb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gaohongyu789.top/gtnpinjgwm.html

================================================================================
来源：http://hz.tian-w.cn/gtzosukvym.html

M. 命令行 / 进程 / 环境
来源：http://hz.shuidangran.top/gtpqjwozet.html

================================================================================
来源：http://hz.jqgfzy.top/gttdtytfls.html

[M01] 读取命令行参数
来源：http://hz.zhengqikj.top/gtjepasjdo.html

Py:   sys.argv[1:]
来源：http://hz.shzxlz.cn/gtyiuwcegu.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtvmurokoy.html

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtbduyzkdd.html

TS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtaeubqtwf.html

Java: args 数组（main 方法参数）
来源：http://hz.svipenyu.cn/gtsdzugazl.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtdxvqarld.html

Ruby: ARGV
来源：http://hz.nwbrower.top/gtujhxtugm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuanzx.com/gtzzrvytto.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtwsjvodln.html

Py:   os.environ.get("HOME")
来源：http://hz.fzhhl.top/gtarlvuxlk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhengqikj.top/gthqkztqyk.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gtmvbbvaia.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gttzmvueka.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtmtwnlbgs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ivvv.top/gtkqxhynbh.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtqqjmdrnj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jiagoushi.top/gttcotxdlz.html

[M03] 执行外部命令
来源：http://hz.aibaodan.cn/gtvtkzxohe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yueranfly.top/gtlxprisrk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtxufsnfqm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtjntnatby.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gtucsvrkjo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtzvuhwwvz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xziqi.cn/gtpsvskdqi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ehwqpu.com/gtblulbtxb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cheryme.top/gtwryxikdb.html

[M04] 获取当前工作目录
来源：http://hz.guannengcc.top/gtcxjvwfbe.html

Py:   os.getcwd()
来源：http://hz.jyoumei.cn/gtabcvdhtl.html

PHP:  getcwd();
来源：http://hz.chenzaomai.com/gtgdpsakvg.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtbrufocwm.html

TS:   process.cwd()
来源：http://hz.nanxuanxn.top/gtmgjqwzpx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gtyvnzlxsg.html

Go:   os.Getwd()
来源：http://hz.shuidangran.top/gtxpjxmaco.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gtxkivmnhv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tanke756.top/gtyicyeyiy.html

[M05] 设置退出码
来源：http://hz.0kj1m.cn/gtzizluzjw.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtrirnummy.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtuxxjulme.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtbvmcyviu.html

TS:   process.exit(1)
来源：http://hz.birdmap.top/gtccawfbjg.html

Java: System.exit(1)
来源：http://hz.zhengqikj.top/gtfnvmchsj.html

Go:   os.Exit(1)
来源：http://hz.tianlin.xyz/gtggyanyqc.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtsqsquxtn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gtugvflbuj.html

[M06] 向标准错误输出
来源：http://hz.9152youxi.cn/gtuxkjdhiy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtcyclnbuc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.feifeiyinyue.top/gtokgpnaha.html

JS:   console.error("err")
来源：http://hz.yvedp.cn/gtieogovwj.html

TS:   console.error("err")
来源：http://hz.bjfxy.top/gtvspvjuln.html

Java: System.err.println("err")
来源：http://hz.yj202588.top/gthjtarrqj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258.top/gthrwtmlpw.html

Ruby: warn "err"
来源：http://hz.yongpay.top/gtjbhetbwr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gteuptqvhg.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gtdyluxytq.html

Py:   if __name__ == "__main__":
来源：http://hz.havefunace.top/gthixprgjk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtdzwbpmou.html

JS:   require.main === module
来源：http://hz.fzhhl.top/gtvnlnpyus.html

TS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtwkloxhzu.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtaavpvykp.html

Go:   func main()
来源：http://hz.andypj.xyz/gtdkldootr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sxryk.cn/gtahmrjazv.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gtcqjpgngk.html

[M08] 获取系统与运行时信息
来源：http://hz.hnxiangtu.top/gtixnfzvdq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtblhalwdt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtlerbfsqj.html

JS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gtnecwfufz.html

TS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtjbfzdirh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gthctzsntk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gtdtsqeqwm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.haohaochexian.top/gtiafjtfrg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtqmcmoxex.html

================================================================================
来源：http://hz.yj20258.top/gthgwkqtgb.html

N. 数据结构与算法
来源：http://hz.birdmap.top/gtcmszntmb.html

================================================================================
来源：http://hz.yvedp.cn/gtnoiwecqe.html

[N01] 二分查找（有序数组）
来源：http://hz.chenlongwang.top/gtcgtmjeab.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhixingplan.top/gtxcztkrbz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtnqulfpwk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtjukkvjoo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtsewqwfqa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtvgmzjktg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gttmjzgawx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtntakxgko.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtzpilbmkd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtcwfsuesk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtkidcgmnz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ybcxt.top/gtfltjhxgl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtvilwrryu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gttyxpwqof.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtxcfrptrq.html

Go:   slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtlcptdgzh.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtansvaptm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258.top/gtyvmcccjh.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtyolivupb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gtfghhlnao.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtvjnlwplp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gtwmudqobi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtxckyvqtw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jianghu66.top/gtevqaipsc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.svipenyu.cn/gtorotaxfm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigufen.top/gtaaypsati.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtqfvdnbop.html

[N04] 斐波那契数列
来源：http://hz.jinqigufen.top/gtphaggzdf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtbifkjrsj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtqywduikm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtbwttkvhk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhengqikj.top/gtoygbsilz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtpzfowwhw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gttlebpqov.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cdnleiting.top/gtitatjyua.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtgbrzyagz.html

[N05] 最大公约数
来源：http://hz.sysykeji.top/gtmlcnxrrq.html

Py:   math.gcd(a, b)
来源：http://hz.yangfankeji.com/gtjpcmnkry.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gtorkfvxou.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtzogbzjeg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtftjxgqtp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yanxiufei.cn/gtquophdts.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtpuozlhcn.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtoexanwci.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jiagoushi.top/gtknmzvnmd.html

[N06] 判断回文字符串
来源：http://hz.yonumen.top/gtadscxmsx.html

Py:   s == s[::-1]
来源：http://hz.hnxiangtu.top/gtfqkbhkti.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtgnlncacl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtobnaqiyd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtevqjogog.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sysykeji.top/gthbzblewg.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtnnlfwvwh.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtdcxxywdm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gthnuzuhqi.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtzeyeenuv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxuanxn.top/gtkjxupffs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtscmpchlw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj20258.top/gtzdyfoxuz.html

TS:   // 手写 Map<string, number>
来源：http://hz.vqdsnc.cn/gtsbziqkmn.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtqrwwtrqh.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtbwibfzrl.html

Ruby: // 手写 Hash
来源：http://hz.jinqigfzy.top/gtexwbtxaf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aibaodan.cn/gttazururb.html

[N08] 生成全排列
来源：http://hz.fzhhl.top/gtpcxalbff.html

Py:   itertools.permutations(arr)
来源：http://hz.xziqi.cn/gtdzjvvgnd.html

PHP:  // 手写递归交换
来源：http://hz.shuidangran.top/gtmvuvbfwk.html

JS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtlpbpdqij.html

TS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtydxkqudr.html

Java: // 手写回溯递归
来源：http://hz.xylfe.cn/gtmzhmykli.html

Go:   // 手写回溯递归
来源：http://hz.havefunace.top/gtycrxuxew.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gtfqgrzdds.html

C#:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtshtjmtkb.html

[N09] 栈与队列
来源：http://hz.mhx1999.top/gtvimvldsg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtffdhabxq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dashuyun.cn/gtszphxjwj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gtiqybstac.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.mhx1999.top/gtrdzgtyge.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ivvv.top/gtpihsconr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zycfv.cn/gtbpenhwtt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gzhubu.top/gtuylltkui.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yanxiufei.cn/gtqzriilla.html

[N10] 链表节点定义
来源：http://hz.sysykeji.top/gthcxnwvcf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dashuyun.cn/gtmtciaiiv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtfhvkzzeh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jlsjyb.cn/gtiawqmlaf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gthzekgfff.html

Java: class Node { int v; Node next; }
来源：http://hz.dashuyun.cn/gtdpcyvfba.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gaohongyu789.top/gtqyqojtse.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fengsongda.top/gtqaxjpiva.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.guowangkeji.top/gtwpdgfyxm.html

[N11] 二叉树中序遍历
来源：http://hz.zhoulong.xyz/gtwhrrlgbm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xziqi.cn/gthdwhebix.html

PHP:  // 手写递归函数
来源：http://hz.fzhhl.top/gtwqsneaht.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtjxpyxbwr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtntrrnmtq.html

Java: // 手写递归
来源：http://hz.9152youxi.cn/gtnwoajhzx.html

Go:   // 手写递归
来源：http://hz.ehwqpu.com/gtvcripnnl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinghuilouyu.cn/gtxdrpbwtb.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gtvrbbqoaj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhijiandao.cn/gtdhjiullm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tian-w.cn/gtsqodciac.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhaomingkeji.xyz/gtlmiaecgi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtuulsafoh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtgucbbpld.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtnnqjegxu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenlongwang.top/gttduxsrmn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinyuanbaomall.cn/gtkvbofcee.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtsghcqnhh.html

================================================================================
来源：http://hz.cqqwz.cn/gtnqzleiyt.html

O. 并发与异步
来源：http://hz.cqqwz.cn/gtmjdyypma.html

================================================================================
来源：http://hz.jyoumei.cn/gtsygwhzhz.html

[O01] 启动一个线程
来源：http://hz.redwolf501.top/gtmtqrerrj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydzc1.top/gtykgszzfp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.smart0.xyz/gttghfyijh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gogol.net.cn/gtjmqwbwlv.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtamokyava.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj202588.top/gtkvfilwwe.html

Go:   go f()
来源：http://hz.jinghuilouyu.cn/gtexwwqaoh.html

Ruby: Thread.new { f }
来源：http://hz.ywan-chungtsiang.top/gtwzbofggn.html

C#:   Task.Run(() => F());
来源：http://hz.tanke756.top/gthkvfurdn.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gtjrtsoxcc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sweek.top/gtagnpinfb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtaqtivpxr.html

JS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtuosphhlt.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtozhdkaps.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtsgrraiky.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtbzbtzkap.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jlsjyb.cn/gtrdtoonwk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gtcvauqbed.html

[O03] 加锁保护共享数据
来源：http://hz.yvedp.cn/gtpkzkqyym.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtnuocxikh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.bjfxy.top/gtoudweqvp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.bjfxy.top/gtvfvkbkxo.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtcxkcosoo.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenlongwang.top/gtqdhjhbvo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.quarkkingdee.top/gtlfgextgx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cheryme.top/gtcxxlhonq.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtcyqioyds.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gtsvnwhyjs.html

Py:   async def f():⏎    await g()
来源：http://hz.jyoumei.cn/gtyblhnjiq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jianghu66.top/gtnlvwpfuh.html

JS:   async function f() { await g(); }
来源：http://hz.yvedp.cn/gtfcwnpghc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sweek.top/gtcotqkcwd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.vqdsnc.cn/gtnojczuno.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gotoacloud.top/gtndgizrtz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgufenzy.top/gtydesocur.html

C#:   async Task F() { await G(); }
来源：http://hz.redwolf501.top/gtukpcxrxg.html

[O05] 并发执行并等待全部完成
来源：http://hz.kuanghao11.cn/gtmtylcrok.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258.top/gtraeessbr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangkeji.top/gtgziftgdo.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtnsvhrlvv.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtkcfusijl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinyuanbaomall.cn/gtiajflvdv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sysykeji.top/gtfncyeewo.html

Ruby: threads.map(&:join)
来源：http://hz.gogol.net.cn/gtmbjbqavh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.haohaochexian.top/gtjiubenqj.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gtatlgwaox.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.meibo888.top/gtinxlfrpq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xinyue.icu/gthdjfvosy.html

JS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtsypajqyd.html

TS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtvaucisme.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtvwlfhkek.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hysaishi.cn/gthlxqkjtd.html

Ruby: // fork 块
来源：http://hz.iojbl.cn/gtegikonmj.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtgxwpvknm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgrmyfvkv.html

P. 常用工具函数
来源：http://hz.jinqigufen.top/gtntcbjsfq.html

================================================================================
来源：http://hz.bjfxy.top/gtuuzqlaic.html


<!-- 参考信息 -->