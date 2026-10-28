代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtftsxegwv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jlsjyb.cn/gtujboqdoi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258.top/gtzfhdubgt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuanzx.com/gtqngcixto.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtoasuxydp.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtfcemltio.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtnltskqcb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xuetiantiany.cn/gthoucgres.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtkpjsztll.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jianghu66.top/gtwysjgpso.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xziqi.cn/gtfbqnglre.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yonumen.top/gtgoohrtvn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258.top/gtmgyagoqf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtcoufioij.html

[L05] 上传文件（multipart）
来源：http://hz.zhaomingkeji.xyz/gtlewcodvd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cashguo.top/gtajdmjasf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.mhx1999.top/gtnfwvehal.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtqfqswken.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gthmqnraaa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtmrxwerbu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtzaepyhnt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuetiantiany.cn/gtginjtnnz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dianchejie.cn/gtgzwonntc.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gtufqejlve.html

Py:   resp.json()
来源：http://hz.nanxinkj.top/gtzuoxpfdw.html

PHP:  json_decode($body, true);
来源：http://hz.svipenyu.cn/gtkjvtbngx.html

JS:   await resp.json()
来源：http://hz.cqqwz.cn/gtyoddmphf.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtxtgktlor.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gtfpkkzaro.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xylfe.cn/gtumtignpv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.vqdsnc.cn/gtdnanuqsx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuanzx.com/gtnptesdce.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtrdeseyix.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.birdmap.top/gtnlninfre.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xinyue.icu/gttprsuzli.html

JS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtxrtgdbos.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtndlrbutb.html

Java: resp.statusCode()
来源：http://hz.gogol.net.cn/gthhvnildj.html

Go:   resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtusnelzft.html

Ruby: resp.code.to_i
来源：http://hz.tian-w.cn/gttjbfdhek.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtznbjmgjk.html

[L08] 并发请求多个地址
来源：http://hz.snrcjt.cn/gtfmhwyecu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtowxxkihl.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtdhmxbskg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtauwrqenh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtafwhmcpd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtwcelzfwg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenzaomai.com/gtwlzarrvq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gaohongyu789.top/gtdsjiemcr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gterzdwpfd.html

================================================================================
来源：http://hz.haohaochexian.top/gtmavwltfz.html

M. 命令行 / 进程 / 环境
来源：http://hz.sxryk.cn/gtzmelfhme.html

================================================================================
来源：http://hz.snrcjt.cn/gtxoynznka.html

[M01] 读取命令行参数
来源：http://hz.ybcxt.top/gtbljtishx.html

Py:   sys.argv[1:]
来源：http://hz.hysaishi.cn/gtbafuvzln.html

PHP:  $argv;  $argc;
来源：http://hz.andypj.xyz/gtbyertdjl.html

JS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtsxzvsprd.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtvfoxwbzk.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtcmudatxp.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gttuwactig.html

Ruby: ARGV
来源：http://hz.nanxinkj.top/gtjtudllxe.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtlssnlook.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtatlxrkyb.html

Py:   os.environ.get("HOME")
来源：http://hz.yj202588.top/gtwdqfxorm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.quarkkingdee.top/gtbvigftee.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gttxhrykmx.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gtosrolbww.html

Java: System.getenv("HOME")
来源：http://hz.nanxuanxn.top/gttpalqfrz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cheryme.top/gtxkanwyjl.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtukzvbpeb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtdzlnqhqk.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtctgmsjax.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtucbjxmpd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtdbkzdeqc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtusmesssv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtzqantoyo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.snrcjt.cn/gtywmfkofs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtlkxzhatl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtmwjssobf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.svipenyu.cn/gtbtfpkgjq.html

[M04] 获取当前工作目录
来源：http://hz.316326.xyz/gthaevkxaf.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtuvxogpyo.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gtpkwvgkyk.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtluvaemuk.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtucvcersk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yvedp.cn/gtjfkwhefi.html

Go:   os.Getwd()
来源：http://hz.chenzaomai.com/gtypnrdllu.html

Ruby: Dir.pwd
来源：http://hz.shuidangran.top/gtfvtcuvae.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigfzy.top/gtaxlrplsn.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtlgarzgju.html

Py:   sys.exit(1)
来源：http://hz.nanxinkj.top/gtbbttjqes.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtwevmtams.html

JS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gttdwoljpn.html

TS:   process.exit(1)
来源：http://hz.guowangkeji.top/gtdfnlmkdb.html

Java: System.exit(1)
来源：http://hz.cqqwz.cn/gtltldkezm.html

Go:   os.Exit(1)
来源：http://hz.kuanghao11.cn/gtjgctforo.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtskgqzkhq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigfzy.top/gtyknoqqrt.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gttdwthntm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtofgihxhk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinyuanbaomall.cn/gtfmbtaobg.html

JS:   console.error("err")
来源：http://hz.hfpthk.cn/gtpkkijxbs.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gtrjqsdzip.html

Java: System.err.println("err")
来源：http://hz.sweek.top/gtopsvrixi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtsajlwhxc.html

Ruby: warn "err"
来源：http://hz.yanxiufei.cn/gtmqgvdaiy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtbusrkuts.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gtszarhtuy.html

Py:   if __name__ == "__main__":
来源：http://hz.52xcode.cn/gtvsezffxt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.feifeiyinyue.top/gtougldvoq.html

JS:   require.main === module
来源：http://hz.ydjk.org.cn/gtekcgnxnf.html

TS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtzaoxcdaz.html

Java: public static void main(String[] args)
来源：http://hz.52xcode.cn/gteqvgglen.html

Go:   func main()
来源：http://hz.zycfv.cn/gtepzkbpnc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtakepzope.html

C#:   static void Main(string[] args)
来源：http://hz.yongpay.top/gtvpylcgyb.html

[M08] 获取系统与运行时信息
来源：http://hz.fzhhl.top/gtlkzjctmz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtkerqsjvj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gtvvmvxxxp.html

JS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtrnpcmxyy.html

TS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtadjbbtcr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangkeji.top/gtwrqwtcil.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangkeji.top/gtpzbsnsbm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtgmiyrvmt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jqgufenzy.top/gtjkdwiogw.html

================================================================================
来源：http://hz.cheryme.top/gtzdkbazbf.html

N. 数据结构与算法
来源：http://hz.yonumen.top/gtqubufndo.html

================================================================================
来源：http://hz.chenzaomai.com/gteohtuvsf.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgfzy.top/gthpetsian.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cdnleiting.top/gtvmlekwze.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuxming.cn/gthceqcysy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtwfvrplvj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtyrrgymdu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gtdsoszjhw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnxiangtu.top/gtkpdzexxc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtuoglqalc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtqwldbwst.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.316326.xyz/gtojucegzn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtktswatrk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yangfankeji.com/gteaooulls.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtxpwnspzz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtzclqtlpp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtjiyldiog.html

Go:   slices.Sort(arr)
来源：http://hz.tanke756.top/gtzqpgsavy.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtvodzraim.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jiagoushi.top/gtnrycyerx.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gtkodgnkst.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtuscbuxwn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenjidiqi.icu/gtyvobarsz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gtnoflagck.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtlupqkoqh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gtcozkwuud.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.andypj.xyz/gtzviimtmj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zycfv.cn/gtcxtmhiho.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtecrcluak.html

[N04] 斐波那契数列
来源：http://hz.aizwys.cn/gtozdvkbtz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtmcnvvojt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.havefunace.top/gtawbnntcm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtxegqwuap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtlfihwjwg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtndhpcsms.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtbjjwhihp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtkychwlfz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtobcxpasj.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gtzlrsuxam.html

Py:   math.gcd(a, b)
来源：http://hz.sysykeji.top/gtvdlfgkbh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gtoypzgeib.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtgolrmlch.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtxqlgbnbb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinghuilouyu.cn/gtrlhdydgc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sufxvd.cn/gtamqvszit.html

Ruby: a.gcd(b)
来源：http://hz.ivvv.top/gtnjpiuykd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtbdhpdukk.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtwdbrxupc.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtdnqadgwe.html

PHP:  $s === strrev($s);
来源：http://hz.ydzc1.top/gtyzsyldwo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtwxaykiph.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtwzalwbct.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhaomingkeji.xyz/gtkvjsrfcj.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtuezsgrhc.html

Ruby: s == s.reverse
来源：http://hz.pycfn.com/gtbykifxmk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtxbixvxph.html

[N07] 两数之和（返回下标）
来源：http://hz.xziqi.cn/gtmtkyvcdp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtmgjaqllk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gtqdqspfzm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydjk.org.cn/gtfvwduhne.html

TS:   // 手写 Map<string, number>
来源：http://hz.quarkkingdee.top/gtdlwmwxkw.html

Java: // 手写 HashMap
来源：http://hz.nanxuanxn.top/gtdjgkqjfb.html

Go:   // 手写 map[int]int
来源：http://hz.svipenyu.cn/gtatixzlgd.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtknvfhirz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hammf.cn/gtebhvanuf.html

[N08] 生成全排列
来源：http://hz.yj202588.top/gtholnpfur.html

Py:   itertools.permutations(arr)
来源：http://hz.aibaodan.cn/gtmfevepwz.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangtech.top/gtzuzzixga.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtdctzrvmv.html

TS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtedwndlcw.html

Java: // 手写回溯递归
来源：http://hz.aibaodan.cn/gtuffknyiy.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gthoqimckv.html

Ruby: arr.permutation.to_a
来源：http://hz.xuetiantiany.cn/gtaheijguc.html

C#:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtsmsyplrs.html

[N09] 栈与队列
来源：http://hz.hnxiangtu.top/gtgexcahlz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtjycizcpl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aibaodan.cn/gtwnednhdx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ehwqpu.com/gtrpqbixlw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtkrpwdmbd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gtsxlmcybg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ivvv.top/gtbrlythyu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258888.top/gtzrndazsb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hongshengwenyu.top/gtdfgzgcij.html

[N10] 链表节点定义
来源：http://hz.wangshuangyany.cn/gthswhvclk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hongshengwenyu.top/gtthieihuo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnxiangtu.top/gtkwhrncal.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangshuangyany.cn/gttncdembt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dashuyun.cn/gtitznhpft.html

Java: class Node { int v; Node next; }
来源：http://hz.chenlongwang.top/gtrzqarruz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtotajpccx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtemivodip.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydzc1.top/gtayjspwoa.html

[N11] 二叉树中序遍历
来源：http://hz.gzhubu.top/gtmolpohlv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtgfqituli.html

PHP:  // 手写递归函数
来源：http://hz.dashuyun.cn/gtjwebtuhg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gthcafswhs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtvszjguta.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtlivtubrg.html

Go:   // 手写递归
来源：http://hz.dashuyun.cn/gtagxnrlcj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pengpengdd.cyou/gtouyxzzsz.html

C#:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtyqiahiwn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtpuxhplrs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtaquhcdjr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangdashe.top/gtsfqdsmvg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtfempsdrf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gtmuikktat.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtxprrimad.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.svipenyu.cn/gtfhfxgzul.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shuidangran.top/gtlpmcaxdo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtyxwetzle.html

================================================================================
来源：http://hz.yangfankeji.com/gtruoyclbp.html

O. 并发与异步
来源：http://hz.sysykeji.top/gthzzxqrga.html

================================================================================
来源：http://hz.shzxlz.cn/gtniasmgdn.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtpbbgtayh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtkbuwovvv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhoulong.xyz/gtjqzidnct.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gtlnnrarns.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtmmnfehmm.html

Java: new Thread(() -> f()).start()
来源：http://hz.shangyingyoupin.top/gtsomrbmzp.html

Go:   go f()
来源：http://hz.cheryme.top/gtflpkxxbq.html

Ruby: Thread.new { f }
来源：http://hz.wangshuangyany.cn/gtfufwworc.html

C#:   Task.Run(() => F());
来源：http://hz.chenlongwang.top/gtaaykfdil.html

[O02] 使用线程池
来源：http://hz.jlsjyb.cn/gtetldnuno.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gttjcshjnk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gtaqeqyjxv.html

JS:   // worker_threads 线程池
来源：http://hz.gogol.net.cn/gtvbqsanes.html

TS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtzmolfbdx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtocypxboh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dashuyun.cn/gtvqauwyqi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhongyouzk.top/gtkstqyyzi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtotiksokx.html

[O03] 加锁保护共享数据
来源：http://hz.yangfankeji.com/gtgahzatvb.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtevhonxvd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhoulong.xyz/gtilqhiolp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhijiandao.cn/gtcljdvdbw.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtustkevwj.html

Java: synchronized (this) { shared++; }
来源：http://hz.gzhubu.top/gtoohkxszj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinyuanbaomall.cn/gtmeagskbg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.mhx1999.top/gthidxuejs.html

C#:   lock (gate) { shared++; }
来源：http://hz.jianghu66.top/gtlwlkdbnk.html

[O04] 定义异步函数并等待
来源：http://hz.sufxvd.cn/gteanwfcwg.html

Py:   async def f():⏎    await g()
来源：http://hz.svipenyu.cn/gtzmydwvxf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xinyue.icu/gtsukjenpy.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtvceaiipu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ehwqpu.com/gtqqxeejot.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.haohaochexian.top/gtnzqybrcp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenjidiqi.icu/gtsdonnofd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.316326.xyz/gtkfzgdapq.html

C#:   async Task F() { await G(); }
来源：http://hz.ybcxt.top/gtnlikshki.html

[O05] 并发执行并等待全部完成
来源：http://hz.svipenyu.cn/gtftokbpjc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sysykeji.top/gtedyylaxx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yanxiufei.cn/gtqjntzcil.html

JS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtxjqxuwbo.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangkeji.top/gtwafsuoes.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jiagoushi.top/gtfbxuskjs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cucudq.cn/gtlyabrdlh.html

Ruby: threads.map(&:join)
来源：http://hz.wangdashe.top/gtpikttxwi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gthzzfneud.html

[O06] 使用进程池
来源：http://hz.tanke756.top/gtbrjeouoo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtpkscnvvh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenzaomai.com/gthvopoxys.html

JS:   // child_process / cluster 模块
来源：http://hz.yj202588.top/gtuaeynsnl.html

TS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtmoioxdyg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ywan-chungtsiang.top/gtphdfcpqf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jianghu66.top/gtcizfgcam.html

Ruby: // fork 块
来源：http://hz.birdmap.top/gtbyygznrt.html

C#:   Parallel.For
来源：http://hz.hongshengwenyu.top/gtdkzzqdee.html

================================================================================
来源：http://hz.mhx1999.top/gtjgqyhwic.html

P. 常用工具函数
来源：http://hz.ywan-chungtsiang.top/gtxogsqyyd.html

================================================================================
来源：http://hz.hfpthk.cn/gtwejdylxb.html

[P01] 生成 UUID
来源：http://hz.zhoulong.xyz/gtqzumpyof.html

Py:   str(uuid.uuid4())
来源：http://hz.xuanzx.com/gtfesixbbm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yongpay.top/gtzwtdgepa.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtoqooyekf.html


<!-- 参考信息 -->