代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.zhaomingkeji.xyz/gtzgwbxukk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pycfn.com/gtwpzekejc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnxiangtu.top/gtedcrxsyw.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gtprolnqhx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hammf.cn/gthgsmwgon.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gthaazptrs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtmrqgqolx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtuaouhmmo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sweek.top/gtawhwfagg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtduinwskj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gtfvczcrmt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hammf.cn/gtyavmagtp.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangtech.top/gtvpskihzi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ivvv.top/gtfmfsuhyy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenlongwang.top/gttnkfduol.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtqlouxzqo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtxccbpqdb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtvbslolrc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtdgicszjd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnqzz.top/gtjomonzem.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtevhjfnsu.html

[L04] 设置超时
来源：http://hz.sufxvd.cn/gtcjzqjqsx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtczlrtoej.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cashguo.top/gtdwfnoizl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtxulxgbip.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtsopfldqb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhaomingkeji.xyz/gtpsupimmu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gthxwtuwdq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj202588.top/gttieiaqbl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenlongwang.top/gtezeoovqq.html

[L05] 上传文件（multipart）
来源：http://hz.sweek.top/gtpxurgcxv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tianlin.xyz/gtysemukky.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuanzx.com/gtklrnsczw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtjznzlntv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtbdunbuws.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tanke756.top/gtvcepmtwt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtjdzsyurd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yangfankeji.com/gtqtqrapks.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuxming.cn/gtvuabnlih.html

[L06] 解析响应为 JSON
来源：http://hz.ppjwa.cn/gtwkmrcdcb.html

Py:   resp.json()
来源：http://hz.hnxiangtu.top/gtnftmurmi.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gttcoxjxza.html

JS:   await resp.json()
来源：http://hz.tian-w.cn/gtyuaqtuyh.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtypjdnalv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangdashe.top/gtszkfbezc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtswskwebn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.smart0.xyz/gtjykioadw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtdhwmjvpv.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gttcyqqklo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtqnnicpcj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtxymlnnvd.html

JS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtnludvuqr.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtbjetdcme.html

Java: resp.statusCode()
来源：http://hz.zhijiandao.cn/gtthvrgwpw.html

Go:   resp.StatusCode
来源：http://hz.xuanzx.com/gtwizqhnxm.html

Ruby: resp.code.to_i
来源：http://hz.smart0.xyz/gtzahhvfho.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtdlitbklz.html

[L08] 并发请求多个地址
来源：http://hz.vqdsnc.cn/gtgrfrgyty.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hongshengwenyu.top/gtyavudlln.html

PHP:  curl_multi_init() 系列
来源：http://hz.sysykeji.top/gtdrffapqf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtlsszbvjs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtiuphsdtv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtkhyypjtz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtgrlffdxt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtnjmrhhrl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cqqwz.cn/gtdkaxjaig.html

================================================================================
来源：http://hz.dashuyun.cn/gtovupwxzn.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gttlwmyjcy.html

================================================================================
来源：http://hz.tian-w.cn/gtqapndehm.html

[M01] 读取命令行参数
来源：http://hz.iojbl.cn/gtpkmcxija.html

Py:   sys.argv[1:]
来源：http://hz.shuidangran.top/gtxlqmotbm.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtocuaivli.html

JS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gtujjrpavp.html

TS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtaxlopctw.html

Java: args 数组（main 方法参数）
来源：http://hz.jlsjyb.cn/gtfqtcmizz.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtfriujgjm.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtlctlkhjn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtvlyvhztp.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gtwtliwatn.html

Py:   os.environ.get("HOME")
来源：http://hz.jinyuanbaomall.cn/gtpvkdgxff.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tian-w.cn/gtknkkuudj.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gthkbvbxyl.html

TS:   process.env.HOME
来源：http://hz.guannengcc.top/gtepwsrtdu.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gttaagqwdw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.redwolf501.top/gtplthudwm.html

Ruby: ENV["HOME"]
来源：http://hz.aibaodan.cn/gtnmenoqgq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhoulong.xyz/gtbgnfjczt.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gthuxynkhg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtwkpzsjhk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.iojbl.cn/gtaljhecbt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtbwlrirnu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtweslhxho.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fengsongda.top/gtwhcdzxkn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.smart0.xyz/gtdfqfzlfn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgfzy.top/gtrccrtqvm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhoulong.xyz/gtoetlxswi.html

[M04] 获取当前工作目录
来源：http://hz.jlsjyb.cn/gtqjfuqdre.html

Py:   os.getcwd()
来源：http://hz.9152youxi.cn/gttobdqmjn.html

PHP:  getcwd();
来源：http://hz.ybcxt.top/gtldtpdfqs.html

JS:   process.cwd()
来源：http://hz.xylfe.cn/gtwdevydwb.html

TS:   process.cwd()
来源：http://hz.snrcjt.cn/gtvqlspqwi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgufenzy.top/gtzwlekwct.html

Go:   os.Getwd()
来源：http://hz.nwbrower.top/gtqyxnqulc.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gthlnzjwau.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.mhx1999.top/gtbiezobgm.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtvfiurhbl.html

Py:   sys.exit(1)
来源：http://hz.c1oappe.top/gtmlkqrqaj.html

PHP:  exit(1);
来源：http://hz.meibo888.top/gtkdqsfylj.html

JS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtbuiwcmel.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtunodjejd.html

Java: System.exit(1)
来源：http://hz.shzxlz.cn/gtditbpffc.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtzmezcnqg.html

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtclfiajth.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ybcxt.top/gtvoxatiod.html

[M06] 向标准错误输出
来源：http://hz.9152youxi.cn/gtgpepfdrk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtxxdgjlzs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtvdtgibrt.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtcmhcjgar.html

TS:   console.error("err")
来源：http://hz.fzhhl.top/gtgwtuexuc.html

Java: System.err.println("err")
来源：http://hz.yongpay.top/gtkuxomyrq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hywenlv.cn/gtdmxanqzx.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtcxjjzswl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yonumen.top/gtdrblloeu.html

[M07] 判断是否为主入口
来源：http://hz.ywan-chungtsiang.top/gtjocpxgkw.html

Py:   if __name__ == "__main__":
来源：http://hz.tianlin.xyz/gtmbawcykt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtizwmrgvi.html

JS:   require.main === module
来源：http://hz.zdqjudy.top/gtkoubokft.html

TS:   require.main === module
来源：http://hz.vqdsnc.cn/gtjhxgucmv.html

Java: public static void main(String[] args)
来源：http://hz.shuidangran.top/gtxauaadgh.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtotdpgvcj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nwbrower.top/gtnhwjrbgy.html

C#:   static void Main(string[] args)
来源：http://hz.jqgfzy.top/gtawumvyer.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gtwstlowjn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenlongwang.top/gtdqyfjigp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtzalzqpxn.html

JS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtrlcfslap.html

TS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtnkmnpusc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtatvbfywz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinyuanbaomall.cn/gtsntcbprf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtwijacnoh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guannengcc.top/gtucsoycvd.html

================================================================================
来源：http://hz.nanxinkj.top/gtbwvwehbu.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtajbeksfe.html

================================================================================
来源：http://hz.havefunace.top/gtpbecdyod.html

[N01] 二分查找（有序数组）
来源：http://hz.guowangkeji.top/gtutxrnbvy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgufenzy.top/gtfvrkpkrn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.smart0.xyz/gtqentfdon.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtvdqliokl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtqheytajg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258888.top/gtmpyxorca.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtwmmuwzxx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.9152youxi.cn/gtsadtkdmf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtmqtdiznt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gtewlgcgdf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtevygvwdb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydjk.org.cn/gtkqrxnflv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtguvdwwch.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtskyxvifg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtcwkadrsf.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtfieoqpnw.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtnqkctyov.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.smart0.xyz/gtzosyrvhw.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gtntrhqclm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guowangkeji.top/gtwgrrtipc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtkwikykgc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtatfgcqkd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtruygopss.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dashuyun.cn/gtsuvrnxms.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtcgqkjscc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.feifeiyinyue.top/gtpfiiadud.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.iojbl.cn/gtgadmqbnh.html

[N04] 斐波那契数列
来源：http://hz.dashuyun.cn/gtgkgnhkfe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtporesatd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtznsawvxe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtyoteofwu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtvgxdwory.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gotoacloud.top/gtfscgtlve.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtnpxabybt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtuqijhrvt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nwbrower.top/gtwgbzgfeh.html

[N05] 最大公约数
来源：http://hz.gzhubu.top/gtaoytpiff.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtduqrxxlu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtkwrjzqwp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtzswadkud.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtvnexyqfa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guowangkeji.top/gtejrcithr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hammf.cn/gtsgeznrsk.html

Ruby: a.gcd(b)
来源：http://hz.jqgufenzy.top/gtpfzuzgtx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gteawmwifz.html

[N06] 判断回文字符串
来源：http://hz.iojbl.cn/gtirpqmrma.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtxvnwhniu.html

PHP:  $s === strrev($s);
来源：http://hz.sxryk.cn/gtzhqaaikx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtzvwsuxpf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtxwmurkwm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtzbznvbum.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtymkxbfgk.html

Ruby: s == s.reverse
来源：http://hz.yuanzhike.top/gtssorakfc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtfrxquajb.html

[N07] 两数之和（返回下标）
来源：http://hz.zhaomingkeji.xyz/gtantjvwrg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhiwuduotai.top/gtbyuzzxho.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtpamgbysg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cqqwz.cn/gtbdwabudn.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtfvgbmhlm.html

Java: // 手写 HashMap
来源：http://hz.chenzaomai.com/gtpcnyzreq.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtxmbiqeal.html

Ruby: // 手写 Hash
来源：http://hz.cheryme.top/gtoafxwvrb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gtwuybfpan.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gtyjijiowr.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtgmizolxn.html

PHP:  // 手写递归交换
来源：http://hz.ywan-chungtsiang.top/gtiiwjgwnv.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtquzzjavf.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtwenlckza.html

Java: // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtvylapjwn.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtbfoswvwb.html

Ruby: arr.permutation.to_a
来源：http://hz.zycfv.cn/gthlupgvnf.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtylcsuudu.html

[N09] 栈与队列
来源：http://hz.tian-w.cn/gtworlyytj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tianlin.xyz/gtsovbnzyh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtgrulnslc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnxiangtu.top/gtfwdhqrtp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhiwuduotai.top/gtqdjajeva.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.smart0.xyz/gtdbiezcxj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.feifeiyinyue.top/gtppaqchxi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yongpay.top/gtkgemnjiu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yangfankeji.com/gtmulxsjsc.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtqzjfhplr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hammf.cn/gtvykeqeiu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtcmmbezyn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fengsongda.top/gtgxumfokm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.quarkkingdee.top/gttfmlsftb.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtendjthft.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cheryme.top/gtilhanfgp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guowangkeji.top/gtbrhipxac.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtsitdiotp.html

[N11] 二叉树中序遍历
来源：http://hz.9152youxi.cn/gticosdcsq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pycfn.com/gtihvygnjq.html

PHP:  // 手写递归函数
来源：http://hz.redwolf501.top/gtrxxpyjyp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtwdnndyxq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtzfhmjiat.html

Java: // 手写递归
来源：http://hz.yj20258.top/gtazwsxfsr.html

Go:   // 手写递归
来源：http://hz.redwolf501.top/gtkfjgfqma.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhiwuduotai.top/gttkltdtkz.html

C#:   // 手写递归
来源：http://hz.xylfe.cn/gtkdnzwceg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtitbeezoy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj202588.top/gtmebaebnq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gteivdzxyd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtiqoyfolk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtaccbygmy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtgrtcqilf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aizwys.cn/gtnuwtmesu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.meibo888.top/gtjwjikyob.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtieqqppqa.html

================================================================================
来源：http://hz.c1oappe.top/gtoqmfrnyf.html

O. 并发与异步
来源：http://hz.cheryme.top/gtekpzjtvy.html

================================================================================
来源：http://hz.daria6918.cn/gtnqxlynhj.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gtoqohmiur.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gaohongyu789.top/gtihmbpjdx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gtluvbxspt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jianghu66.top/gttdggzoyw.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtphzskgap.html

Java: new Thread(() -> f()).start()
来源：http://hz.xinyue.icu/gtiisoodmz.html

Go:   go f()
来源：http://hz.xuetiantiany.cn/gtnswasyap.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtiuxbqsgj.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtojudhmvx.html

[O02] 使用线程池
来源：http://hz.0kj1m.cn/gtqocppqbk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtfpcvackk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.0kj1m.cn/gtzoedzomt.html

JS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtdjumzjho.html

TS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtvtikqfto.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.iojbl.cn/gtawomxqft.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.havefunace.top/gtragtljqu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.316326.xyz/gtaowdtvsk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenjidiqi.icu/gtntscairg.html

[O03] 加锁保护共享数据
来源：http://hz.cashguo.top/gtckuoldxg.html

Py:   with lock: shared += 1
来源：http://hz.yongpay.top/gtsbcgwrsk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhoulong.xyz/gtnejxmxeg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yj20258888.top/gtwetkkgwx.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtnejfhjwx.html

Java: synchronized (this) { shared++; }
来源：http://hz.aibaodan.cn/gtjrmcdzah.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cdnleiting.top/gtqntsnfqw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.snrcjt.cn/gthgzaqkcf.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258.top/gtgpxvirzt.html

[O04] 定义异步函数并等待
来源：http://hz.zhixingplan.top/gtobkysvvk.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigfzy.top/gtexhelnnp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuetiantiany.cn/gtfexdtnbx.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtahdyrgph.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daxiang520.top/gtztobwghk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydjk.org.cn/gtrvqrzlpz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zycfv.cn/gtpzuyimaa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinqigufen.top/gtushayxvj.html

C#:   async Task F() { await G(); }
来源：http://hz.zhixingplan.top/gtlbclyqom.html

[O05] 并发执行并等待全部完成
来源：http://hz.tanke756.top/gtjkkzbepb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigufen.top/gtsiaoafqy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hammf.cn/gtfbjxpgrd.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtckmupecr.html

TS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtbltghvdd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gtrcmanxvp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cheryme.top/gthumkgilq.html

Ruby: threads.map(&:join)
来源：http://hz.bjfxy.top/gtuwpsfyyk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhijiandao.cn/gtemzmzbjr.html


<!-- 参考信息 -->