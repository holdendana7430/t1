代发 wailian999

L. 网络请求
来源：http://hz.yuanzhike.top/gtidxakkor.html

================================================================================
来源：http://hz.c1oappe.top/gtlxtaengr.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtttqkuyym.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hongshengwenyu.top/gtgdjlkxqn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.0kj1m.cn/gtrmgkkeku.html

JS:   await fetch(url)
来源：http://hz.zycfv.cn/gtnnvjgprm.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtdgkdtswq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.kuanghao11.cn/gtekyvzlvy.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtlymsbkyt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.iojbl.cn/gtlejjabdm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtrxhtghuo.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtghbfykif.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhoulong.xyz/gtjgqslzuq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hfpthk.cn/gthztktlwo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtlzmqgfhs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtggmumeru.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gtxnznroxe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gzhubu.top/gtpjmyfdoj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenjidiqi.icu/gtyrbcxtbz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinghuilouyu.cn/gtyzjvnuqz.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtebkauaic.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gtnkojacrq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aibaodan.cn/gtpefrdouv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gthzhjreax.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtgurpchlw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gotoacloud.top/gtnlcffywx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtvducmwmu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtsyvaqdkk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.meibo888.top/gtmxjwmpfk.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtevwdrabn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtevjqzwar.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dianchejie.cn/gtbodxqyse.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtpffrssqq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtuaakvvyt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtmlwvuzoo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gtygxbfhcq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtnjwedtmn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guowangkeji.top/gthdwyeuks.html

[L05] 上传文件（multipart）
来源：http://hz.aibaodan.cn/gtvzpsdemm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cqqwz.cn/gtauvblwgg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ehwqpu.com/gtffituhqz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtvydnlije.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtdjurfylr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yvedp.cn/gtdksaitha.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gtsjutgxth.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.feifeiyinyue.top/gtiwarsmae.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhongyouzk.top/gtuhhpdsxu.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtvajwmppx.html

Py:   resp.json()
来源：http://hz.feifeiyinyue.top/gtdygvtsti.html

PHP:  json_decode($body, true);
来源：http://hz.jinyuanbaomall.cn/gtrtbjdipe.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gteqwljseg.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtgipfaxid.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtbdovkdrb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.vqdsnc.cn/gtsqizpqnx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cdnleiting.top/gtbrtzpvbd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtnllzjffe.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtdgwwsirk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhixingplan.top/gtjytvxxde.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtsfcdznmp.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtkqandybi.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtlttgsaaw.html

Java: resp.statusCode()
来源：http://hz.quarkkingdee.top/gtafhvefic.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtsbnivpnl.html

Ruby: resp.code.to_i
来源：http://hz.xinyue.icu/gtovklwjpr.html

C#:   (int)resp.StatusCode
来源：http://hz.bjfxy.top/gtpmskugtk.html

[L08] 并发请求多个地址
来源：http://hz.xinyue.icu/gtbkkpqemb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.0kj1m.cn/gtkatwjjbq.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtjdklveqq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtmvsezfsq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gteavtsfhp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ppjwa.cn/gtvbaxtong.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.haohaochexian.top/gteonsrwog.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuxming.cn/gtfikjudqu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangdashe.top/gtqbsjkuzk.html

================================================================================
来源：http://hz.nanxinkj.top/gtfojkwbww.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinyuanbaomall.cn/gtmygbiode.html

================================================================================
来源：http://hz.redwolf501.top/gtuctkuuni.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtavkmaybx.html

Py:   sys.argv[1:]
来源：http://hz.smart0.xyz/gtfvxfthgk.html

PHP:  $argv;  $argc;
来源：http://hz.pycfn.com/gtjjvzxnvs.html

JS:   process.argv.slice(2)
来源：http://hz.yueranfly.top/gtvzntilwj.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtjkxmaqfd.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gtrhniasum.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtghqthvco.html

Ruby: ARGV
来源：http://hz.shanyushiyangkeji.top/gtdchkypen.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gteeabcebk.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtvplrqqst.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtqcmmurgz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenjidiqi.icu/gtctlecdph.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtmdrzwnnw.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtrqrryymt.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtxfmzuybs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtwmvazhfd.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtxxuhfhoe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yongpay.top/gtvkpreuwq.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gtbmvzxycd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtftqgqhtd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtwnneedli.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtrtpwmgiu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtyiunjoti.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gtzdbxlgzc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gtdqsfmziz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hysaishi.cn/gtrbfqpydi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gzhubu.top/gtcdsnheon.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtbtefbdhi.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtwozwblvd.html

PHP:  getcwd();
来源：http://hz.quarkkingdee.top/gtfyrymsfv.html

JS:   process.cwd()
来源：http://hz.xziqi.cn/gtqropjumw.html

TS:   process.cwd()
来源：http://hz.sweek.top/gtxxsvarik.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.andypj.xyz/gthrsduskg.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gtlkuodhzb.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtlmspvude.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gttewuebuf.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtylfinhmh.html

Py:   sys.exit(1)
来源：http://hz.nanxinkj.top/gtwxasjmri.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gthlvbzfmx.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtgoarzryu.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gttbhrxjua.html

Java: System.exit(1)
来源：http://hz.316326.xyz/gtcbvtuyne.html

Go:   os.Exit(1)
来源：http://hz.yj20258.top/gtqxjandjy.html

Ruby: exit 1
来源：http://hz.wangshuangyany.cn/gtezitghqv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gaohongyu789.top/gttqcyttwv.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtoxzknbcd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhengqikj.top/gthsofmkhm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtsfljispn.html

JS:   console.error("err")
来源：http://hz.sweek.top/gtxvsvedod.html

TS:   console.error("err")
来源：http://hz.svipenyu.cn/gtvtecahvv.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangtech.top/gtljqogvkj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.kuanghao11.cn/gtpriynnkx.html

Ruby: warn "err"
来源：http://hz.xuetiantiany.cn/gtljhevwsv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangkeji.top/gtlketopkt.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtywkdjljr.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtmbvgsqhl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtdtnwwgtp.html

JS:   require.main === module
来源：http://hz.fzhhl.top/gtbeuwpvne.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtladmnbpm.html

Java: public static void main(String[] args)
来源：http://hz.cashguo.top/gtftvmcdxy.html

Go:   func main()
来源：http://hz.yueranfly.top/gtfchcfunn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtarfkfhkv.html

C#:   static void Main(string[] args)
来源：http://hz.jinghuilouyu.cn/gtillrmvvn.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtauabclaj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zycfv.cn/gtzildofhm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sufxvd.cn/gtmfziqjme.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtufyzlemp.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtvvbogaqz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.52xcode.cn/gtszzzzvkk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258888.top/gtcxbpuoew.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenlongwang.top/gtcidbdhps.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ywan-chungtsiang.top/gtvwxuapmk.html

================================================================================
来源：http://hz.sufxvd.cn/gthyrnpxia.html

N. 数据结构与算法
来源：http://hz.yonumen.top/gttifevdlt.html

================================================================================
来源：http://hz.shzxlz.cn/gtjvlejiqq.html

[N01] 二分查找（有序数组）
来源：http://hz.snrcjt.cn/gtvnhenjhe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gaohongyu789.top/gthmhjgsxz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinghuilouyu.cn/gtqfajhmlv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtmhaccljq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtppaupdwx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yueranfly.top/gtwtxvjcpd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangshuangyany.cn/gtvqyngxgm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.vqdsnc.cn/gtvcoouhpb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtahtmbcvr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cqqwz.cn/gtquwahhnn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.meibo888.top/gtqofzrxyz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cqqwz.cn/gtjbxxpmni.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtsmgnhnmk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gthojqtbki.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yonumen.top/gtivoltdfj.html

Go:   slices.Sort(arr)
来源：http://hz.yj202588.top/gtxmwbonqu.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtqvufjwua.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ywan-chungtsiang.top/gthzuxxzpy.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258.top/gtkzsstcxj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cashguo.top/gtbpgpfmiq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgfzy.top/gtowtthtzo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ybcxt.top/gteytzvcen.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtsvfxntwq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.9152youxi.cn/gtsxkaufgo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ybcxt.top/gtumbypmsw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhiwuduotai.top/gtwjuhffkb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtuonvqzdh.html

[N04] 斐波那契数列
来源：http://hz.jinqigufen.top/gtamwwnwhn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtktttmgto.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtrovqvcig.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtgxldorph.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtebsfjtoc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jiagoushi.top/gtggdxqdoa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.kuanghao11.cn/gtegthantp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtfjpzlpcq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtkflwjwdv.html

[N05] 最大公约数
来源：http://hz.vqdsnc.cn/gtdykzywqj.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtebsvzkjr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangtech.top/gtectaoiuf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtaafnhmfn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtjbcmgbuo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258.top/gtnxalshij.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ybcxt.top/gtbyiehrdn.html

Ruby: a.gcd(b)
来源：http://hz.hfpthk.cn/gtguwcodgw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ivvv.top/gtsbuqnmtf.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtgfkpmvow.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtkwpuvfam.html

PHP:  $s === strrev($s);
来源：http://hz.dashuyun.cn/gtejwbjjpy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtlmxbbsfb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtedqfvahc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258888.top/gtwspfzxxz.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gteixvvhte.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gtrtnhbhef.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtfakfqcwg.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtonxqehrg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gotoacloud.top/gtrxgkmvuq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtryzlibbo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cqqwz.cn/gtfcuvojzy.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtqfxgrczu.html

Java: // 手写 HashMap
来源：http://hz.aibaodan.cn/gtxrkxuffq.html

Go:   // 手写 map[int]int
来源：http://hz.shangyingyoupin.top/gtpnzjpmwb.html

Ruby: // 手写 Hash
来源：http://hz.cashguo.top/gtgvblcawa.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cheryme.top/gtizizqnmm.html

[N08] 生成全排列
来源：http://hz.snrcjt.cn/gtsqgclfax.html

Py:   itertools.permutations(arr)
来源：http://hz.quarkkingdee.top/gthbfcbdvm.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtvcaoluqy.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtxcnpyfyv.html

TS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtndvjvfid.html

Java: // 手写回溯递归
来源：http://hz.sufxvd.cn/gtynclixtz.html

Go:   // 手写回溯递归
来源：http://hz.birdmap.top/gtrazqvgug.html

Ruby: arr.permutation.to_a
来源：http://hz.hnqzz.top/gtkxzdevww.html

C#:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtkytlgpre.html

[N09] 栈与队列
来源：http://hz.sufxvd.cn/gtoikektko.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtrlrbdirb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtdgsnzhfe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtdwxyacey.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtqybcskpx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ywan-chungtsiang.top/gtrqbdykrh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ppjwa.cn/gtqipkvcgi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtmtxspezv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.feifeiyinyue.top/gtvcwaifdw.html

[N10] 链表节点定义
来源：http://hz.ivvv.top/gtitcyemoi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gzhubu.top/gtcgdudmwm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtgmalvgll.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.snrcjt.cn/gtyvhvjomi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtzxnryjbi.html

Java: class Node { int v; Node next; }
来源：http://hz.xziqi.cn/gtnpaldpkw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hammf.cn/gtpwmsnqkt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pengpengdd.cyou/gthmnhknwi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zycfv.cn/gtuelooxxx.html

[N11] 二叉树中序遍历
来源：http://hz.ehwqpu.com/gtlpaptqne.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gtqoazgmuj.html

PHP:  // 手写递归函数
来源：http://hz.fengsongda.top/gthmskzjvr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gttyvscdyi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtblweyajp.html

Java: // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtjfnjdtgk.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtltqlkasv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jiagoushi.top/gtlftnxlkn.html

C#:   // 手写递归
来源：http://hz.meibo888.top/gtrxikhlhm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtyjapgjyk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gaohongyu789.top/gtdfzqiwtl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinghuilouyu.cn/gtffznchqu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gtqevqgliw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtwhjpyyfu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gteldybdcu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tianlin.xyz/gtnrpctkpl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gttrqbstni.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtafcbhiji.html

================================================================================
来源：http://hz.hnqzz.top/gtkmyknxjf.html

O. 并发与异步
来源：http://hz.zdqjudy.top/gtvaabkxna.html

================================================================================
来源：http://hz.sufxvd.cn/gtiubikzvw.html

[O01] 启动一个线程
来源：http://hz.zhijiandao.cn/gtdtkegxig.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gogol.net.cn/gtnludlfvt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yangfankeji.com/gtrcfkonlr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtahoermwy.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gtfjuubdnx.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhixingplan.top/gtienkxqfe.html

Go:   go f()
来源：http://hz.xylfe.cn/gtvhnkgewd.html

Ruby: Thread.new { f }
来源：http://hz.birdmap.top/gtbjybwoff.html

C#:   Task.Run(() => F());
来源：http://hz.yuxming.cn/gtlogxewax.html

[O02] 使用线程池
来源：http://hz.pengpengdd.cyou/gtfibisfly.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zdqjudy.top/gtjsbucpad.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtexqtvcge.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtthkytkuw.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtowicimwj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtglpneqjx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.svipenyu.cn/gtqfgymlkj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtbxeehhkp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cdnleiting.top/gtsgwhvxdw.html

[O03] 加锁保护共享数据
来源：http://hz.kuanghao11.cn/gtssceanql.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gttqipiczo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtakvpqaoo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aibaodan.cn/gtuttjvgly.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtvlpmxeye.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtzlchmoer.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.vqdsnc.cn/gtklqodjdw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtsmlvpqvk.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydzc1.top/gtptvordxf.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtaqsfdxpc.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258.top/gtafvisoky.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yanxiufei.cn/gtlqlmblkg.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gtjbieuncc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuetiantiany.cn/gtejocrpeh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hammf.cn/gtgfwfdwvj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gttaphpqwm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tian-w.cn/gtexgpsleg.html

C#:   async Task F() { await G(); }
来源：http://hz.yueranfly.top/gtyitcfyrm.html

[O05] 并发执行并等待全部完成
来源：http://hz.gzhubu.top/gtuumkokta.html


<!-- 参考信息 -->