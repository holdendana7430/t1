代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ppjwa.cn/gtwxoxqafc.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtkbntnyqq.html

TS:   await fetch(url)
来源：http://hz.nwbrower.top/gtbepdjxve.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydjk.org.cn/gtxqnfjvhj.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gtwhsiktkv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtzuvcirkr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtphfndefj.html

[L02] 发送 POST JSON
来源：http://hz.yueranfly.top/gtxzreqlqu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gtdnikyxhq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cheryme.top/gtbnnfxvap.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtskpewgna.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtaqtrqvob.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtigaetwft.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jlsjyb.cn/gtijxipuil.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtudtgfhxo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuxming.cn/gtbdbrsgyh.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gtzpimsikc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tian-w.cn/gtcgazuysh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhengqikj.top/gtsjucevrh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtzbaufpge.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtivebgoia.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fengsongda.top/gtlnbxuddd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtohiefobj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gteoaedrqi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtngrrulxb.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtppczthyd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yanxiufei.cn/gtqakfcxzd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtivnbqavs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtlxywitnd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtviubonff.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.svipenyu.cn/gtxkegvcuu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtngkahydt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xylfe.cn/gtoqhbbkor.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgufenzy.top/gtllzipate.html

[L05] 上传文件（multipart）
来源：http://hz.chenzaomai.com/gtuvsiscxc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yongpay.top/gtotuewsbe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.snrcjt.cn/gtfpdzpjtw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtzvdqcwdp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtnunwwgnw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgufenzy.top/gtsmheyxuk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aibaodan.cn/gtlfmbljdg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtiezeirsu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtupymqfin.html

[L06] 解析响应为 JSON
来源：http://hz.zhixingplan.top/gtgyngblce.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtktpkfkxo.html

PHP:  json_decode($body, true);
来源：http://hz.hysaishi.cn/gtwdrummlg.html

JS:   await resp.json()
来源：http://hz.wangdashe.top/gtaivjhqxp.html

TS:   await resp.json()
来源：http://hz.havefunace.top/gtzjhkpion.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtqqmegzfj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgfzy.top/gtgnluxzci.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guowangkeji.top/gtwnvljbjp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.mhx1999.top/gtpnnexkwx.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gteopkytoo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ppjwa.cn/gtjgmhutoq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtubwsgyjg.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtgmmqazoz.html

TS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtmwaezgdg.html

Java: resp.statusCode()
来源：http://hz.nwbrower.top/gtrhwopjxp.html

Go:   resp.StatusCode
来源：http://hz.zhijiandao.cn/gtirsmdjaa.html

Ruby: resp.code.to_i
来源：http://hz.ywan-chungtsiang.top/gtglsrizys.html

C#:   (int)resp.StatusCode
来源：http://hz.wangdashe.top/gtylvcigwv.html

[L08] 并发请求多个地址
来源：http://hz.nanxinkj.top/gtkrnvjryi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cheryme.top/gtrocmvixp.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangshuangyany.cn/gtdpgcnfsw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtvorskyqe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtpttdzics.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aibaodan.cn/gtllwyyglu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cqqwz.cn/gtiwfohikt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtgygojhmv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gotoacloud.top/gtgubapcyv.html

================================================================================
来源：http://hz.dashuyun.cn/gtrqhjnubn.html

M. 命令行 / 进程 / 环境
来源：http://hz.cashguo.top/gtzpftgxfo.html

================================================================================
来源：http://hz.jinqigufen.top/gtaoznksod.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gteuexkxje.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtxzobiynk.html

PHP:  $argv;  $argc;
来源：http://hz.c1oappe.top/gtmqjoujbp.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtkbkxectw.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtewhuiwjy.html

Java: args 数组（main 方法参数）
来源：http://hz.gaohongyu789.top/gtnqylrymt.html

Go:   os.Args[1:]
来源：http://hz.yueranfly.top/gtuldlcxzx.html

Ruby: ARGV
来源：http://hz.wangshuangyany.cn/gtbefdcpam.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtzdqtolme.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gtjuzwvcwa.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgfzy.top/gtfdolxvzr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pycfn.com/gthhmovxok.html

JS:   process.env.HOME
来源：http://hz.yvedp.cn/gtibzplgyv.html

TS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gttnfkcvgs.html

Java: System.getenv("HOME")
来源：http://hz.ydjk.org.cn/gtdhgkxbfe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtuyrlbmjv.html

Ruby: ENV["HOME"]
来源：http://hz.haohaochexian.top/gtiazaiejo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhijiandao.cn/gtxojyauea.html

[M03] 执行外部命令
来源：http://hz.guannengcc.top/gtxyokcrzi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yanxiufei.cn/gtrczdjcjr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtnsjafndu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtqwhhnixs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtkdwykkxd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtmgbvtazn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tanke756.top/gtcxxpsdgo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuanzhike.top/gtxkmrwiyi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.wangshuangyany.cn/gtrveptpem.html

[M04] 获取当前工作目录
来源：http://hz.svipenyu.cn/gtacshvzgw.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtwboxkjuy.html

PHP:  getcwd();
来源：http://hz.jinqigfzy.top/gtyvnqkxkj.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtqkqbrwuh.html

TS:   process.cwd()
来源：http://hz.daria6918.cn/gtbmsgkqbp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ybcxt.top/gtyczknxed.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtvzfnpznz.html

Ruby: Dir.pwd
来源：http://hz.hnqzz.top/gtocfijbrq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuanzx.com/gtuklkqlvr.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtwfwfiqwa.html

Py:   sys.exit(1)
来源：http://hz.chenjidiqi.icu/gtxawxnpdp.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gtiylrvnek.html

JS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtqnycbezc.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtafsaeksc.html

Java: System.exit(1)
来源：http://hz.yuanzhike.top/gtgdjbvcja.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtvzbgwsou.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtlxlcqlvh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yangfankeji.com/gtmisihbpt.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gttmzuebwt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.0kj1m.cn/gtikowqzuk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shzxlz.cn/gtyedxszqk.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtmehjlaql.html

TS:   console.error("err")
来源：http://hz.haohaochexian.top/gtbatkfhcx.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtlxwpojic.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtfvpzkutv.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtvyqweygr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gttjmhclyg.html

[M07] 判断是否为主入口
来源：http://hz.ybcxt.top/gtmkgppwiw.html

Py:   if __name__ == "__main__":
来源：http://hz.iojbl.cn/gtcjcrfdrn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinghuilouyu.cn/gthkbxalkw.html

JS:   require.main === module
来源：http://hz.yongpay.top/gtcjkyucru.html

TS:   require.main === module
来源：http://hz.hammf.cn/gtskenmxpm.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtycclfgsu.html

Go:   func main()
来源：http://hz.c1oappe.top/gthluepkuu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xingfuxueyuan.xyz/gteapvohcc.html

C#:   static void Main(string[] args)
来源：http://hz.ivvv.top/gtxmsrzarj.html

[M08] 获取系统与运行时信息
来源：http://hz.andypj.xyz/gtepvqoumc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtdkefynlc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xingfuxueyuan.xyz/gtrjbvgawj.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtzotkudat.html

TS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtydcuhsrk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtglmaydrr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtclfnakmp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuanzx.com/gtrcezzygm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pycfn.com/gticvafooj.html

================================================================================
来源：http://hz.jianghu66.top/gtddumxtju.html

N. 数据结构与算法
来源：http://hz.meibo888.top/gtwnqyoasa.html

================================================================================
来源：http://hz.snrcjt.cn/gtgoksjnal.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtrzkcsqrl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gttdqhpzvm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gtuzukmukl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtttpimmjt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gthsjsplxr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtotxzgjuw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxuanxn.top/gtuwovgnld.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.haohaochexian.top/gtibdwxzdg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtezegyalg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtgehlynym.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtizrzfntq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.iojbl.cn/gttanrakkg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtrucoyewk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jianghu66.top/gtcwzpwdgw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yanxiufei.cn/gtvthjrfui.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gthatnkagn.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtepbaszoa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yanxiufei.cn/gtswemzmal.html

[N03] 快速排序（分治示例）
来源：http://hz.jiagoushi.top/gtmzpadoaq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gaohongyu789.top/gtxbtadxqv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuetiantiany.cn/gteprvakhf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gthufeihnf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtuhycxafa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pengpengdd.cyou/gtjcufevvy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtqmlbsolx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtsyzctvrn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gaohongyu789.top/gtnfydcebw.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtfyruyqpf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtaqvdcjkj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gtpckddrie.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtcqysaptd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtyetlzpct.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuetiantiany.cn/gtvayklqqt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtcahoolxe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtezarplpj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtttzeoigu.html

[N05] 最大公约数
来源：http://hz.ivvv.top/gtzvdwbkjg.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtnadvvllp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gtjvqbimlq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtfovvngtz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtptddqlnr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gtolffsznr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yangfankeji.com/gtknftrvxy.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtaziepqxj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guannengcc.top/gtxkycfyzm.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtitgulyue.html

Py:   s == s[::-1]
来源：http://hz.cheryme.top/gtrwvaawke.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtlqgymvcb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtepksvdwd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtprypbvmr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhiwuduotai.top/gttinsixha.html

Go:   // 双指针从两端比较
来源：http://hz.ybcxt.top/gtvvjdppgh.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gttdlyvwdh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtqzugxhyf.html

[N07] 两数之和（返回下标）
来源：http://hz.shzxlz.cn/gthcdvgcrl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jyoumei.cn/gtwdoqdcsz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhiwuduotai.top/gtyutlwzcw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgufenzy.top/gttvfjrrxk.html

TS:   // 手写 Map<string, number>
来源：http://hz.meibo888.top/gtjbojkyeb.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtbbeqylgo.html

Go:   // 手写 map[int]int
来源：http://hz.shzxlz.cn/gtechibupa.html

Ruby: // 手写 Hash
来源：http://hz.bjfxy.top/gttjpnytae.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gtmoxpiccs.html

[N08] 生成全排列
来源：http://hz.aizwys.cn/gtpwveqdit.html

Py:   itertools.permutations(arr)
来源：http://hz.zhaomingkeji.xyz/gtdawwkywx.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gtfsmozffi.html

JS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtxghmjenf.html

TS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtzlbusikz.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gthlfhklgb.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtrvhzbksi.html

Ruby: arr.permutation.to_a
来源：http://hz.xziqi.cn/gthovxxgtk.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtgtrexgso.html

[N09] 栈与队列
来源：http://hz.yonumen.top/gtcvbnnpwe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xinyue.icu/gtjgvnhcuq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhixingplan.top/gtqttnjkzf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tianlin.xyz/gtzzkfdycx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fzhhl.top/gtyjraxcfx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtmvtrcppd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aibaodan.cn/gtahjnbyyp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tian-w.cn/gtnqgcijbl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxuanxn.top/gtxfyyyllv.html

[N10] 链表节点定义
来源：http://hz.cucudq.cn/gthdhamywk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gtxhycdwoi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shangyingyoupin.top/gtjebciudr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sufxvd.cn/gttcdfdrmm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtlwkvhlay.html

Java: class Node { int v; Node next; }
来源：http://hz.iojbl.cn/gtrxfceoue.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangdashe.top/gtzdvgkwsr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gtcdxldpxp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinyuanbaomall.cn/gtiwkfknhl.html

[N11] 二叉树中序遍历
来源：http://hz.sufxvd.cn/gtbakkiofh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ehwqpu.com/gtsgvlbclb.html

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gtrggmrcrm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtiuxernsj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gticlqnuop.html

Java: // 手写递归
来源：http://hz.dianchejie.cn/gtiryyioet.html

Go:   // 手写递归
来源：http://hz.quarkkingdee.top/gtgpnlaqkf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dashuyun.cn/gtxrhiwmae.html

C#:   // 手写递归
来源：http://hz.bjfxy.top/gttyszqrwo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gzhubu.top/gtrmlbchiv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gogol.net.cn/gtjoexhvno.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtdluhhbui.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtwqkdzzwk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtojmbqkex.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gttgdcggcb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yanxiufei.cn/gtmxxxxfig.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgufenzy.top/gtqyeuwbtt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtbtdpmeyp.html

================================================================================
来源：http://hz.yj202588.top/gtvtqlfjjs.html

O. 并发与异步
来源：http://hz.nanxinkj.top/gtxuktgqwb.html

================================================================================
来源：http://hz.fengsongda.top/gtztvaklgn.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtcinjhqcx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jiagoushi.top/gtzmzygukf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtdbdkpqpk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtjtighnjw.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtmleavbfg.html

Java: new Thread(() -> f()).start()
来源：http://hz.daria6918.cn/gtrunwzrbh.html

Go:   go f()
来源：http://hz.zhiwuduotai.top/gttqaqwvgj.html

Ruby: Thread.new { f }
来源：http://hz.jqgufenzy.top/gtjfvsmqdx.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258888.top/gtfakvjdyh.html

[O02] 使用线程池
来源：http://hz.guowangkeji.top/gttjzhzboc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.aibaodan.cn/gtekcdhqpk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.andypj.xyz/gtyjkkfeby.html

JS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtqhnpryic.html

TS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtxtwhdzvi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtzwemrgtz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hongshengwenyu.top/gtwbazcaws.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ehwqpu.com/gtcawdpkkt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.9152youxi.cn/gtvyybalpo.html

[O03] 加锁保护共享数据
来源：http://hz.hnxiangtu.top/gtaxpmqmwt.html

Py:   with lock: shared += 1
来源：http://hz.cdnleiting.top/gtnhkouror.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhongyouzk.top/gtatzyerhf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cashguo.top/gtljumawvu.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtkyjywoje.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gtintaumum.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgfzy.top/gtabsganii.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenzaomai.com/gtbupqmaip.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtbkyguhup.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtjkaauhgt.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gtwqcvplxn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtzgayqcix.html

JS:   async function f() { await g(); }
来源：http://hz.ybcxt.top/gtxbhpptqo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangkeji.top/gtmbhhhbux.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuanzhike.top/gtkdqvdmpd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.redwolf501.top/gtptjdltqb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtaasfxfvb.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gtcxtgbysf.html

[O05] 并发执行并等待全部完成
来源：http://hz.tianlin.xyz/gthahdhixp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuetiantiany.cn/gtskhyotul.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guowangkeji.top/gtlesvmggy.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtolkovkdh.html

TS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtxcoofvre.html


<!-- 参考信息 -->