代发 wailian999

L. 网络请求
来源：http://hz.hnqzz.top/gtiexfncdb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtszjicnjg.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtlncpxtfd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jlsjyb.cn/gtfxyqwcyt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shzxlz.cn/gtdqvlfaip.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtvnuznsbg.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtqhygapau.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gotoacloud.top/gtacqwyeog.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gtomkizarl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtivizorps.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.aizwys.cn/gtppzzxdae.html

[L02] 发送 POST JSON
来源：http://hz.hysaishi.cn/gtpbnpvevo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gtjdpivpvt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.redwolf501.top/gtvczdmdrp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtppvzadxe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtnhajjmjr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tanke756.top/gthpktqwwx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnqzz.top/gtlydurnpp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.snrcjt.cn/gtcaitufcl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gtrsfmtnmi.html

[L03] 设置自定义请求头
来源：http://hz.ywan-chungtsiang.top/gtwdsfrvax.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gttyjlmqzq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pengpengdd.cyou/gtzkdhpdnz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtdvrklnoz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtydejwage.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtksssdrsp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtgvakcljt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtvpwllcdo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydjk.org.cn/gttvidfuhe.html

[L04] 设置超时
来源：http://hz.sweek.top/gtjgogwylv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtrnjcermr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.redwolf501.top/gtzxwqfssi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtpaztgwus.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtswciyean.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.svipenyu.cn/gtbzzcftfc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yonumen.top/gtltzoknnh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gthqsgrgwx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.meibo888.top/gtirmcdrja.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtvklohrpg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuanzx.com/gtqsaltphu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.birdmap.top/gtryjbciwh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtupoofrzf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtwfynyocd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtlgpamocd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yueranfly.top/gtwnpfdmcu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtqctakvjn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtoboeklpm.html

[L06] 解析响应为 JSON
来源：http://hz.nanxuanxn.top/gtvatedpus.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtadcvjfsw.html

PHP:  json_decode($body, true);
来源：http://hz.cdnleiting.top/gtgqvysuti.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gttgrdkscx.html

TS:   await resp.json()
来源：http://hz.svipenyu.cn/gtgljgroto.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydzc1.top/gtkximmuwh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pengpengdd.cyou/gtottkuqls.html

Ruby: JSON.parse(resp.body)
来源：http://hz.haohaochexian.top/gtekvvbgzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtpvjcqxgu.html

[L07] 处理 HTTP 状态码
来源：http://hz.zycfv.cn/gtbdhttmxp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtpkjttdeu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtwhnoibmj.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtzjgcrbtq.html

TS:   resp.ok;  resp.status
来源：http://hz.shuidangran.top/gticubsxyo.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangkeji.top/gtzrsmjbwx.html

Go:   resp.StatusCode
来源：http://hz.andypj.xyz/gtzgghcqzn.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gtaugrleft.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gtjcxeoxra.html

[L08] 并发请求多个地址
来源：http://hz.fzhhl.top/gttieuiukw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gtudcmggce.html

PHP:  curl_multi_init() 系列
来源：http://hz.tian-w.cn/gtrlemxwzx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtnkulwxje.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gttvvatmlp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xylfe.cn/gtucfyjxak.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sxryk.cn/gtotjioncn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gogol.net.cn/gttptcjfjr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtrxtaycyj.html

================================================================================
来源：http://hz.bjfxy.top/gtcnkiblvy.html

M. 命令行 / 进程 / 环境
来源：http://hz.yonumen.top/gtmsqwphos.html

================================================================================
来源：http://hz.haohaochexian.top/gtvumqovrz.html

[M01] 读取命令行参数
来源：http://hz.pengpengdd.cyou/gtgsdqwjsr.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gtunkppgob.html

PHP:  $argv;  $argc;
来源：http://hz.jqgufenzy.top/gtbofgvmyd.html

JS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gttqvtkmni.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtgmjqpowq.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtxzwqirno.html

Go:   os.Args[1:]
来源：http://hz.cheryme.top/gtfcjyiapy.html

Ruby: ARGV
来源：http://hz.dashuyun.cn/gtcevcftit.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guowangkeji.top/gtndmahvmy.html

[M02] 读取环境变量
来源：http://hz.dianchejie.cn/gtqjnfrger.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtehieptui.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhongyouzk.top/gtgeloeheo.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtgtmtpdwz.html

TS:   process.env.HOME
来源：http://hz.yuanzhike.top/gtatwrqphc.html

Java: System.getenv("HOME")
来源：http://hz.jlsjyb.cn/gtoosampze.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.iojbl.cn/gtmryljgmo.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gthswcbjsv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pycfn.com/gtjzryqrqw.html

[M03] 执行外部命令
来源：http://hz.52xcode.cn/gtmrqitzjz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtqlrmxgci.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258888.top/gtjajijwmm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gtxwjlkkqw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtrathplwz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ppjwa.cn/gtjirindes.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258.top/gtulwzvppi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aibaodan.cn/gtcnqzkphm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gtfejxongh.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtsxygkskk.html

Py:   os.getcwd()
来源：http://hz.zhaomingkeji.xyz/gtyyludwyl.html

PHP:  getcwd();
来源：http://hz.gotoacloud.top/gtzuldtldf.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtgyrpyzyh.html

TS:   process.cwd()
来源：http://hz.fengsongda.top/gthdorgiqr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtvhlhcjwf.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gtvvemiaxs.html

Ruby: Dir.pwd
来源：http://hz.xylfe.cn/gtbuqlaukk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtnsuhcohb.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtrzdckpeo.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gtgdietjyb.html

PHP:  exit(1);
来源：http://hz.chenjidiqi.icu/gtgwwpryvm.html

JS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtbfegvthd.html

TS:   process.exit(1)
来源：http://hz.andypj.xyz/gtbpeqdtuy.html

Java: System.exit(1)
来源：http://hz.jlsjyb.cn/gtsdqwgpez.html

Go:   os.Exit(1)
来源：http://hz.0kj1m.cn/gtwvyntzfg.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gttgxtfged.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gtegrlzpcb.html

[M06] 向标准错误输出
来源：http://hz.sufxvd.cn/gtxuoqlptl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtgudeakhx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tianlin.xyz/gtfkhmxigk.html

JS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtokfybupp.html

TS:   console.error("err")
来源：http://hz.gogol.net.cn/gtdmotjhzy.html

Java: System.err.println("err")
来源：http://hz.jinqigfzy.top/gtyugwzehj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtgslxuych.html

Ruby: warn "err"
来源：http://hz.nanxuanxn.top/gtmnlvodhy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guannengcc.top/gtzryyuvdc.html

[M07] 判断是否为主入口
来源：http://hz.zhixingplan.top/gtotwfstxt.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtzgzetjza.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xziqi.cn/gtivpbeehc.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtflsbsdik.html

TS:   require.main === module
来源：http://hz.hammf.cn/gtoohangbd.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gttabdjbxv.html

Go:   func main()
来源：http://hz.shanyushiyangtech.top/gtktdmuwif.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gtfwoffumk.html

C#:   static void Main(string[] args)
来源：http://hz.yangfankeji.com/gtwnorokwr.html

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gtuvvvnzmu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangdashe.top/gtjcqnmfkv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtjmiwhoee.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtcbpoljta.html

TS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtliywcxtn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gtxrdgagyh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gtbidqthst.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pengpengdd.cyou/gtzftzzeen.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gtyjvrenlh.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtbxapkwzn.html

N. 数据结构与算法
来源：http://hz.cdnleiting.top/gtsstjewzm.html

================================================================================
来源：http://hz.hnxiangtu.top/gtkeebveho.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangkeji.top/gtnzkdascu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258888.top/gtqilkznil.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ybcxt.top/gtkipermse.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtomousyed.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtcxffhdvh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtnjplfrom.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shzxlz.cn/gtnvahuhom.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtdjzwzgzb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.52xcode.cn/gtaexxdcwq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gtmtvdyodw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtawgkbnhu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtcnaplagv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtarffdlqu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtxfynjfdc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xinyue.icu/gttegzbmlt.html

Go:   slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtzjtzefdt.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtxuzplvin.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gtkmblsqwk.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gthvwleplt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yueranfly.top/gtxvccpbwm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtrfixsijx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yangfankeji.com/gtcvofdtmk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtxqqoarwk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jiagoushi.top/gthjvfsslx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gttfpiiemx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gtczgjuwvq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenzaomai.com/gtbamlnonq.html

[N04] 斐波那契数列
来源：http://hz.yj20258.top/gtmxmcggig.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtqjbgtmee.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtwcmfjwsa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtodfsmmlu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtocpqsjwm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtuwdinxyi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gtymvsjpix.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtjjswjyaw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtzhezccjl.html

[N05] 最大公约数
来源：http://hz.jyoumei.cn/gtizzuxhza.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gtdfdaxkvt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.bjfxy.top/gtqdwtqswk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtfvjyygxm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtannoctse.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnqzz.top/gtjqdtrgyr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ehwqpu.com/gtmhfqwcau.html

Ruby: a.gcd(b)
来源：http://hz.mhx1999.top/gtrgbyirhh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxinkj.top/gtaqkgnvzz.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtivpzcpau.html

Py:   s == s[::-1]
来源：http://hz.kuanghao11.cn/gtuwnmyrws.html

PHP:  $s === strrev($s);
来源：http://hz.shzxlz.cn/gtuoufcdsl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gthrsbavpf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtqydnqigj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gtbuwuykit.html

Go:   // 双指针从两端比较
来源：http://hz.cheryme.top/gtovedpewp.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtwarkqrro.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtkguehdos.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gtidzljbnb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hammf.cn/gtodmhxbdm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.snrcjt.cn/gtnzegddlf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ehwqpu.com/gteugvgkmw.html

TS:   // 手写 Map<string, number>
来源：http://hz.sufxvd.cn/gtaambguuk.html

Java: // 手写 HashMap
来源：http://hz.redwolf501.top/gtcuvicimb.html

Go:   // 手写 map[int]int
来源：http://hz.bjfxy.top/gtlamvptjp.html

Ruby: // 手写 Hash
来源：http://hz.fengsongda.top/gtptdpwpev.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gteanrseaz.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtfddrezyd.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigufen.top/gtuyejgjly.html

PHP:  // 手写递归交换
来源：http://hz.zhongyouzk.top/gtliwbsrgs.html

JS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtvalqiluc.html

TS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtashcqnws.html

Java: // 手写回溯递归
来源：http://hz.sysykeji.top/gtykdmzgyz.html

Go:   // 手写回溯递归
来源：http://hz.yj20258.top/gtinarhkbz.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtljhlcxra.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtfkaycxvg.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtvvklfdci.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tanke756.top/gtahasvwou.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtphtwepuj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtwkeavxqd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hammf.cn/gtszuwovrp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hysaishi.cn/gtuvyywdwi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtaytvvkhk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtwcenegvi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jqgfzy.top/gtlggbimui.html

[N10] 链表节点定义
来源：http://hz.zdqjudy.top/gtmanjzpul.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gtlonywcev.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydjk.org.cn/gttigtwonh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.redwolf501.top/gtkepowafl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jyoumei.cn/gtmbhdyfsc.html

Java: class Node { int v; Node next; }
来源：http://hz.shangyingyoupin.top/gtflsbzzqp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuanzhike.top/gtlranfehv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gttkdbrlwi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtcblrzkys.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtkgqtukwq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gtpzbwhhnb.html

PHP:  // 手写递归函数
来源：http://hz.svipenyu.cn/gtyltdokbj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhijiandao.cn/gtegyzvawb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtslryetfm.html

Java: // 手写递归
来源：http://hz.pycfn.com/gtuulepsbj.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtmckvfvch.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuanzhike.top/gtotmkyzio.html

C#:   // 手写递归
来源：http://hz.fzhhl.top/gtxpkmquco.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shzxlz.cn/gtiwvctiyw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nwbrower.top/gtxbsrgvnj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tanke756.top/gtgeqlbzzt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gtfvcdipwz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gttknwtdzu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtuvugzkac.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtbcvmdabe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gtdxpywlit.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zdqjudy.top/gtvcmhklpo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgfxodisy.html

O. 并发与异步
来源：http://hz.dianchejie.cn/gticojbkzc.html

================================================================================
来源：http://hz.dashuyun.cn/gtwljmrlnd.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtjycnaubk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.vqdsnc.cn/gttxoqcpod.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtdakztewi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangdashe.top/gtdemlfagn.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtmyvrpqva.html

Java: new Thread(() -> f()).start()
来源：http://hz.dianchejie.cn/gtskjutujy.html

Go:   go f()
来源：http://hz.nanxuanxn.top/gtlbvwmhdw.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtocpiyamz.html

C#:   Task.Run(() => F());
来源：http://hz.nwbrower.top/gtbevxqpwq.html

[O02] 使用线程池
来源：http://hz.aizwys.cn/gtrhcccorr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtjrdjmcbo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtadugenws.html

JS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gttsredwzg.html

TS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtkpbfjhpd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuanzhike.top/gtkfzwxwle.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnqzz.top/gtqsdqrnjs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.vqdsnc.cn/gtakjswrdf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtukuzjcug.html

[O03] 加锁保护共享数据
来源：http://hz.ywan-chungtsiang.top/gtzsqslxom.html

Py:   with lock: shared += 1
来源：http://hz.smart0.xyz/gtjzqznqiw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258.top/gtasmajsef.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtbizqhuly.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtxjvenqqs.html

Java: synchronized (this) { shared++; }
来源：http://hz.wangdashe.top/gtgoiwrjoo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxuanxn.top/gterhjsfob.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtpgolrujw.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhiwuduotai.top/gtzryduwqy.html

[O04] 定义异步函数并等待
来源：http://hz.shangyingyoupin.top/gtxjplxjnb.html

Py:   async def f():⏎    await g()
来源：http://hz.zhixingplan.top/gtwzerbmom.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aibaodan.cn/gtbudeqgsr.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangkeji.top/gtlhzgjufb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tian-w.cn/gtrqsnlljf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cucudq.cn/gtyxkjypyb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guannengcc.top/gtsygikcen.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgufenzy.top/gtwwruacjz.html

C#:   async Task F() { await G(); }
来源：http://hz.fzhhl.top/gtjdwunxek.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtrvdqdrom.html


<!-- 参考信息 -->