代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtfsimevjo.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtnmpphcpx.html

TS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtjtlacihd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fzhhl.top/gtnhdejdcy.html

Go:   resp, err := http.Get(url)
来源：http://hz.yanxiufei.cn/gtadlqxagq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yonumen.top/gtatgogvop.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgfzy.top/gtprkuuerv.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtiqkwsjqz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ivvv.top/gtptkezydv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtdpeqjzkb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtbofkmvcw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtapiwvijq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtknutplau.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinghuilouyu.cn/gtzkqevhrb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yueranfly.top/gtzclyvvou.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtqdfbksdl.html

[L03] 设置自定义请求头
来源：http://hz.xuetiantiany.cn/gtthnyowxp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pycfn.com/gtezsiflle.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhiwuduotai.top/gtjrzalmlc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gteahnwlja.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtiaijswye.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenzaomai.com/gtishlivpk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtndamtswb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jiagoushi.top/gtsjkgmnhb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtzcvriqrl.html

[L04] 设置超时
来源：http://hz.hfpthk.cn/gtlfebhonw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yanxiufei.cn/gthxzqrrfy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenlongwang.top/gttxswogck.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gthmkbfhtu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtzarkjciz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tianlin.xyz/gtrtciapfo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.feifeiyinyue.top/gtpcqhqufg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhixingplan.top/gtizyjisky.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gtkjxephhd.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtjyysyant.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jlsjyb.cn/gtlandqahk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.redwolf501.top/gtqodeyerq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gthhgowhjt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtdarhvxtf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aibaodan.cn/gtxtnxuvbw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ivvv.top/gtvsktjmxb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtshkxvicg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtrtiwsrcz.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtqjkopjql.html

Py:   resp.json()
来源：http://hz.chenzaomai.com/gtxyrbqqjo.html

PHP:  json_decode($body, true);
来源：http://hz.daxiang520.top/gtgbeinszm.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gtmmtyzkei.html

TS:   await resp.json()
来源：http://hz.gotoacloud.top/gtkbouzlwb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtxxpcxzkl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zdqjudy.top/gtnrqcocqo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ywan-chungtsiang.top/gtxjvvyxsk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shzxlz.cn/gtueruakcw.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtturnnnkd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtgubkklud.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gaohongyu789.top/gtutdgmhlv.html

JS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtcaiayrit.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtjbzzrnyk.html

Java: resp.statusCode()
来源：http://hz.jyoumei.cn/gtnydvmehl.html

Go:   resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtqfytyawt.html

Ruby: resp.code.to_i
来源：http://hz.cucudq.cn/gtajwnpboo.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtmgufefqn.html

[L08] 并发请求多个地址
来源：http://hz.hammf.cn/gthbgyyltn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtthpdgeeb.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtjbhblfjp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtmagdwvjc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtbrnzwwgf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxinkj.top/gtjexizfvc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtwjuvhufk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtsqihpuya.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtjvjhzitv.html

================================================================================
来源：http://hz.jqgfzy.top/gtcpkqiwyl.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtlttrjlcu.html

================================================================================
来源：http://hz.snrcjt.cn/gtonvruskj.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtktzahkwe.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtakgxbsao.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtyslzgpyf.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtfllfmtdj.html

TS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtjydnrnsi.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gtjhsokzzc.html

Go:   os.Args[1:]
来源：http://hz.birdmap.top/gtmernzlwb.html

Ruby: ARGV
来源：http://hz.xylfe.cn/gtkcivtohh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtwfhiykob.html

[M02] 读取环境变量
来源：http://hz.feifeiyinyue.top/gtipmrnmkq.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtjkygctcg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.haohaochexian.top/gthfzuywrj.html

JS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtsdzddsqs.html

TS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtacdivvoa.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gttfxlppnj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtgphnnswo.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtouhuvlzl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtynuzwcww.html

[M03] 执行外部命令
来源：http://hz.iojbl.cn/gtquthktfg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jiagoushi.top/gtvnnrqvpu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shangyingyoupin.top/gtmrhqaszo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtapptcbqs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtcywoiapt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ehwqpu.com/gtoifeedeg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtpwpeshur.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sxryk.cn/gthptmjiwn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gtzyqojrux.html

[M04] 获取当前工作目录
来源：http://hz.shangyingyoupin.top/gtzbtvgjrc.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtykmcypsp.html

PHP:  getcwd();
来源：http://hz.havefunace.top/gtmwfutzsl.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtqvhodtbz.html

TS:   process.cwd()
来源：http://hz.yj20258.top/gthkxhtrap.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtsdsqwnzh.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gtfixdqeal.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtgnfufymx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gtgoqkocyu.html

[M05] 设置退出码
来源：http://hz.ydjk.org.cn/gtmhswkhpf.html

Py:   sys.exit(1)
来源：http://hz.snrcjt.cn/gtjgywxqar.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gtzoilyxuf.html

JS:   process.exit(1)
来源：http://hz.zdqjudy.top/gttvnhchmv.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gtawzjrewu.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtegrwnoml.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtmizhnrcs.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gtdbevzyhx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.quarkkingdee.top/gtvpdszptc.html

[M06] 向标准错误输出
来源：http://hz.cashguo.top/gtunbjmrax.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangshuangyany.cn/gtxeitpsbt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hongshengwenyu.top/gtibginkgm.html

JS:   console.error("err")
来源：http://hz.ehwqpu.com/gtkpjabvof.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gthwnfdcis.html

Java: System.err.println("err")
来源：http://hz.tanke756.top/gtgmzeloxp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.daxiang520.top/gtmipppole.html

Ruby: warn "err"
来源：http://hz.yj202588.top/gttuhrsbbt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhengqikj.top/gtdbzyiuof.html

[M07] 判断是否为主入口
来源：http://hz.52xcode.cn/gttodwjkck.html

Py:   if __name__ == "__main__":
来源：http://hz.yuxming.cn/gtuiglsnmv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtghdikxpj.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gtthfblsmr.html

TS:   require.main === module
来源：http://hz.redwolf501.top/gtuzshmiev.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtoswgknuk.html

Go:   func main()
来源：http://hz.aibaodan.cn/gtkbqzekmr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtgskwyrkc.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtksnbjdnv.html

[M08] 获取系统与运行时信息
来源：http://hz.ppjwa.cn/gthnsriymr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtthwluazv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hongshengwenyu.top/gtugrtclny.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtdypdqelv.html

TS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtnkzgyfdl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aibaodan.cn/gtnabjvvbt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gturzncuyl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gttbsgfnpd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shuidangran.top/gtmtugrpmr.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfchxpxoe.html

N. 数据结构与算法
来源：http://hz.pengpengdd.cyou/gtmdejrclp.html

================================================================================
来源：http://hz.sweek.top/gtrchibgxz.html

[N01] 二分查找（有序数组）
来源：http://hz.iojbl.cn/gtulvfqxst.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtrkgbufew.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ivvv.top/gtgkjbihpu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtddbnlssv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtmrnqxlvn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtcrbtqbij.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenjidiqi.icu/gtgefdmlfi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.bjfxy.top/gtvipgicgj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtjdhuzzkc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtkezgemkm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtepyddjyg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cdnleiting.top/gtkwnsfrov.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtxdwsyrct.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtrosanjka.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ppjwa.cn/gtenzipwrb.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtwkwcdjrt.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtkmtlphxy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gtfnozhfjy.html

[N03] 快速排序（分治示例）
来源：http://hz.haohaochexian.top/gtwpksjqlw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yuanzhike.top/gtwkzdweiy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pengpengdd.cyou/gtjzubasou.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtqyyruxin.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtawtqcjno.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtymwdanei.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtbkaovvnl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shangyingyoupin.top/gtjdaoplnm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gtgxkxdpyf.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gtqwzfugag.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtnfcyayaj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gzhubu.top/gtpptqzghk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtreiaizlw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtipmozoks.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhiwuduotai.top/gtgtseauxy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgufenzy.top/gttwlnsfsx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gtdcmrovqz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gotoacloud.top/gtyqxjkzte.html

[N05] 最大公约数
来源：http://hz.ppjwa.cn/gtsciuknmv.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gtdzpujski.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ywan-chungtsiang.top/gtmzjfrcwj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtgaxwhfyg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtnezwqyqa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtbuffqblt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xziqi.cn/gtpfdqqnfo.html

Ruby: a.gcd(b)
来源：http://hz.jqgufenzy.top/gttuynhipw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtrdolgxsp.html

[N06] 判断回文字符串
来源：http://hz.zhiwuduotai.top/gtgifwigso.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtemhdotev.html

PHP:  $s === strrev($s);
来源：http://hz.kuanghao11.cn/gtftzypzrk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtbkyijyga.html

TS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtfbjfgouw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.c1oappe.top/gtvyekfhrg.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtvgkrmbvz.html

Ruby: s == s.reverse
来源：http://hz.yuxming.cn/gtywmdrltr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtfiiqdfel.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtdqrdcjcn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ywan-chungtsiang.top/gtnzdgegyn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuanzhike.top/gtgkhcxxwr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.quarkkingdee.top/gtufzgrzpm.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gtspswnhch.html

Java: // 手写 HashMap
来源：http://hz.havefunace.top/gtzdkmcncf.html

Go:   // 手写 map[int]int
来源：http://hz.yuxming.cn/gtemhfwvyc.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gtxoprfixv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.vqdsnc.cn/gthuzwnoed.html

[N08] 生成全排列
来源：http://hz.fzhhl.top/gthvlowcre.html

Py:   itertools.permutations(arr)
来源：http://hz.gzhubu.top/gtywpjdspv.html

PHP:  // 手写递归交换
来源：http://hz.xuetiantiany.cn/gtsmfhkcap.html

JS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtoralfdwk.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtvpugzclt.html

Java: // 手写回溯递归
来源：http://hz.dianchejie.cn/gtbqkhvkrd.html

Go:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtjjyfdfaj.html

Ruby: arr.permutation.to_a
来源：http://hz.yueranfly.top/gtpiloozdz.html

C#:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtvrkyoziw.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gtucdhkano.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtuqlsviyx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhoulong.xyz/gtgozdkpkn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtpldtnwvu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sysykeji.top/gtxfcjvfqy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gtkdqcppge.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cdnleiting.top/gtougvtjfp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.svipenyu.cn/gtbqtiahzt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtpzkoljvb.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gtovycphfm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenjidiqi.icu/gtediyunwi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.9152youxi.cn/gtijzavfcl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.52xcode.cn/gtlkrppkwm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.0kj1m.cn/gtobcyopew.html

Java: class Node { int v; Node next; }
来源：http://hz.sysykeji.top/gtiawhzahq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jyoumei.cn/gtdgehtdri.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtwusgenqr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gzhubu.top/gtnxreewih.html

[N11] 二叉树中序遍历
来源：http://hz.xylfe.cn/gtfguvvtrl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tianlin.xyz/gtxcpmsupq.html

PHP:  // 手写递归函数
来源：http://hz.tian-w.cn/gtesedrnwn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinyuanbaomall.cn/gthzjhiutt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtzermoruw.html

Java: // 手写递归
来源：http://hz.ivvv.top/gtxoruvdsz.html

Go:   // 手写递归
来源：http://hz.smart0.xyz/gtktofsvlx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tanke756.top/gtvokggefx.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gtmjuuxohh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.vqdsnc.cn/gtwglioqjm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtjmhmnpid.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.svipenyu.cn/gtpudbejao.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtaczvhbtd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtafutbljj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtqqbrzrzd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtzjiihmca.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.316326.xyz/gtpdjvwlhj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtqazlfnrq.html

================================================================================
来源：http://hz.wangdashe.top/gtetaqmrke.html

O. 并发与异步
来源：http://hz.pengpengdd.cyou/gtvkcacorr.html

================================================================================
来源：http://hz.sysykeji.top/gtejjrjjmm.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gtjdguowyw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gtddfobend.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnqzz.top/gtiypwizas.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xinyue.icu/gtxvvqlxbl.html

TS:   // 同 JS
来源：http://hz.aizwys.cn/gthuhteuzw.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhaomingkeji.xyz/gtxqgymczy.html

Go:   go f()
来源：http://hz.guowangkeji.top/gtcbgayspk.html

Ruby: Thread.new { f }
来源：http://hz.aizwys.cn/gtyfkmzazv.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtkpatktqx.html

[O02] 使用线程池
来源：http://hz.yj20258888.top/gtghhaerpz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtdxxffbsu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtnqjpijmx.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtzmbjxnhl.html

TS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtfzupxkwv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jqgfzy.top/gtditujthm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tian-w.cn/gtvtgdubkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hfpthk.cn/gtobapgvun.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xylfe.cn/gtpboqfsvl.html

[O03] 加锁保护共享数据
来源：http://hz.ivvv.top/gtqdvqkoxw.html

Py:   with lock: shared += 1
来源：http://hz.ydjk.org.cn/gtlovfgvko.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtrydyhicj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gaohongyu789.top/gtjxhxponu.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtlfdxbyjc.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtvrwmnxxg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.andypj.xyz/gtatirynja.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhiwuduotai.top/gtpljhyblp.html

C#:   lock (gate) { shared++; }
来源：http://hz.quarkkingdee.top/gtndfdqdzo.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gtrblpksri.html

Py:   async def f():⏎    await g()
来源：http://hz.gogol.net.cn/gtitixigut.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydzc1.top/gtyqalcgmi.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gtcfceoywx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gthvonrfcg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gttkhscsss.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gthfpcbrtn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenlongwang.top/gtdxayygwg.html

C#:   async Task F() { await G(); }
来源：http://hz.yongpay.top/gtpfdogqan.html

[O05] 并发执行并等待全部完成
来源：http://hz.gzhubu.top/gtismyvktd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhixingplan.top/gtiomjllvj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnqzz.top/gtinrpuwls.html

JS:   await Promise.all(tasks)
来源：http://hz.hnxiangtu.top/gtcjcuickx.html

TS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtatiapqed.html


<!-- 参考信息 -->