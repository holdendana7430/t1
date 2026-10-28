代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pengpengdd.cyou/gtmontqsbw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinyuanbaomall.cn/gtimuttjmb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jlsjyb.cn/gtkwsldowc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangshuangyany.cn/gtytfotnuk.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtboxezzyk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jyoumei.cn/gtrkfdanur.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtgapjttpw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtifjozscj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtojrmewnv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtzqlcqexq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtszorxtid.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gtqsftsjjd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gtvfxkhpoi.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gtrwckarrv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtokoohifx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gtzyxdubzo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtlupanfjh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtxrpnifdp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuanzx.com/gtjbuhdsze.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aizwys.cn/gtvnlctmhr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gthdaftvxg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yonumen.top/gtkewkwfwi.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtpgdxiubu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxuanxn.top/gtjrcmoktc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuanzx.com/gtxniuhxdx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtgcpchzhl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtwkqkrfji.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.52xcode.cn/gtwolpyvxi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtfgsiwovn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sxryk.cn/gtngktoorv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhengqikj.top/gtxadwucgd.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtawftbiqm.html

Py:   resp.json()
来源：http://hz.snrcjt.cn/gtdywlqdfb.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtijeccsrb.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtsmakcfdb.html

TS:   await resp.json()
来源：http://hz.hnxiangtu.top/gttvkkfvhu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gthveelymd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gthoffohsa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.birdmap.top/gtqrtmwcnn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guowangkeji.top/gtxygnfupv.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtoexeddqm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gtqwoxpyrc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gtpwjxafkv.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtncqydggo.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtzprovwww.html

Java: resp.statusCode()
来源：http://hz.meibo888.top/gtthidmwgu.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtxnevlclu.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtafsrwrcj.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gthlpqyvzu.html

[L08] 并发请求多个地址
来源：http://hz.gogol.net.cn/gttjbgcbbg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtkrrwmvqw.html

PHP:  curl_multi_init() 系列
来源：http://hz.jyoumei.cn/gteddjtdyl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtdyigonog.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtibvzisef.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.iojbl.cn/gtqrjdafwf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sufxvd.cn/gtthqtxlyc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtkldrodkn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhoulong.xyz/gtscsjxhob.html

================================================================================
来源：http://hz.zdqjudy.top/gtukejnrtl.html

M. 命令行 / 进程 / 环境
来源：http://hz.tanke756.top/gttcfmhvkz.html

================================================================================
来源：http://hz.haohaochexian.top/gtjcuzhtqo.html

[M01] 读取命令行参数
来源：http://hz.tanke756.top/gtgdslvevs.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtlgklrgsa.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtbxxohatj.html

JS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtvigplnic.html

TS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtremjcaei.html

Java: args 数组（main 方法参数）
来源：http://hz.feifeiyinyue.top/gtdvwftyox.html

Go:   os.Args[1:]
来源：http://hz.yanxiufei.cn/gtvrphvkgd.html

Ruby: ARGV
来源：http://hz.wangdashe.top/gthdcxbzop.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgfzy.top/gttlhcbtsk.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gtfltauklz.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258888.top/gtgblsvrym.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gthsqzcmtx.html

JS:   process.env.HOME
来源：http://hz.yonumen.top/gtnzwppsab.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtubcuedxi.html

Java: System.getenv("HOME")
来源：http://hz.jqgfzy.top/gtubxfagfm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtdcxxobpz.html

Ruby: ENV["HOME"]
来源：http://hz.c1oappe.top/gtrgneadgg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydzc1.top/gtbgxynlaw.html

[M03] 执行外部命令
来源：http://hz.meibo888.top/gtenofnebz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtgcposvzl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtbjgxrblj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtbfckusiv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtqknrvnak.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangdashe.top/gtshjtiawo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gtvfurhbfh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gtcdmreafc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtxtvoiene.html

[M04] 获取当前工作目录
来源：http://hz.ppjwa.cn/gtoxvplkrk.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtjhojbpor.html

PHP:  getcwd();
来源：http://hz.ybcxt.top/gtzbhwtymv.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtkuynxghw.html

TS:   process.cwd()
来源：http://hz.dashuyun.cn/gtvutzrlnb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhiwuduotai.top/gtlzywfbke.html

Go:   os.Getwd()
来源：http://hz.daria6918.cn/gtpyecyhau.html

Ruby: Dir.pwd
来源：http://hz.sysykeji.top/gtvtwozriy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gtuznppckx.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtxahjwxwj.html

Py:   sys.exit(1)
来源：http://hz.fzhhl.top/gtmlmmjxmp.html

PHP:  exit(1);
来源：http://hz.tanke756.top/gtrvgegjxh.html

JS:   process.exit(1)
来源：http://hz.52xcode.cn/gtzqnivuog.html

TS:   process.exit(1)
来源：http://hz.zdqjudy.top/gtrgjsybsn.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtepqzvoix.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtuegubmug.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtheivlese.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenjidiqi.icu/gtlguhvuxu.html

[M06] 向标准错误输出
来源：http://hz.ivvv.top/gtijavbytv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtnmfjvpsc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xingfuxueyuan.xyz/gtifplmxwi.html

JS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtfwgmvozr.html

TS:   console.error("err")
来源：http://hz.yueranfly.top/gtwkqwxtpt.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gtblhwwoae.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gtmtcoxltz.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gtrcuyefcu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhengqikj.top/gtcmwjzlbu.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtxgdlubfy.html

Py:   if __name__ == "__main__":
来源：http://hz.vqdsnc.cn/gtgiszagws.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hysaishi.cn/gtwrmkikjg.html

JS:   require.main === module
来源：http://hz.hnxiangtu.top/gtmtwpgpdu.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtxqumauov.html

Java: public static void main(String[] args)
来源：http://hz.yvedp.cn/gtppyxbtwl.html

Go:   func main()
来源：http://hz.zhoulong.xyz/gtoxqvputn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtgloqerrc.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtphpcxeof.html

[M08] 获取系统与运行时信息
来源：http://hz.ydzc1.top/gtbntviegk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gtzxhksrhg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.quarkkingdee.top/gtlzwlqhem.html

JS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtohudjcog.html

TS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtoxnpvpww.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.meibo888.top/gtkkztjukm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigfzy.top/gtciopdxdw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gtwxjrzsar.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtgwcxirtl.html

================================================================================
来源：http://hz.yj202588.top/gtbcquoskv.html

N. 数据结构与算法
来源：http://hz.haohaochexian.top/gtevtqequg.html

================================================================================
来源：http://hz.jianghu66.top/gtyozmnpeq.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtwavfakku.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtkrtlocgk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jiagoushi.top/gtqvqiyghl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtqymojbht.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtwbhskgpd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtankszzym.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gttgipskiz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cdnleiting.top/gtqqysfwzc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtohkzkadm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hywenlv.cn/gtwdmcrbuu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtbllsofzh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtqfwyptmi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtcgznjini.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtywdbpawx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.svipenyu.cn/gtncwjnwfc.html

Go:   slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gtasdsrops.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtqnrmtwrm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtbkocetoa.html

[N03] 快速排序（分治示例）
来源：http://hz.birdmap.top/gtvwdrbgnm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gaohongyu789.top/gtatbwbsdp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gtzqllxhac.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtzovzzncq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yangfankeji.com/gtjbualesk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gtnacflvzt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtjzcfqcxc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jianghu66.top/gttrtwzhkv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinyuanbaomall.cn/gtiulwjtca.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtrdpodrrq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtnhfpyulz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhongyouzk.top/gtwnwqjqje.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.316326.xyz/gtzrpjdtig.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydzc1.top/gtwcsdxtdl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtndbjqotw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jlsjyb.cn/gtsrcxukoe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtvpxnjfgi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhoulong.xyz/gtcezkwzgw.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gtsrczhcop.html

Py:   math.gcd(a, b)
来源：http://hz.zhengqikj.top/gtpeleqvju.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj202588.top/gthnwusfvc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gttzmtjrqy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtnbcqsnrf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gthtwfckwj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtzdwddvvo.html

Ruby: a.gcd(b)
来源：http://hz.shangyingyoupin.top/gtshqzibwe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangtech.top/gtkcdbbwsw.html

[N06] 判断回文字符串
来源：http://hz.gotoacloud.top/gtzkibvloo.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtwcmdrtzi.html

PHP:  $s === strrev($s);
来源：http://hz.c1oappe.top/gtsqjdbgsf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtfniozcsr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtikxenflu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dashuyun.cn/gttvbszxgw.html

Go:   // 双指针从两端比较
来源：http://hz.jianghu66.top/gtdpunreii.html

Ruby: s == s.reverse
来源：http://hz.chenzaomai.com/gtcyftvqrp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gthgmdghwy.html

[N07] 两数之和（返回下标）
来源：http://hz.zhengqikj.top/gtbyeosxqi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtaaqsprtv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtovdvimfz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtvrrnrmuy.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtmoefrgax.html

Java: // 手写 HashMap
来源：http://hz.shuidangran.top/gthtdyxwtt.html

Go:   // 手写 map[int]int
来源：http://hz.jyoumei.cn/gtkbbopukx.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtswkftznw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gthaohmadu.html

[N08] 生成全排列
来源：http://hz.ybcxt.top/gtrsxjcaol.html

Py:   itertools.permutations(arr)
来源：http://hz.sysykeji.top/gtjxjzwzqm.html

PHP:  // 手写递归交换
来源：http://hz.hnqzz.top/gtplumamgl.html

JS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtofubxpkf.html

TS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtovsrhwtw.html

Java: // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtkujdwlsf.html

Go:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtjhenupve.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gtizzfgvvd.html

C#:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtjhnelpaw.html

[N09] 栈与队列
来源：http://hz.havefunace.top/gthqnqwuth.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtxctpuzlb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gogol.net.cn/gtvjploznm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zdqjudy.top/gtzcqjmxfj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtnovulgkj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.feifeiyinyue.top/gtvhmeuuhb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xuetiantiany.cn/gterzmdpft.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ydzc1.top/gtaoeoeqaj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj202588.top/gtmnftrudy.html

[N10] 链表节点定义
来源：http://hz.yongpay.top/gtcfaakbnt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinghuilouyu.cn/gtbwwngahp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtostyafoo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gtpczwsltg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtdwkpoczs.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gttkpvpzxo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tanke756.top/gtniaeqkpt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.mhx1999.top/gtykkgktfw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtwekknkfa.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtygytoffl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cashguo.top/gtccfwniqy.html

PHP:  // 手写递归函数
来源：http://hz.feifeiyinyue.top/gtjomhdhri.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtmyzmgdpw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtvxazjkrj.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtnczqykcz.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gttotnvsuy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.smart0.xyz/gtxijviuuu.html

C#:   // 手写递归
来源：http://hz.snrcjt.cn/gtzkojuvli.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.redwolf501.top/gttgccoqqn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gthyletowy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxuanxn.top/gtakzhvdzu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtqqzinoqv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gthchgglcd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gturrbvxlw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.haohaochexian.top/gtivgntyqa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangkeji.top/gtuqfmzeqk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtmjwkklfm.html

================================================================================
来源：http://hz.hammf.cn/gtjqagusvj.html

O. 并发与异步
来源：http://hz.yj202588.top/gtzpnaexje.html

================================================================================
来源：http://hz.cheryme.top/gtgvgzlzkp.html

[O01] 启动一个线程
来源：http://hz.zhoulong.xyz/gtkesxzntk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sufxvd.cn/gtmivbfxcy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhengqikj.top/gtnywtuyme.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shzxlz.cn/gtmxecnbet.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtpnqcgjgr.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuetiantiany.cn/gtywmqkadf.html

Go:   go f()
来源：http://hz.sufxvd.cn/gtqizciqzz.html

Ruby: Thread.new { f }
来源：http://hz.xuetiantiany.cn/gtmclfgzev.html

C#:   Task.Run(() => F());
来源：http://hz.fzhhl.top/gtngjcdmwk.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gtoyqteiqk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gtjdkbakqe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.smart0.xyz/gtupnbsulm.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtvvxqqgmn.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtbjmxowgo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinghuilouyu.cn/gtbgmmoqci.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtwtzdbrgo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gtmobinadp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxuanxn.top/gtfyzwncdz.html

[O03] 加锁保护共享数据
来源：http://hz.smart0.xyz/gtftacewyl.html

Py:   with lock: shared += 1
来源：http://hz.birdmap.top/gtfxbvxepm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hywenlv.cn/gtqsszmsiq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shangyingyoupin.top/gtwyhuvqmm.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtvcgzxkwx.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhijiandao.cn/gtcrikcjtm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtqhfolilm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fengsongda.top/gtmyvfsheg.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenzaomai.com/gtiujsiclm.html

[O04] 定义异步函数并等待
来源：http://hz.chenjidiqi.icu/gtwqdbicil.html

Py:   async def f():⏎    await g()
来源：http://hz.xinyue.icu/gtevcsibre.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtjxehihbn.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtfowdtaqq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gaohongyu789.top/gtiezcyccs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtcugiaxct.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gteiiyocrh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hfpthk.cn/gtozqitwdw.html

C#:   async Task F() { await G(); }
来源：http://hz.zhongyouzk.top/gtzmhgszsw.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuanzhike.top/gtmvjtsete.html

Py:   asyncio.gather(*tasks)
来源：http://hz.52xcode.cn/gtazkcihxf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hfpthk.cn/gtoqwzvhir.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtbagzvggc.html

TS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gtbofjkpxg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.meibo888.top/gtxvebprby.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtuaiioila.html

Ruby: threads.map(&:join)
来源：http://hz.snrcjt.cn/gtisjbybim.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.redwolf501.top/gtsaazkirh.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtogyiljil.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aibaodan.cn/gtwpqkudhc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.c1oappe.top/gtihrddtrs.html

JS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gtiukkrbce.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gteispxngl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gtcqtcvptl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtmwcvqjhf.html

Ruby: // fork 块
来源：http://hz.gogol.net.cn/gtqawzushu.html


<!-- 参考信息 -->