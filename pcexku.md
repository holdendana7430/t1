代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtljzduukq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtbmeisook.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daria6918.cn/gtffrnbsbz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtctuvyygy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtirlvktpg.html

[L04] 设置超时
来源：http://hz.guannengcc.top/gtienvlbhu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtqqkxkxmq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gtixfzizct.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtcvuxmzse.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gttkbctgpm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinyuanbaomall.cn/gtflowammc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gtbfthlhsg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnxiangtu.top/gtpqvvdlmu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gotoacloud.top/gtnbwwvxzp.html

[L05] 上传文件（multipart）
来源：http://hz.zhoulong.xyz/gtcflglkah.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hysaishi.cn/gtsiahifxo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cqqwz.cn/gtidjwlsai.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtzwtucwdc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtozscdafm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.andypj.xyz/gtmqhiuhnc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sweek.top/gtovwfkhcf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtwbjhwvgc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.vqdsnc.cn/gtlnayrozn.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtzmluuhst.html

Py:   resp.json()
来源：http://hz.daria6918.cn/gtjqifbbdf.html

PHP:  json_decode($body, true);
来源：http://hz.cashguo.top/gtcrluxqek.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtrzzmhgdp.html

TS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtmzpyqlyk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gthrucfyfu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtkmghdjax.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinyuanbaomall.cn/gtqsdikwmm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.0kj1m.cn/gteqbzlccz.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtbfyorjul.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuetiantiany.cn/gtunfzmcmx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pengpengdd.cyou/gtetvpycvs.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtqskzojbo.html

TS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtjpanvphd.html

Java: resp.statusCode()
来源：http://hz.cucudq.cn/gtbsbqutlj.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gtafhitdhk.html

Ruby: resp.code.to_i
来源：http://hz.cucudq.cn/gtcivwavav.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtldvsualz.html

[L08] 并发请求多个地址
来源：http://hz.cashguo.top/gtftnbionh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gttgknhmbn.html

PHP:  curl_multi_init() 系列
来源：http://hz.sxryk.cn/gtexljeyry.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtdmmusbpl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtteccpzze.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxinkj.top/gtdnklwajg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.9152youxi.cn/gtclennpdw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.andypj.xyz/gtsyzgejov.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtikethlri.html

================================================================================
来源：http://hz.jianghu66.top/gtjlrxliie.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtycddofkf.html

================================================================================
来源：http://hz.gzhubu.top/gtqjbppfxc.html

[M01] 读取命令行参数
来源：http://hz.wangshuangyany.cn/gtijthnurt.html

Py:   sys.argv[1:]
来源：http://hz.nwbrower.top/gtpyqacwqa.html

PHP:  $argv;  $argc;
来源：http://hz.haohaochexian.top/gtellgglaf.html

JS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gteispsqtt.html

TS:   process.argv.slice(2)
来源：http://hz.cdnleiting.top/gtkpsmidgw.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtjoysjqqs.html

Go:   os.Args[1:]
来源：http://hz.zhiwuduotai.top/gtyozrkvga.html

Ruby: ARGV
来源：http://hz.ehwqpu.com/gtkjgbdyyg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sysykeji.top/gtndewviod.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtfbakyvmf.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gtrojpttii.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.bjfxy.top/gtndtgoqlu.html

JS:   process.env.HOME
来源：http://hz.shuidangran.top/gtamzifczu.html

TS:   process.env.HOME
来源：http://hz.52xcode.cn/gtdhqsmuyu.html

Java: System.getenv("HOME")
来源：http://hz.jinghuilouyu.cn/gtmzcjueup.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.52xcode.cn/gtbvllzxmg.html

Ruby: ENV["HOME"]
来源：http://hz.guowangkeji.top/gttwvkkwwq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yueranfly.top/gtatckvacy.html

[M03] 执行外部命令
来源：http://hz.svipenyu.cn/gttrhckzpg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtqlpgkfis.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtmihutqdi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtripnsmdg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtxhdccqwh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtjxupkxac.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtuazukjym.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yanxiufei.cn/gtqjoqdeyw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtstpzwlli.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gttbplpovd.html

Py:   os.getcwd()
来源：http://hz.haohaochexian.top/gtlqchyhjo.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtjjfojmtf.html

JS:   process.cwd()
来源：http://hz.ppjwa.cn/gtcaddhkod.html

TS:   process.cwd()
来源：http://hz.guowangkeji.top/gtgbjyfjco.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtqcdfwltq.html

Go:   os.Getwd()
来源：http://hz.ydzc1.top/gtytrgmyil.html

Ruby: Dir.pwd
来源：http://hz.haohaochexian.top/gtjrwlzqff.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sysykeji.top/gtjiksypiw.html

[M05] 设置退出码
来源：http://hz.ybcxt.top/gtwdvsoqgv.html

Py:   sys.exit(1)
来源：http://hz.yangfankeji.com/gtexuxjpat.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gtjsscwyrf.html

JS:   process.exit(1)
来源：http://hz.dianchejie.cn/gtpdvmmwqx.html

TS:   process.exit(1)
来源：http://hz.iojbl.cn/gttfrcbzom.html

Java: System.exit(1)
来源：http://hz.hywenlv.cn/gtzpadekgc.html

Go:   os.Exit(1)
来源：http://hz.ydzc1.top/gtjlxezpvd.html

Ruby: exit 1
来源：http://hz.feifeiyinyue.top/gtnlicunuj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.bjfxy.top/gtmdydwzsd.html

[M06] 向标准错误输出
来源：http://hz.mhx1999.top/gtfvwecxqf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.havefunace.top/gtwpqoszci.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinyuanbaomall.cn/gtqohxzmdv.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtmbisdrql.html

TS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtoacyfsnc.html

Java: System.err.println("err")
来源：http://hz.316326.xyz/gtpndarutb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtrfimirkz.html

Ruby: warn "err"
来源：http://hz.tanke756.top/gtcmkoswpk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daria6918.cn/gtzmgfekpo.html

[M07] 判断是否为主入口
来源：http://hz.cheryme.top/gtfhviuahu.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtfysjtqfv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.mhx1999.top/gtyuohsdmu.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtqsvxukdd.html

TS:   require.main === module
来源：http://hz.zhengqikj.top/gtzgmrtpeb.html

Java: public static void main(String[] args)
来源：http://hz.birdmap.top/gtudsflqdi.html

Go:   func main()
来源：http://hz.yongpay.top/gtkrzrzvro.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenlongwang.top/gtjrrqpnex.html

C#:   static void Main(string[] args)
来源：http://hz.wangshuangyany.cn/gtjyyfycev.html

[M08] 获取系统与运行时信息
来源：http://hz.chenlongwang.top/gtmskovoni.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yangfankeji.com/gtljetvcrp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtozhgmjvu.html

JS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtgptamzgv.html

TS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtuosilqtq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtrrwnmmjo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guannengcc.top/gtnzdqwyqn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yueranfly.top/gtffkdcfqm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydzc1.top/gtftwnchzd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzbycwkbo.html

N. 数据结构与算法
来源：http://hz.dashuyun.cn/gtjddadzwr.html

================================================================================
来源：http://hz.sysykeji.top/gtgnqhvxke.html

[N01] 二分查找（有序数组）
来源：http://hz.sysykeji.top/gtszxlcwdr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtrcpkmryy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gtfnrdbcsx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtiefiybyx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtoogovpoc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.52xcode.cn/gtmxstdhft.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangshuangyany.cn/gtbjahjhtc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gtncdusmyd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtzhtwbket.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtwskmcpob.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtwltyovmy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guannengcc.top/gtbkevbyug.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gttsmwrhae.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtfyfqazsj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.haohaochexian.top/gtfeetqgts.html

Go:   slices.Sort(arr)
来源：http://hz.sxryk.cn/gtqthjqgth.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtuhyhshth.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jyoumei.cn/gtlkgewefz.html

[N03] 快速排序（分治示例）
来源：http://hz.jyoumei.cn/gtmlzscrua.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shzxlz.cn/gtvgmdmvqr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gtzvlcxzvu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.quarkkingdee.top/gtvssbmadw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtuqqgbnfi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxinkj.top/gtxvwzovzj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtzsdkogdg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtcqnzelug.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gaohongyu789.top/gturteqgfn.html

[N04] 斐波那契数列
来源：http://hz.yonumen.top/gtwwbqvhxl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtuunkkkgp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gaohongyu789.top/gtagdeqine.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtexxizbjw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yongpay.top/gtadxpspzu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangshuangyany.cn/gtouuqewcz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtfjhlilin.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtyybrnhew.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gttguuwwjo.html

[N05] 最大公约数
来源：http://hz.52xcode.cn/gtxgvuqskq.html

Py:   math.gcd(a, b)
来源：http://hz.ydjk.org.cn/gtinozcowf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ehwqpu.com/gtopqwyjjh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gaohongyu789.top/gtkebopfyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtzotblggq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtjkfukcky.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtymcjmomd.html

Ruby: a.gcd(b)
来源：http://hz.cheryme.top/gthitiojax.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtlsfamhzd.html

[N06] 判断回文字符串
来源：http://hz.daria6918.cn/gtbdudpwov.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtiedwwjka.html

PHP:  $s === strrev($s);
来源：http://hz.haohaochexian.top/gtpscfjnph.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtecidrxtc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtivczwyim.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dashuyun.cn/gtgwvrpifm.html

Go:   // 双指针从两端比较
来源：http://hz.hysaishi.cn/gtvmubpwwd.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gttyynxykj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtxbauqcjz.html

[N07] 两数之和（返回下标）
来源：http://hz.zhongyouzk.top/gtymhjtlip.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtfjtpnmya.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuetiantiany.cn/gtojnpfxnw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuanzhike.top/gtkqdxemgp.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnqzz.top/gthfipdnwy.html

Java: // 手写 HashMap
来源：http://hz.fengsongda.top/gtfcvdxzdg.html

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtweedtrgx.html

Ruby: // 手写 Hash
来源：http://hz.yonumen.top/gtmucmsdda.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.52xcode.cn/gtugyjazgt.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gtogpebdoz.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtcaiutagb.html

PHP:  // 手写递归交换
来源：http://hz.hammf.cn/gtkzyxcaij.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtzeeaofsy.html

TS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtcqyskcol.html

Java: // 手写回溯递归
来源：http://hz.sweek.top/gtozesovbl.html

Go:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtahhjjejo.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gttntjrqix.html

C#:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtuunknmhb.html

[N09] 栈与队列
来源：http://hz.zycfv.cn/gtrjiqglgc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgufenzy.top/gtiarmenwg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gtppanftvy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.c1oappe.top/gtogpreaah.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhiwuduotai.top/gtaeuklfyq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tanke756.top/gtdroawnyt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtreixryer.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtspgqwjox.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gtvgmceesu.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gtwhikkaik.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hongshengwenyu.top/gtohruqnuh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhoulong.xyz/gtrersaqil.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtnnnyatpm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenlongwang.top/gtwsegwzan.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gtgvjjhqsa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guowangkeji.top/gtulemcpai.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dianchejie.cn/gthfcbqyss.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.redwolf501.top/gtzxaojgug.html

[N11] 二叉树中序遍历
来源：http://hz.havefunace.top/gtgopiomcs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenlongwang.top/gtdxzyysyg.html

PHP:  // 手写递归函数
来源：http://hz.ivvv.top/gtaewrirjl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtsbjymhud.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtmhdordac.html

Java: // 手写递归
来源：http://hz.chenzaomai.com/gtdfgiaiqa.html

Go:   // 手写递归
来源：http://hz.9152youxi.cn/gtlbdxovgx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aizwys.cn/gtudzndwdv.html

C#:   // 手写递归
来源：http://hz.daria6918.cn/gtaxqvgroe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daria6918.cn/gtzoxuepyj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtdjkxfcyd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuanzhike.top/gtitnqnrvn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtunsuifur.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guowangkeji.top/gttudkmubc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtlxpkyqbb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.fzhhl.top/gthywfcdgl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gtnhkrhkaf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtyinmyagq.html

================================================================================
来源：http://hz.dashuyun.cn/gtgjsjoatc.html

O. 并发与异步
来源：http://hz.cdnleiting.top/gtkeetsccs.html

================================================================================
来源：http://hz.haohaochexian.top/gtiubcqofj.html

[O01] 启动一个线程
来源：http://hz.0kj1m.cn/gtwjrasgkl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.redwolf501.top/gtsqxitfba.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.smart0.xyz/gtzzzcxehn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yanxiufei.cn/gttbecsjjx.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gteotpebpn.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhoulong.xyz/gtycncfjng.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtysndoezv.html

Ruby: Thread.new { f }
来源：http://hz.aizwys.cn/gtagkoceuc.html

C#:   Task.Run(() => F());
来源：http://hz.gaohongyu789.top/gtgjdyczav.html

[O02] 使用线程池
来源：http://hz.xziqi.cn/gtufulaekv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sysykeji.top/gtewgewpzv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtbwurjflf.html

JS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtqwqakwhc.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtervupqlx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ybcxt.top/gttrpglgzz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.quarkkingdee.top/gtwxfgnimh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hongshengwenyu.top/gtyaevcxob.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.andypj.xyz/gtmickxmsu.html

[O03] 加锁保护共享数据
来源：http://hz.zycfv.cn/gtfzverdmm.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtgwlqknzy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yonumen.top/gtebbqwgam.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuanzhike.top/gtmkvsvpbc.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtgsdbvntc.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxuanxn.top/gtxhqvrqua.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shuidangran.top/gtbpcyzmwq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zdqjudy.top/gtpxlqflkz.html

C#:   lock (gate) { shared++; }
来源：http://hz.sxryk.cn/gtwooscjfx.html

[O04] 定义异步函数并等待
来源：http://hz.ywan-chungtsiang.top/gtezauufau.html

Py:   async def f():⏎    await g()
来源：http://hz.dashuyun.cn/gtmxmzxffq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daxiang520.top/gtepwxxarf.html

JS:   async function f() { await g(); }
来源：http://hz.hnxiangtu.top/gtlfxococi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.haohaochexian.top/gtzrgbhvuy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxuanxn.top/gtrhmdddmt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gtdsbivbnu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shzxlz.cn/gtvhloktep.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangkeji.top/gtkswhygvu.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhoulong.xyz/gtwztrrwnx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtmvykzxma.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gthwefyigw.html

JS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtkrsxjpte.html

TS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtzoiosjhy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.quarkkingdee.top/gtcravgsww.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtdsijtsvd.html

Ruby: threads.map(&:join)
来源：http://hz.ybcxt.top/gtusbehqwa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhaomingkeji.xyz/gtfavmfczh.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtsqturctr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sweek.top/gtpfotgwox.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinyuanbaomall.cn/gtebeyxrob.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtrczbpubh.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtyesqdtek.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gtzoxnatrs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtcdsdbwbl.html

Ruby: // fork 块
来源：http://hz.guannengcc.top/gtnpmlvlsi.html

C#:   Parallel.For
来源：http://hz.zycfv.cn/gttjpkosyb.html

================================================================================
来源：http://hz.hysaishi.cn/gtvgcslzph.html

P. 常用工具函数
来源：http://hz.hywenlv.cn/gtbcvuulod.html

================================================================================
来源：http://hz.dashuyun.cn/gtwvypipjt.html

[P01] 生成 UUID
来源：http://hz.jinqigfzy.top/gtlbcuhntw.html

Py:   str(uuid.uuid4())
来源：http://hz.dashuyun.cn/gtfpafasca.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.smart0.xyz/gtmszlaajy.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtqppcpsxc.html


<!-- 参考信息 -->