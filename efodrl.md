代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.yuanzhike.top/gtkkhhathi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigufen.top/gtcgfufhkk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gttmucqswa.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gteqjnjien.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daxiang520.top/gtocrvupvi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtqxzjspyg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtzhrioykd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtbldnghuf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hywenlv.cn/gtjurfyfhj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuetiantiany.cn/gtcskabcsa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhoulong.xyz/gteefwkavz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gtwkghbang.html

[L03] 设置自定义请求头
来源：http://hz.yuanzhike.top/gtbcbvwkpf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.mhx1999.top/gtrvwdiljr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shzxlz.cn/gtgkddwzfd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtftdrokle.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtgfkvlggw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guannengcc.top/gtjljllkfw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtcueynipb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zycfv.cn/gtnxjdseyf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.52xcode.cn/gtjaflulob.html

[L04] 设置超时
来源：http://hz.xylfe.cn/gtubdqrtdj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sufxvd.cn/gtfsbyyztl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhongyouzk.top/gtndplnxzi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtvawumvjw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gttbspwzao.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yueranfly.top/gtmhlyepub.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtokkzatej.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daxiang520.top/gtbkkxommt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.haohaochexian.top/gtegzvezij.html

[L05] 上传文件（multipart）
来源：http://hz.hongshengwenyu.top/gtznqttjko.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jyoumei.cn/gtnituyzuj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtvekmwxrn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtmcasdghq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtefsfwdua.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gttujyumkp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cdnleiting.top/gteorqdguj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.birdmap.top/gtkldcuybr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtxcyekqwm.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtrlnvedku.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtsusanjju.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigufen.top/gtydtxosgl.html

JS:   await resp.json()
来源：http://hz.fengsongda.top/gtzuezesjv.html

TS:   await resp.json()
来源：http://hz.guowangkeji.top/gtegnnqdbn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fengsongda.top/gtwwcegksd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinghuilouyu.cn/gtiseerpld.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtdpyrosav.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtxozhfphw.html

[L07] 处理 HTTP 状态码
来源：http://hz.haohaochexian.top/gtjfnlztno.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pycfn.com/gtrzzehtcl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sweek.top/gtgoyrwtdn.html

JS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtbuyoqhiq.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtjisownuj.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtpwvqalks.html

Go:   resp.StatusCode
来源：http://hz.gzhubu.top/gtmytsmynq.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtcpgfdlnf.html

C#:   (int)resp.StatusCode
来源：http://hz.sysykeji.top/gtgqmgqiue.html

[L08] 并发请求多个地址
来源：http://hz.hammf.cn/gtzgmoucfr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cdnleiting.top/gtnesdqykm.html

PHP:  curl_multi_init() 系列
来源：http://hz.hywenlv.cn/gtyfvwwcml.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtvfwekfjm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtklkvujyd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jiagoushi.top/gtbhjanebz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fzhhl.top/gtmhghmzcb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cheryme.top/gtutokjvya.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sweek.top/gtdhsoamny.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtfsbzlmlx.html

M. 命令行 / 进程 / 环境
来源：http://hz.cashguo.top/gtyyzrjdrq.html

================================================================================
来源：http://hz.dashuyun.cn/gtatzqqmjs.html

[M01] 读取命令行参数
来源：http://hz.yueranfly.top/gtzkrebcqj.html

Py:   sys.argv[1:]
来源：http://hz.snrcjt.cn/gtqayediem.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtjbojpcqk.html

JS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtqmdgygct.html

TS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gtuclvnbrb.html

Java: args 数组（main 方法参数）
来源：http://hz.gzhubu.top/gtsmafghtm.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtubrlhkan.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtlcznsotu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hfpthk.cn/gtcaidthwl.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtqxmkkrgt.html

Py:   os.environ.get("HOME")
来源：http://hz.yuxming.cn/gtxlbkjbwp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhoulong.xyz/gtrydmsgps.html

JS:   process.env.HOME
来源：http://hz.c1oappe.top/gtkkieosrw.html

TS:   process.env.HOME
来源：http://hz.sxryk.cn/gtlbnrztfw.html

Java: System.getenv("HOME")
来源：http://hz.svipenyu.cn/gtlixrmzac.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtleuaysof.html

Ruby: ENV["HOME"]
来源：http://hz.yonumen.top/gtnmhsnpvq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hongshengwenyu.top/gtdlruvpkk.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gtybvqbdka.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zycfv.cn/gtdekljoty.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shuidangran.top/gtgddbyrha.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtgaoaitwy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtveafepgl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xinyue.icu/gtfkhvcmkr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yangfankeji.com/gtsxzarifq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yonumen.top/gtqemkdfix.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jlsjyb.cn/gtkcokwotf.html

[M04] 获取当前工作目录
来源：http://hz.cucudq.cn/gtgkwpxhqa.html

Py:   os.getcwd()
来源：http://hz.daxiang520.top/gturbipbyx.html

PHP:  getcwd();
来源：http://hz.vqdsnc.cn/gtdaefnggt.html

JS:   process.cwd()
来源：http://hz.tian-w.cn/gtamzzzjlv.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtoisckhdr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sysykeji.top/gtnnuocpro.html

Go:   os.Getwd()
来源：http://hz.jyoumei.cn/gtgqsdhqvm.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtldbgmgoh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigfzy.top/gtbbbujxdk.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtyxaizkqd.html

Py:   sys.exit(1)
来源：http://hz.shangyingyoupin.top/gtfccqfyrc.html

PHP:  exit(1);
来源：http://hz.gaohongyu789.top/gtozdjsvru.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtswgnnxdd.html

TS:   process.exit(1)
来源：http://hz.ivvv.top/gtnsjlmvfz.html

Java: System.exit(1)
来源：http://hz.yj20258.top/gtnrrvivns.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtjetmwljg.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtfinyiuho.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.316326.xyz/gtwhjonchc.html

[M06] 向标准错误输出
来源：http://hz.tian-w.cn/gtpaphqbuu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtehnlwvzb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tanke756.top/gtvncvhgxq.html

JS:   console.error("err")
来源：http://hz.yvedp.cn/gtoywxhinf.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtymmutxys.html

Java: System.err.println("err")
来源：http://hz.wangdashe.top/gtyhtjjgzx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.quarkkingdee.top/gtlkzrwpzy.html

Ruby: warn "err"
来源：http://hz.sxryk.cn/gtcnpgmhwt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daxiang520.top/gtepsjjxef.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtfmwbmmah.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxinkj.top/gtmcltxeno.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtgzhfnjbu.html

JS:   require.main === module
来源：http://hz.gotoacloud.top/gtggjscglw.html

TS:   require.main === module
来源：http://hz.dianchejie.cn/gtufcquxfx.html

Java: public static void main(String[] args)
来源：http://hz.hfpthk.cn/gtsabhplwq.html

Go:   func main()
来源：http://hz.dashuyun.cn/gtgskeqotg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.9152youxi.cn/gtficnjxzz.html

C#:   static void Main(string[] args)
来源：http://hz.0kj1m.cn/gtlzvbgtph.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtgopxktea.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gtxrwwjrty.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sysykeji.top/gtlvaflhbo.html

JS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtfszxvmvk.html

TS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtdxxbqhbp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxuanxn.top/gtdbkgdcik.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtyhhllmzv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtnazeecpv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guannengcc.top/gtqadxvxer.html

================================================================================
来源：http://hz.yonumen.top/gtoyiwfkln.html

N. 数据结构与算法
来源：http://hz.hysaishi.cn/gtgrgbreth.html

================================================================================
来源：http://hz.yueranfly.top/gtglrflzcd.html

[N01] 二分查找（有序数组）
来源：http://hz.zhoulong.xyz/gtaopuptou.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.vqdsnc.cn/gtrprjkpmw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtrczrgvgs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gtflntzjeo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtrawtroxy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tanke756.top/gtjzphowxb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtsrhmypzu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gtmtaxlgbc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtkssqpdgv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xingfuxueyuan.xyz/gtiyimeirv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.52xcode.cn/gtudoulcfd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jiagoushi.top/gtotelhzfx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtsrsxahhd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtdpypdqrb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gttasixsyq.html

Go:   slices.Sort(arr)
来源：http://hz.yuanzhike.top/gttwlasqsz.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtnemrhxeg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtehyacnlf.html

[N03] 快速排序（分治示例）
来源：http://hz.tianlin.xyz/gtjtungekv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtucccciip.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ywan-chungtsiang.top/gtwhwuenbq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtecrcmqab.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtcjpujclq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.smart0.xyz/gtrhrgedwe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yanxiufei.cn/gtqweeppgp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gtbptdgfyy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hammf.cn/gtpsejnygc.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtxrczqbqe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtgjafmlhl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtzwrayncx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtjxxrcgrl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtrdbrupfx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhijiandao.cn/gtqaadaqzq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gtmvqabwkx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtnczsaxqw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtihmnavey.html

[N05] 最大公约数
来源：http://hz.haohaochexian.top/gtzeujlpks.html

Py:   math.gcd(a, b)
来源：http://hz.guannengcc.top/gtaqgeneht.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aizwys.cn/gtabfziwub.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtzduuupkk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtvzbyskih.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangtech.top/gtaxbatezx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtogivncra.html

Ruby: a.gcd(b)
来源：http://hz.feifeiyinyue.top/gtkwypyxwi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.bjfxy.top/gtnklbydsb.html

[N06] 判断回文字符串
来源：http://hz.yongpay.top/gtyanqlubd.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtmryaevva.html

PHP:  $s === strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gteomowhur.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtcdnahsuh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtcayqdwgp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jianghu66.top/gtyjeparvq.html

Go:   // 双指针从两端比较
来源：http://hz.gzhubu.top/gtrxmjcglw.html

Ruby: s == s.reverse
来源：http://hz.tianlin.xyz/gtfklnovko.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtcygmwvec.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gtmqwdvdjq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pengpengdd.cyou/gtewsdufjb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.52xcode.cn/gtawfblrbm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxuanxn.top/gtceowxyyn.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangkeji.top/gtvgnevxco.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtjeypdded.html

Go:   // 手写 map[int]int
来源：http://hz.zhaomingkeji.xyz/gtezomiiym.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtvgcmpamo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jianghu66.top/gtrgucrifc.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gtbqnwahwx.html

Py:   itertools.permutations(arr)
来源：http://hz.c1oappe.top/gtzhtnraua.html

PHP:  // 手写递归交换
来源：http://hz.sweek.top/gtjsejkwtx.html

JS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtzznfhprl.html

TS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtjtjrrfkk.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtpvngpiar.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtdfowasag.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtyhjxhapb.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtdcodhrcr.html

[N09] 栈与队列
来源：http://hz.ybcxt.top/gtxuyzczor.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ybcxt.top/gtdamhqtdh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgufenzy.top/gtwncyfsep.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtjpmoqaia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.meibo888.top/gtgjhnzzww.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ivvv.top/gteytttmlr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258888.top/gtqstdapvk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cheryme.top/gtetcfnzgm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.9152youxi.cn/gtpsbdxhcx.html

[N10] 链表节点定义
来源：http://hz.wangshuangyany.cn/gtliwkzpwj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gtloosiqla.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gotoacloud.top/gtmlsfzlea.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gthtunwqaj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gttvcpazjb.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtfvalvvmg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtoiuqujvr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.havefunace.top/gtuhyznfct.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sweek.top/gtqhstcald.html

[N11] 二叉树中序遍历
来源：http://hz.yongpay.top/gtsandcfrw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sxryk.cn/gtpzettnai.html

PHP:  // 手写递归函数
来源：http://hz.zhiwuduotai.top/gtxmjyfapf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtypvcstus.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtwascucry.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtfejtvvkl.html

Go:   // 手写递归
来源：http://hz.jqgufenzy.top/gtepsfnplm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtucbddsky.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gthcgnozpi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ivvv.top/gtxrqsafjd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xylfe.cn/gtsgdwjfiu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtgptauuwg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtpfareguv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtgrddvige.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtatpfenwd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sufxvd.cn/gtdqyetmzs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnqzz.top/gtjxeithsy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtxfqtxdwh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgefvqjmd.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gtttodmxff.html

================================================================================
来源：http://hz.dashuyun.cn/gtjhvuazym.html

[O01] 启动一个线程
来源：http://hz.haohaochexian.top/gtsyqeapaw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ivvv.top/gtmwkijxru.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gteejvxkrj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yanxiufei.cn/gtiqmzucpk.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtgwjlnxgr.html

Java: new Thread(() -> f()).start()
来源：http://hz.bjfxy.top/gthjobpanp.html

Go:   go f()
来源：http://hz.hnqzz.top/gtmqlzjbeg.html

Ruby: Thread.new { f }
来源：http://hz.yongpay.top/gtffmrttvp.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtzlyomtnu.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtadhpkmei.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtkqnabmeu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhongyouzk.top/gtnlbuimnf.html

JS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtxoobrgfb.html

TS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gteqbyfmvp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aizwys.cn/gtcadvkqfb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gtdatahfus.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yueranfly.top/gtmilfmevp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.pengpengdd.cyou/gteymmivcd.html

[O03] 加锁保护共享数据
来源：http://hz.9152youxi.cn/gtgpdhlooa.html

Py:   with lock: shared += 1
来源：http://hz.chenzaomai.com/gtlllbyhtv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zycfv.cn/gtjwymfdwu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtiurqjbfb.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtjztsveje.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtflrhuxio.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.birdmap.top/gtzuqwvngr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xinyue.icu/gtfhbwnshp.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtcidyauwf.html

[O04] 定义异步函数并等待
来源：http://hz.yanxiufei.cn/gtanvfzygw.html

Py:   async def f():⏎    await g()
来源：http://hz.haohaochexian.top/gtlwiqtups.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dianchejie.cn/gthpkojetg.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gtdmlnxgnt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aibaodan.cn/gtavsurtxk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daxiang520.top/gtyzrgqare.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhengqikj.top/gtqgelxgzz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinyuanbaomall.cn/gtiblnytxh.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtywbuhuii.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gtkpazxmck.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtngytfnbg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangshuangyany.cn/gtzstwpbmc.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtimcprguq.html

TS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtkqrlvkfw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.vqdsnc.cn/gtyssbping.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gtdvfvgmvl.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gtxvsvnfhp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gogol.net.cn/gtlkgephso.html


<!-- 参考信息 -->