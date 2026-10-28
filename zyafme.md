代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gtbkwdrtbp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuanzx.com/gtahlgiqsj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtrqiztcmr.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtwnftntse.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtvokttmsy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtjoboivhs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtwqjrerwp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtzvfbdvcf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtsaomymrp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jiagoushi.top/gtwmhgywan.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fengsongda.top/gtsaokqkxv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aibaodan.cn/gtyvrlcvhi.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gtzzqvwzcr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.havefunace.top/gtjyzjzrjb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shzxlz.cn/gtcwbdyblq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtqqkazqaf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtujkpnerk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtofqzfogy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.mhx1999.top/gtrgnzbfxq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gtyxybksnu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yueranfly.top/gtpocoxcpn.html

[L04] 设置超时
来源：http://hz.jiagoushi.top/gtgknjlxkz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtsesykzih.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtoicjgvqk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtamhzqvxh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtyawamlga.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cashguo.top/gtillvjfwc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.andypj.xyz/gtaherevgt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nwbrower.top/gtsfqfvaeu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.havefunace.top/gtppcifevm.html

[L05] 上传文件（multipart）
来源：http://hz.vqdsnc.cn/gtafnzxefd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhaomingkeji.xyz/gtjpuleiam.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ywan-chungtsiang.top/gthmsmtbfb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtikxjivwq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtknmmtxye.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zycfv.cn/gtzwxawadh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shuidangran.top/gtdzucjujq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jlsjyb.cn/gtyltljuag.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.52xcode.cn/gtnnitntrc.html

[L06] 解析响应为 JSON
来源：http://hz.chenjidiqi.icu/gtwpcqdqby.html

Py:   resp.json()
来源：http://hz.aizwys.cn/gtlmyplkuk.html

PHP:  json_decode($body, true);
来源：http://hz.bjfxy.top/gtsykxydkr.html

JS:   await resp.json()
来源：http://hz.316326.xyz/gtwuncqxnp.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtiaixyvpg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gtvyycfnrl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtkyadbhnm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtivrpyxkw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtcisqhsoi.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gthgathkdk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ivvv.top/gtjytxqyje.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtwcimkmaq.html

JS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtkhwjpvka.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtdwfoiwiq.html

Java: resp.statusCode()
来源：http://hz.yj202588.top/gtrkcmanzk.html

Go:   resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtaunsoeuw.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtyetojurp.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtkiszzqca.html

[L08] 并发请求多个地址
来源：http://hz.hysaishi.cn/gtgwbsukwc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tianlin.xyz/gtbvdtrpwh.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtgzqhuing.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtjuqdmlli.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gthhpvcozc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.birdmap.top/gtqfujddbj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ywan-chungtsiang.top/gtjvjxydmk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.andypj.xyz/gtzfuaavwr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gtohgtnmkw.html

================================================================================
来源：http://hz.tianlin.xyz/gtwcacltvh.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangdashe.top/gtgjtrojlo.html

================================================================================
来源：http://hz.sufxvd.cn/gtvjqqetcm.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtqdygxqfq.html

Py:   sys.argv[1:]
来源：http://hz.aibaodan.cn/gtgdzgjctt.html

PHP:  $argv;  $argc;
来源：http://hz.hongshengwenyu.top/gttofxrdwt.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gteuzboxgm.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtuicacoov.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxuanxn.top/gtncodmznl.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gtisykhwgw.html

Ruby: ARGV
来源：http://hz.zycfv.cn/gtengsekri.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gthsnuoorx.html

[M02] 读取环境变量
来源：http://hz.jyoumei.cn/gtkvjfnfan.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gtqzwqgjxx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtcxhtlcvn.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtnahqyoou.html

TS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtoekkvtur.html

Java: System.getenv("HOME")
来源：http://hz.hfpthk.cn/gtdffselgd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cheryme.top/gtntiqltpn.html

Ruby: ENV["HOME"]
来源：http://hz.hnqzz.top/gtidscqybf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.c1oappe.top/gtlaituezu.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtucuxmvfd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinyuanbaomall.cn/gtiwlogine.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xziqi.cn/gtiqlzzvcr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtppbrhbpf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtxldisxms.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cqqwz.cn/gtmspzgdqe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gthrgjkglt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ivvv.top/gtemncjnto.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gzhubu.top/gttwypiasd.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtjluugbmh.html

Py:   os.getcwd()
来源：http://hz.zhijiandao.cn/gttascoxrh.html

PHP:  getcwd();
来源：http://hz.zdqjudy.top/gtnwjovqdv.html

JS:   process.cwd()
来源：http://hz.chenzaomai.com/gtbajzipwm.html

TS:   process.cwd()
来源：http://hz.zycfv.cn/gtrnwruisl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.snrcjt.cn/gtsoeurfpd.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtkiqftxhs.html

Ruby: Dir.pwd
来源：http://hz.zhijiandao.cn/gtlcaqkzlp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj20258888.top/gtvkrardeu.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gttrcvowuf.html

Py:   sys.exit(1)
来源：http://hz.ydjk.org.cn/gtanccyumk.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtkjmumvfp.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtlwyktaqy.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtnmswmmmi.html

Java: System.exit(1)
来源：http://hz.shuidangran.top/gtwfgazodb.html

Go:   os.Exit(1)
来源：http://hz.yuxming.cn/gtfbbtwdjh.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtnalpyrbo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cucudq.cn/gtexnrujjx.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gteezrlxfu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtmhcbagpn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtncaidpjb.html

JS:   console.error("err")
来源：http://hz.jqgfzy.top/gtaeixapma.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtbmegnbsy.html

Java: System.err.println("err")
来源：http://hz.jianghu66.top/gtaflxtqac.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tian-w.cn/gteszfxanc.html

Ruby: warn "err"
来源：http://hz.yanxiufei.cn/gtufqtistb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtbuzhpdkq.html

[M07] 判断是否为主入口
来源：http://hz.wangdashe.top/gtnazamnqp.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtwkauxkka.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtiajdolrk.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtovbpqsau.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtpnjqejtv.html

Java: public static void main(String[] args)
来源：http://hz.gotoacloud.top/gteofnfqzn.html

Go:   func main()
来源：http://hz.yj20258.top/gtowikfmrg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangtech.top/gtjkttmvie.html

C#:   static void Main(string[] args)
来源：http://hz.jianghu66.top/gtmmaettlg.html

[M08] 获取系统与运行时信息
来源：http://hz.zhixingplan.top/gtfnnwjsrc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtwalmowxj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sufxvd.cn/gtxmjyusaa.html

JS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtdqwnspfd.html

TS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtglalqeuu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj202588.top/gtltcjgqvw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gtuxxejzan.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtrcgqpmlx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dashuyun.cn/gtmeqtkmmi.html

================================================================================
来源：http://hz.cucudq.cn/gteytaedwq.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gtlaldbqit.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcmhnoblh.html

[N01] 二分查找（有序数组）
来源：http://hz.hongshengwenyu.top/gtavdafobi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gzhubu.top/gtipwpjgzx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258.top/gtqgyoadbq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtecnvrenb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtpoooawhi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtshgjjqdc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtifjnuzty.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtjbfevdyk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258.top/gtpypdflor.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuanzhike.top/gtkrrteblb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtjymbxjwf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ehwqpu.com/gtriyxbqjb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtsiyythme.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtnoesoriz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dashuyun.cn/gtdpwnjrrh.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtbpzpeyea.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtdtiobcrz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gtjvzxxdwg.html

[N03] 快速排序（分治示例）
来源：http://hz.jiagoushi.top/gtiyuqhybv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cucudq.cn/gtrvmrlcnc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.9152youxi.cn/gtaefexdwg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtyelnrctc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtubezeyqu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.0kj1m.cn/gturapecjy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gaohongyu789.top/gtizpamain.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.meibo888.top/gtdnpmqrzl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtwqekkgei.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gtvgswvvlf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtdvduudut.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.meibo888.top/gtsxgaepvz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtwtzmhucl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtsyuqunjc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dianchejie.cn/gtteehktyl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xylfe.cn/gtnoqdbtoc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtjqosdcsm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtsqrtifrr.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtlpolxvst.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gthehyeoce.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sweek.top/gtgsajoqiy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gthxevszkx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtnkdtpddh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtfdumamwl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xylfe.cn/gtpkwkeexv.html

Ruby: a.gcd(b)
来源：http://hz.shuidangran.top/gtaqfguois.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinghuilouyu.cn/gttmonutbi.html

[N06] 判断回文字符串
来源：http://hz.gzhubu.top/gtnftfjzge.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtdelrzcrs.html

PHP:  $s === strrev($s);
来源：http://hz.hywenlv.cn/gtxwnejlsg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtlyijmmcf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtjpjogpas.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtzghwkunw.html

Go:   // 双指针从两端比较
来源：http://hz.shanyushiyangkeji.top/gteqzollzp.html

Ruby: s == s.reverse
来源：http://hz.zhijiandao.cn/gtkpuugbwu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangkeji.top/gtqokfqazm.html

[N07] 两数之和（返回下标）
来源：http://hz.daria6918.cn/gttjpmenof.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtnxumepmw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtuwxctncx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydjk.org.cn/gtmcpweqah.html

TS:   // 手写 Map<string, number>
来源：http://hz.zycfv.cn/gtkrebwrvl.html

Java: // 手写 HashMap
来源：http://hz.hnxiangtu.top/gtntcqtfxp.html

Go:   // 手写 map[int]int
来源：http://hz.yj202588.top/gtwnwrhzwv.html

Ruby: // 手写 Hash
来源：http://hz.zhiwuduotai.top/gtkqgzicuz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jlsjyb.cn/gtmkranwoi.html

[N08] 生成全排列
来源：http://hz.shzxlz.cn/gtvblwiovs.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtobifppww.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtpdwzcabo.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtkwxdxufr.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gttikkztmj.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtiwzskxbf.html

Go:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtbjrvkrzg.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxuanxn.top/gtnsypppmg.html

C#:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtjlhceqio.html

[N09] 栈与队列
来源：http://hz.jlsjyb.cn/gteijjfgsv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtcnridndq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yvedp.cn/gtasryqrxv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnqzz.top/gtrnyegsrv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinghuilouyu.cn/gtezpsjlod.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ywan-chungtsiang.top/gtnbsdujhd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hammf.cn/gthebdlvta.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gtyfizwcof.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yongpay.top/gttxztslha.html

[N10] 链表节点定义
来源：http://hz.cqqwz.cn/gtcggbvzur.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xuanzx.com/gtzlosiesr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtmcgboywv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yanxiufei.cn/gtclfpldqb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zdqjudy.top/gtvqwjgqxy.html

Java: class Node { int v; Node next; }
来源：http://hz.ppjwa.cn/gtbytkbati.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.quarkkingdee.top/gtpttpqgps.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shuidangran.top/gtknyilbai.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenjidiqi.icu/gtjzzmjfuh.html

[N11] 二叉树中序遍历
来源：http://hz.jinghuilouyu.cn/gtiqyqrkwq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aibaodan.cn/gtznkoxssk.html

PHP:  // 手写递归函数
来源：http://hz.meibo888.top/gtzqhshqff.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtunfjuaxy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtbxirddqk.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gtnooprsxn.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtfhmhltgy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guannengcc.top/gtjtiexkad.html

C#:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtxwjnguyn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hammf.cn/gtqgjmlhiv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.aizwys.cn/gtpjyycjea.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daxiang520.top/gtwxtlnyiu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.52xcode.cn/gtarbfayne.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtapidscdu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtkwtspfsk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ehwqpu.com/gtelcluyov.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhixingplan.top/gtjowoadsi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtargooebv.html

================================================================================
来源：http://hz.tianlin.xyz/gtfbdlekct.html

O. 并发与异步
来源：http://hz.zhijiandao.cn/gtgvmeqqvu.html

================================================================================
来源：http://hz.dashuyun.cn/gtgoziipbg.html

[O01] 启动一个线程
来源：http://hz.yj202588.top/gtiwumkpde.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gotoacloud.top/gtgsdjhhdj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.smart0.xyz/gtstmasevp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gtrqpmrrjs.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtvkcahkcs.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtndjbmwrk.html

Go:   go f()
来源：http://hz.cqqwz.cn/gtazmhkbpb.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtwecfxond.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtucjmmsay.html

[O02] 使用线程池
来源：http://hz.fengsongda.top/gtecizcghz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtanooqyaa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zdqjudy.top/gtubtcbphb.html

JS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtjkqlmbkd.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtrdudrphc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gtbyhfpomz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnxiangtu.top/gtrtvtsrkv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.svipenyu.cn/gtgdogmrxw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtujcrcqji.html

[O03] 加锁保护共享数据
来源：http://hz.hongshengwenyu.top/gtaqruqwaj.html

Py:   with lock: shared += 1
来源：http://hz.cdnleiting.top/gtzmrwvrel.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gzhubu.top/gttajawmui.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gthyrztfbk.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtmjriowzl.html

Java: synchronized (this) { shared++; }
来源：http://hz.sxryk.cn/gtezpebjtz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jyoumei.cn/gtgclcgqow.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gtszqfjade.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj202588.top/gtbymdedzg.html

[O04] 定义异步函数并等待
来源：http://hz.pycfn.com/gtrsvkihgj.html

Py:   async def f():⏎    await g()
来源：http://hz.ydjk.org.cn/gtqpnazhzf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtqjadlvsd.html

JS:   async function f() { await g(); }
来源：http://hz.nwbrower.top/gtnyqgofci.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.bjfxy.top/gtjmkvsbqy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuetiantiany.cn/gtxqgxkdbp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gtlaatwlxx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ehwqpu.com/gtaajojige.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gtlppljndd.html

[O05] 并发执行并等待全部完成
来源：http://hz.hammf.cn/gtjtxjpgcb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.quarkkingdee.top/gtktyjprux.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hysaishi.cn/gtmfsjrrps.html

JS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtafmxjdub.html

TS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtdtcimofl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gtrkqqvyvf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yueranfly.top/gtwqkxiudr.html

Ruby: threads.map(&:join)
来源：http://hz.ywan-chungtsiang.top/gtjevluidh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hammf.cn/gtudkvirtf.html


<!-- 参考信息 -->