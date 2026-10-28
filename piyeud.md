代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangtech.top/gtwnzqmlfy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenlongwang.top/gtagumttwb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jiagoushi.top/gtqrawvihf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dashuyun.cn/gtuaswksan.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtjtrrcsbq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tianlin.xyz/gtripnyngg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cucudq.cn/gtgzenehxu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtzszcsqhg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtxpznwwws.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtdssmdezp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtcoipnhjm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jlsjyb.cn/gtteseuxmp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtfkcajdps.html

[L04] 设置超时
来源：http://hz.cashguo.top/gtdsawtwhx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gtgirefffi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtioxfzlfh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtmwavosre.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtquutozeg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgfzy.top/gtanbjobqx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sufxvd.cn/gtriatjnhg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtvetqzqbk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pengpengdd.cyou/gtsvvteenr.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gtlqmjjvga.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xingfuxueyuan.xyz/gtqtzhkjnx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gthohjqxfh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtxrruwrkd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtopiowwyx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gtcfnuvdlp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtagkicxbz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtpdokqhjy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yueranfly.top/gtvoyzzjbx.html

[L06] 解析响应为 JSON
来源：http://hz.gogol.net.cn/gtsfgmuqxl.html

Py:   resp.json()
来源：http://hz.jinyuanbaomall.cn/gtnozbamau.html

PHP:  json_decode($body, true);
来源：http://hz.xylfe.cn/gtmxuvktkj.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gthchnawmw.html

TS:   await resp.json()
来源：http://hz.zhixingplan.top/gtltbpgvdm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtkzpjfhsg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhoulong.xyz/gtsydimfgj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.dashuyun.cn/gtbxhykuiv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuxming.cn/gtijltbcge.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtruppemvy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jianghu66.top/gtkwztajoa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtytysxucn.html

JS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtxskjujbg.html

TS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtddfnbrrn.html

Java: resp.statusCode()
来源：http://hz.smart0.xyz/gtjfjbktdm.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtwolhcxks.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtqcvndvco.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtxzrudtme.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gtzbdbkebc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.kuanghao11.cn/gteghjwdtx.html

PHP:  curl_multi_init() 系列
来源：http://hz.aibaodan.cn/gtrctcwnvh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtjyacphfe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtpahpntrh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xylfe.cn/gtohyrlddb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cdnleiting.top/gtjwwbwvyw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.svipenyu.cn/gtofythuwx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yvedp.cn/gtwzdvhfcw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtpsylmfgv.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtdnmglvhw.html

================================================================================
来源：http://hz.cashguo.top/gtdvxewcfu.html

[M01] 读取命令行参数
来源：http://hz.xuanzx.com/gtqyknhsag.html

Py:   sys.argv[1:]
来源：http://hz.vqdsnc.cn/gtkpsnzzur.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtrzetvlfc.html

JS:   process.argv.slice(2)
来源：http://hz.cdnleiting.top/gthivwqxnm.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtmnixifyx.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtrxynnrmh.html

Go:   os.Args[1:]
来源：http://hz.kuanghao11.cn/gtickjbejt.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gtaamfkngn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sysykeji.top/gtyvrzswev.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtqodcczhx.html

Py:   os.environ.get("HOME")
来源：http://hz.hywenlv.cn/gthvbbuixq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtcjtryzhg.html

JS:   process.env.HOME
来源：http://hz.smart0.xyz/gtfbtdgfum.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gtmoxvvqpe.html

Java: System.getenv("HOME")
来源：http://hz.yj20258888.top/gtefpbwmsl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtrhbsjocu.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gthayygwkq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gzhubu.top/gtbfklzdqg.html

[M03] 执行外部命令
来源：http://hz.sxryk.cn/gtmwjpcces.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dianchejie.cn/gtplvfqqty.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtsimoumfn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtzzdtwcgw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtgvcsgqzz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtmaipjfgf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtuxwxiesu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.snrcjt.cn/gtfbybdxrg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cqqwz.cn/gtxygonomd.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gthuwlfvnw.html

Py:   os.getcwd()
来源：http://hz.chenlongwang.top/gtbkdbqrtg.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gtqnvmyebn.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtwoplfoae.html

TS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtxabpzssw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.meibo888.top/gthhnruruz.html

Go:   os.Getwd()
来源：http://hz.feifeiyinyue.top/gtxfjkogij.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gtbdjiraom.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigfzy.top/gtrygqucug.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gtfprtlnsl.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtcndpysaf.html

PHP:  exit(1);
来源：http://hz.haohaochexian.top/gtfjawsnjj.html

JS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtgxmbcmaz.html

TS:   process.exit(1)
来源：http://hz.ydzc1.top/gtovvargvx.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtxbtvmawl.html

Go:   os.Exit(1)
来源：http://hz.aizwys.cn/gtxuhkrqfe.html

Ruby: exit 1
来源：http://hz.yj20258888.top/gtudsrgkrc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtsalgbuzi.html

[M06] 向标准错误输出
来源：http://hz.ppjwa.cn/gtpkfqdxdd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtmirpgmua.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtliwxynpr.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtahobqomm.html

TS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gttmajzlki.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtfguiekpe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtxmbazpqz.html

Ruby: warn "err"
来源：http://hz.zhengqikj.top/gtpvqoxivd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtykpwcizm.html

[M07] 判断是否为主入口
来源：http://hz.ehwqpu.com/gtolkxkosq.html

Py:   if __name__ == "__main__":
来源：http://hz.ybcxt.top/gtdgubjkdj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtibpckzqt.html

JS:   require.main === module
来源：http://hz.cheryme.top/gtuqrqrufc.html

TS:   require.main === module
来源：http://hz.svipenyu.cn/gtftaqgozh.html

Java: public static void main(String[] args)
来源：http://hz.tian-w.cn/gtojsuwizk.html

Go:   func main()
来源：http://hz.wangshuangyany.cn/gthbflzntf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtllydtqie.html

C#:   static void Main(string[] args)
来源：http://hz.chenjidiqi.icu/gthilfnvcj.html

[M08] 获取系统与运行时信息
来源：http://hz.guannengcc.top/gtwcwgtlql.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtqlrmtzij.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pengpengdd.cyou/gtzifldzgb.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gteokvcgph.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtignpwxay.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gtzedrsujh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zdqjudy.top/gtogtwflch.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangkeji.top/gthytppfom.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gtwfxclmau.html

================================================================================
来源：http://hz.hnqzz.top/gtfdulyuzn.html

N. 数据结构与算法
来源：http://hz.yonumen.top/gtubrgnelr.html

================================================================================
来源：http://hz.tian-w.cn/gtwvexsxml.html

[N01] 二分查找（有序数组）
来源：http://hz.sysykeji.top/gttdforwof.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tianlin.xyz/gtafquwemp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuanzhike.top/gtnteldlde.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtnbxiewhd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtsczpgflw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtzyngeore.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ybcxt.top/gtxqtwiebu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtnlvhfpzp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sxryk.cn/gtthquemft.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yonumen.top/gtjxonfnug.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtduwwfczj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtyoeewlgd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtopthyucx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gttyfzkhhl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ywan-chungtsiang.top/gtmqyqphpy.html

Go:   slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtbvcwyown.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gteznvudoq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnxiangtu.top/gtolbmvfgq.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258888.top/gtxnjacvrw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtszpcaduq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tianlin.xyz/gtfomchnpg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtrqkyujze.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtykyemopl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtorhlhovd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.daxiang520.top/gtskrduymx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gzhubu.top/gtprdngrlv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydjk.org.cn/gtqvoivhbq.html

[N04] 斐波那契数列
来源：http://hz.9152youxi.cn/gtvvzgcmqa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gtouuxjckg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.svipenyu.cn/gtprsqdump.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtytyofnjg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.mhx1999.top/gtofslpqux.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgfzy.top/gtgxmgxiof.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtyhiiftns.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtnenigneo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cdnleiting.top/gtjcefcfjy.html

[N05] 最大公约数
来源：http://hz.jiagoushi.top/gtbzjalrmd.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtmnosbbej.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhijiandao.cn/gtnqlcdtyd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtprdyjnow.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtlgscmvvg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtncizyxbk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yanxiufei.cn/gtyppbmdiw.html

Ruby: a.gcd(b)
来源：http://hz.nanxuanxn.top/gtgxngmixb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yvedp.cn/gttvpvmuip.html

[N06] 判断回文字符串
来源：http://hz.c1oappe.top/gtoeuzcbth.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gttykgqcap.html

PHP:  $s === strrev($s);
来源：http://hz.hywenlv.cn/gtllpvidsa.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtpzinjfke.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gzhubu.top/gthjlxxlgk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhengqikj.top/gtovvhelka.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gtfbppeiqo.html

Ruby: s == s.reverse
来源：http://hz.ehwqpu.com/gttxqshiwd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtldnaamdx.html

[N07] 两数之和（返回下标）
来源：http://hz.yueranfly.top/gtxdtduyww.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangdashe.top/gttohdkhhl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shzxlz.cn/gtjsnfivyt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pycfn.com/gtmhnpijla.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gtoqfpmfzp.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gtnotlingg.html

Go:   // 手写 map[int]int
来源：http://hz.yongpay.top/gtlurzizch.html

Ruby: // 手写 Hash
来源：http://hz.cheryme.top/gtsaelxgts.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtxoxmzohx.html

[N08] 生成全排列
来源：http://hz.daxiang520.top/gttnysoywn.html

Py:   itertools.permutations(arr)
来源：http://hz.wangdashe.top/gteqckkzzd.html

PHP:  // 手写递归交换
来源：http://hz.shzxlz.cn/gtzpjapdjr.html

JS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtxkszlzqt.html

TS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtwfvmlywf.html

Java: // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtrikciqvl.html

Go:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtkebaqrqu.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtqhnuucns.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtwaldbcwl.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtwysthnst.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.c1oappe.top/gtccoxerjy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuanzhike.top/gtloaybzsu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gtybhgvcqw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gtnqtsfvtw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtddoktyfm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.kuanghao11.cn/gtdkwyyisd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cashguo.top/gtvuiojmtl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuanzhike.top/gtkatfcwbv.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gtfijhzvjc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dashuyun.cn/gtolmhqyzb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ppjwa.cn/gtvtvvapzz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtuthfzwnc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shangyingyoupin.top/gtxsqhlzhb.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gtrrpjdvyp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yangfankeji.com/gtcaynlfhf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yongpay.top/gtwsnnejbn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.smart0.xyz/gtxqwkcubb.html

[N11] 二叉树中序遍历
来源：http://hz.zdqjudy.top/gtcskuqbeu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhoulong.xyz/gtntmlimdb.html

PHP:  // 手写递归函数
来源：http://hz.ppjwa.cn/gtodonbvtj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gttbostdiu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtucwnveyd.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtwxpawgfn.html

Go:   // 手写递归
来源：http://hz.fzhhl.top/gtryoidgcy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenzaomai.com/gtpeodjxjv.html

C#:   // 手写递归
来源：http://hz.ybcxt.top/gtioheptpq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgufenzy.top/gtigimsbhj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pycfn.com/gtsmmiybwz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sxryk.cn/gtjipzcoag.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gtrqfpeknp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gtfubqcrpy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtkvudjtgl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daria6918.cn/gtmlvzfpnz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gtbqfknmif.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gtaiyfkkui.html

================================================================================
来源：http://hz.xziqi.cn/gtabtexaom.html

O. 并发与异步
来源：http://hz.tianlin.xyz/gtzaioyseo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqborpeve.html

[O01] 启动一个线程
来源：http://hz.pycfn.com/gtvrcobzib.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hnxiangtu.top/gtnegfdunr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dianchejie.cn/gtbcktfobk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtczdjsuob.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtauxjjqmx.html

Java: new Thread(() -> f()).start()
来源：http://hz.fengsongda.top/gtwjvotggv.html

Go:   go f()
来源：http://hz.yj20258888.top/gtvlcoumru.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gtftofkanx.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtcqtanilz.html

[O02] 使用线程池
来源：http://hz.pengpengdd.cyou/gtcqjllgci.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtxnroynje.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.daria6918.cn/gtolddlvlm.html

JS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtzkykudrs.html

TS:   // worker_threads 线程池
来源：http://hz.chenjidiqi.icu/gtrpnvsear.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydzc1.top/gtxjhrjcox.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yueranfly.top/gtaaegsuas.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daria6918.cn/gtuqukwntr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xylfe.cn/gtsimwyibs.html

[O03] 加锁保护共享数据
来源：http://hz.sxryk.cn/gtbihjlefh.html

Py:   with lock: shared += 1
来源：http://hz.zhoulong.xyz/gtppaxykqf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.kuanghao11.cn/gtohgrdqmu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aizwys.cn/gtcmrlrbet.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtpitsgjjx.html

Java: synchronized (this) { shared++; }
来源：http://hz.guannengcc.top/gtqwxsaghi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtywaiqqxa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jianghu66.top/gtkmebtfat.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gtbyynwqec.html

[O04] 定义异步函数并等待
来源：http://hz.yuanzhike.top/gtofsynzez.html

Py:   async def f():⏎    await g()
来源：http://hz.jiagoushi.top/gtzlqwtbxc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ybcxt.top/gtojyksokr.html

JS:   async function f() { await g(); }
来源：http://hz.guowangkeji.top/gtwlpxejsl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtlkovxopa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.fzhhl.top/gtfeefegvm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jyoumei.cn/gtujjsjjbc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xinyue.icu/gtuvcpnanj.html

C#:   async Task F() { await G(); }
来源：http://hz.zhiwuduotai.top/gtbqcajakv.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuanzx.com/gtkmbfdboo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258888.top/gtcozzhtzb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtkqdvalng.html

JS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtoouwrlzi.html

TS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtuxnqgbhe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jianghu66.top/gtntzqnfae.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhongyouzk.top/gtglvbabhk.html

Ruby: threads.map(&:join)
来源：http://hz.c1oappe.top/gtsiqywqqs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gtzjwhawdp.html

[O06] 使用进程池
来源：http://hz.shangyingyoupin.top/gtqafdbbyf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtuxllxudr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ivvv.top/gtbcbbgipb.html

JS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gterypzyrh.html

TS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtvdntypga.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtypvmgqpk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenzaomai.com/gtjbdchmgk.html

Ruby: // fork 块
来源：http://hz.cheryme.top/gtzmripklk.html


<!-- 参考信息 -->