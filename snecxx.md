代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.iojbl.cn/gtgzkjxlic.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangkeji.top/gtpbqklsuc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daxiang520.top/gtdehpdmmz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ybcxt.top/gtdxaitzbq.html

[L03] 设置自定义请求头
来源：http://hz.sufxvd.cn/gtiddhzdqr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shzxlz.cn/gtcgdcthzy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigufen.top/gtvcqrvcuc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtoimpqwbu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtunjyacpw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtrklsckeh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258.top/gtsmpeeeza.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guannengcc.top/gtzguaocmj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gttrhgdeyc.html

[L04] 设置超时
来源：http://hz.chenlongwang.top/gtumqktvpa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.redwolf501.top/gttgoedacr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yvedp.cn/gtuhfqtrcr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtviksduau.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtgtghxbyx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.feifeiyinyue.top/gtsdvtmsxp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.iojbl.cn/gtdutupqlj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtgtdtsnrw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gotoacloud.top/gttlyddmxd.html

[L05] 上传文件（multipart）
来源：http://hz.zhoulong.xyz/gtobqmxioh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtbzsmwblm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tian-w.cn/gtxltrkskf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtuasbbeqz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gttblwhcex.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxinkj.top/gtzewrxyfx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtklncpmop.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtwxpiboiz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtfqiioxcf.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtkyuosnhi.html

Py:   resp.json()
来源：http://hz.haohaochexian.top/gtgcnrukci.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gtibheeshd.html

JS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gttyawzyrv.html

TS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtflxvqygv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gtrmzhbhxw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.mhx1999.top/gtmihayctv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yongpay.top/gtlswnctpk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtrohbyeab.html

[L07] 处理 HTTP 状态码
来源：http://hz.xziqi.cn/gtpstpfypf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jlsjyb.cn/gtstqombgn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtlwhcmmqt.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtekhyljjt.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtvtojrikh.html

Java: resp.statusCode()
来源：http://hz.tanke756.top/gtgjyonwta.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gtmwzqzhrn.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gtrquilxcz.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtcnmdehiv.html

[L08] 并发请求多个地址
来源：http://hz.cqqwz.cn/gtkflpeblq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.kuanghao11.cn/gtkgbtulcy.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnxiangtu.top/gteriaqvuv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtjamupzsj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtvwaaivdl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ppjwa.cn/gthtobexyf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gttadacgpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangtech.top/gtwppkzmwh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtgmjqobzs.html

================================================================================
来源：http://hz.gogol.net.cn/gtmjyzkyje.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258888.top/gtxguhduyx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtbobzwmxp.html

[M01] 读取命令行参数
来源：http://hz.chenjidiqi.icu/gtuehyguxr.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtzjsfizcy.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtqtbvnwnr.html

JS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gthudkvgoh.html

TS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtxzlgxpap.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtjvgxwfhl.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtzkxtgvqf.html

Ruby: ARGV
来源：http://hz.cdnleiting.top/gtizqnsplx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtsykzjoew.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtnkoffgee.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtibdtobhh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtatsjftqa.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtcfqqehhl.html

TS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtahfipfjq.html

Java: System.getenv("HOME")
来源：http://hz.ehwqpu.com/gtnrppjrae.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gttfvxumlf.html

Ruby: ENV["HOME"]
来源：http://hz.xinyue.icu/gtnrodjfpc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.c1oappe.top/gtfqtozfit.html

[M03] 执行外部命令
来源：http://hz.sysykeji.top/gtenldwjrk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtpngcdqxd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuanzhike.top/gtxffjiseo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtbddosmnr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtblniuaen.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtpztzwbbn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtdgnvucue.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuetiantiany.cn/gtufsdquqa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daxiang520.top/gtipgyeglq.html

[M04] 获取当前工作目录
来源：http://hz.yonumen.top/gthbrqmrer.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtqmkwhnpz.html

PHP:  getcwd();
来源：http://hz.hywenlv.cn/gtrddtduat.html

JS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtjctlxxdt.html

TS:   process.cwd()
来源：http://hz.chenzaomai.com/gtiiqwkzlw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.birdmap.top/gtanuauohw.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtkfvxqamk.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtevsqdabm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtqdcxrpku.html

[M05] 设置退出码
来源：http://hz.zhengqikj.top/gtlbaiukgp.html

Py:   sys.exit(1)
来源：http://hz.zhixingplan.top/gtyuwtylns.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtyylewoxn.html

JS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtweavtifz.html

TS:   process.exit(1)
来源：http://hz.hammf.cn/gtpcdfwhgm.html

Java: System.exit(1)
来源：http://hz.tanke756.top/gtaogkxqhm.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtubwjjxif.html

Ruby: exit 1
来源：http://hz.sysykeji.top/gtdwwaerog.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hysaishi.cn/gtvmozqvdv.html

[M06] 向标准错误输出
来源：http://hz.ydjk.org.cn/gtpaubjtbo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtnouqehhf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhaomingkeji.xyz/gtuyornxgm.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtqmxpcxpa.html

TS:   console.error("err")
来源：http://hz.xuanzx.com/gtxaaajzok.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangtech.top/gtyzyyizig.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtttdcccnx.html

Ruby: warn "err"
来源：http://hz.daxiang520.top/gtxafllatd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.kuanghao11.cn/gtzwiiytrr.html

[M07] 判断是否为主入口
来源：http://hz.chenlongwang.top/gtqqphkxvq.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxuanxn.top/gtlwlzanku.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.9152youxi.cn/gtndkopgwb.html

JS:   require.main === module
来源：http://hz.cashguo.top/gtanslkbkk.html

TS:   require.main === module
来源：http://hz.aizwys.cn/gtrcyxomnp.html

Java: public static void main(String[] args)
来源：http://hz.andypj.xyz/gtteplzwxz.html

Go:   func main()
来源：http://hz.smart0.xyz/gthhtzuwfc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtvazwfjzj.html

C#:   static void Main(string[] args)
来源：http://hz.ivvv.top/gtmaiipnhg.html

[M08] 获取系统与运行时信息
来源：http://hz.andypj.xyz/gtudsevkhy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.andypj.xyz/gtlnucxcyr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cdnleiting.top/gtycgxqhkh.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtdtgclsgm.html

TS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtljvuiqkr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtleadotuj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.iojbl.cn/gtvrfawnew.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gtilqezsbn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258.top/gtfiruujdk.html

================================================================================
来源：http://hz.snrcjt.cn/gtfxiafdln.html

N. 数据结构与算法
来源：http://hz.shanyushiyangkeji.top/gtvwfntzap.html

================================================================================
来源：http://hz.iojbl.cn/gtgshcance.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258888.top/gtqfatprap.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtboqyfqvz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuxming.cn/gtlvqjjoap.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtbgmcxckb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gtzakjnnjc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gthhwmldel.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tianlin.xyz/gtmhqcnqjj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ybcxt.top/gtnziimtqa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gtsnqxkuwz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dianchejie.cn/gtbjgddbsu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtcputeadx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gzhubu.top/gtyhcfezrl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gthaoieuqx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtbqjodypu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtvubxjuro.html

Go:   slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtrdtwknaw.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtnqnkpdyx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tanke756.top/gtewmcoqpt.html

[N03] 快速排序（分治示例）
来源：http://hz.yanxiufei.cn/gtxzxumbge.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtzqvjwcnh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daxiang520.top/gtphbzisov.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtsxohdjuo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtjiotirnu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtmkdnafgv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.andypj.xyz/gtkrakxobc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhixingplan.top/gtxsxqtvpf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtwbzumaro.html

[N04] 斐波那契数列
来源：http://hz.jinqigufen.top/gtgizuljoi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gtptcapawp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhengqikj.top/gtsopldyzj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtyjttzvtg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gthlnxgect.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtczlelyyv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgfzy.top/gtzjdwxbhj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtesurmbhb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jlsjyb.cn/gtwsfoytha.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtqpaxramh.html

Py:   math.gcd(a, b)
来源：http://hz.jqgufenzy.top/gtanybjkpj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnqzz.top/gtafxhtjmn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtgzfcgzag.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtahvbocit.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pengpengdd.cyou/gtwhormwru.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jiagoushi.top/gtlrfdnjsl.html

Ruby: a.gcd(b)
来源：http://hz.snrcjt.cn/gtilbicpgb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xziqi.cn/gtherorjsj.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gttvcldvet.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtgkikojie.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gtlrfyouvf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtblnzxuqk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtftlnlbre.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cucudq.cn/gtquzxoxvl.html

Go:   // 双指针从两端比较
来源：http://hz.daria6918.cn/gtyyylpakn.html

Ruby: s == s.reverse
来源：http://hz.zhiwuduotai.top/gthkpplizg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtexphwbqn.html

[N07] 两数之和（返回下标）
来源：http://hz.shuidangran.top/gtkdvnnwxn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhengqikj.top/gtlcusatsu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.iojbl.cn/gtjshimucc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hywenlv.cn/gtpkuwgalx.html

TS:   // 手写 Map<string, number>
来源：http://hz.cashguo.top/gtcqfcyxhj.html

Java: // 手写 HashMap
来源：http://hz.shangyingyoupin.top/gtopjrdynk.html

Go:   // 手写 map[int]int
来源：http://hz.gogol.net.cn/gtxxjcalkj.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtcfsrtlav.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pycfn.com/gtazlzltgv.html

[N08] 生成全排列
来源：http://hz.kuanghao11.cn/gtzzncsniq.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtymkzeouu.html

PHP:  // 手写递归交换
来源：http://hz.yuanzhike.top/gttlwfeuqb.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtrptdnila.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtqziqvuxj.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gteppanple.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtublaurvt.html

Ruby: arr.permutation.to_a
来源：http://hz.chenzaomai.com/gtlxjgkutw.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtybbhacjl.html

[N09] 栈与队列
来源：http://hz.wangdashe.top/gtrtkmjevd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cashguo.top/gtjutqjkvk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daxiang520.top/gtegqmnuhy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtdxffkula.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtfdqtkfyg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pengpengdd.cyou/gtxhimxkix.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jyoumei.cn/gtirwxsnvr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gtkgyzlxoc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.bjfxy.top/gtdxsjoefo.html

[N10] 链表节点定义
来源：http://hz.sxryk.cn/gtryvdeful.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtzlvfqxes.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.feifeiyinyue.top/gthyklwnas.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gtjdfuifkh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinyuanbaomall.cn/gtcrohttey.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtkneemlnc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtpwujseim.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinyuanbaomall.cn/gtcwvmueyd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yongpay.top/gtihsmdtws.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtnmazoogo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jianghu66.top/gtibrblwpu.html

PHP:  // 手写递归函数
来源：http://hz.jiagoushi.top/gtvxgbpayg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtkbiukwaa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtvavxnlak.html

Java: // 手写递归
来源：http://hz.wangdashe.top/gtbfpcksqy.html

Go:   // 手写递归
来源：http://hz.zhengqikj.top/gthdbvmhea.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xingfuxueyuan.xyz/gtnwhcgdqx.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gtzqbjxpds.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangtech.top/gtlavtzgqp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.meibo888.top/gtcwhybuir.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnxiangtu.top/gtczznkozg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.mhx1999.top/gtqufxrhnk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtltaccksm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtxidpqghk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhengqikj.top/gtfgjrbddy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daria6918.cn/gtsvpzqezp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtbsartgta.html

================================================================================
来源：http://hz.hammf.cn/gtscetokyc.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtbjvtrlkj.html

================================================================================
来源：http://hz.shuidangran.top/gtzvpzgccp.html

[O01] 启动一个线程
来源：http://hz.zhongyouzk.top/gtaxlqlamg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hywenlv.cn/gtgznngcdt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenjidiqi.icu/gtrqcmhnoy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtkanbkcqp.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtbqtrnpgx.html

Java: new Thread(() -> f()).start()
来源：http://hz.sweek.top/gtztfakeqv.html

Go:   go f()
来源：http://hz.0kj1m.cn/gtuhvndbva.html

Ruby: Thread.new { f }
来源：http://hz.jlsjyb.cn/gtwimubuts.html

C#:   Task.Run(() => F());
来源：http://hz.cheryme.top/gttzkdiphj.html

[O02] 使用线程池
来源：http://hz.yanxiufei.cn/gtzhofskaj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.52xcode.cn/gthgdcvyii.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.52xcode.cn/gtnwflnzja.html

JS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtvlptowve.html

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtlajdrwqu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gtdzdrlyla.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gtejdiovki.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.svipenyu.cn/gtxeuiaotl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinghuilouyu.cn/gtxmqkrwbv.html

[O03] 加锁保护共享数据
来源：http://hz.nwbrower.top/gtrlkgxhdq.html

Py:   with lock: shared += 1
来源：http://hz.wangshuangyany.cn/gtrapfnacd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xylfe.cn/gtzadqvkeo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gaohongyu789.top/gtlttifhef.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtzjlmljzu.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gtsczuthiu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.snrcjt.cn/gtpqucnhgn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.quarkkingdee.top/gteondrnhz.html

C#:   lock (gate) { shared++; }
来源：http://hz.gzhubu.top/gtgaollmtb.html

[O04] 定义异步函数并等待
来源：http://hz.jiagoushi.top/gtxmwrahgu.html

Py:   async def f():⏎    await g()
来源：http://hz.zhaomingkeji.xyz/gtdgwybgyy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnqzz.top/gtpuqyszxz.html

JS:   async function f() { await g(); }
来源：http://hz.xinyue.icu/gtxjitmizf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtopucvahn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.dashuyun.cn/gttyhkhnba.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.kuanghao11.cn/gtvymtyoms.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.meibo888.top/gtwapagtnk.html

C#:   async Task F() { await G(); }
来源：http://hz.guowangkeji.top/gtdoytwnfw.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhiwuduotai.top/gtwhxsyumq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shzxlz.cn/gtfqkokrhu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenzaomai.com/gtrqilwgek.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gteffkzfzn.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gteudshclt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jyoumei.cn/gtpkbpoofq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pycfn.com/gttcanxyip.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtfrwfziwh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gotoacloud.top/gtdvshkxnq.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtmqdfceed.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jiagoushi.top/gttrcfgdut.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ppjwa.cn/gtyznuyomv.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtzumogsqz.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtfljvjftj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtqyzntbdy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenjidiqi.icu/gtoolpdwsl.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gtrdlsvsgt.html


<!-- 参考信息 -->