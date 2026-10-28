代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gthxmvmesl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.kuanghao11.cn/gtnzrlqaym.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.kuanghao11.cn/gtljycdfxy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yongpay.top/gtnyjnlhwk.html

[L03] 设置自定义请求头
来源：http://hz.jinghuilouyu.cn/gtxyxckgcg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtedwfokpj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fzhhl.top/gtcsifwuxr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtwfoaxmaa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtpmiyhfih.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yueranfly.top/gtevoatzao.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtgjcpowjz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gtdhhhmurz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtbiyhxtxy.html

[L04] 设置超时
来源：http://hz.cqqwz.cn/gteuheedqu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtbcmypkrh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtpnrokwnw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtgslkdvxr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtwwbgsuod.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtmaorjzpv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jqgufenzy.top/gthlbfrgqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ehwqpu.com/gtacczmrip.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ivvv.top/gtnjowmogl.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtazabnqgv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtcdiiwsed.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtyyyrqlex.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigufen.top/gtgffjmqpn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gthajhveso.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtmrkdkial.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj202588.top/gteuqestzc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zycfv.cn/gtfnjsjnll.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gttuotmkix.html

[L06] 解析响应为 JSON
来源：http://hz.52xcode.cn/gtykbdwybc.html

Py:   resp.json()
来源：http://hz.havefunace.top/gtpwhuopzv.html

PHP:  json_decode($body, true);
来源：http://hz.sufxvd.cn/gtjsosazez.html

JS:   await resp.json()
来源：http://hz.gzhubu.top/gttzqhquvz.html

TS:   await resp.json()
来源：http://hz.yj20258.top/gtlxalpgik.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtwafwlyux.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xylfe.cn/gtdcsavofv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hammf.cn/gtlzyrvkwp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.smart0.xyz/gtzekpmojc.html

[L07] 处理 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtymvvpcyg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtkdkpkthj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tian-w.cn/gtidgjebwe.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gthwrbwqdy.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtltlanukg.html

Java: resp.statusCode()
来源：http://hz.yangfankeji.com/gtutuqaxif.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtqjqnbjqt.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtierymuyv.html

C#:   (int)resp.StatusCode
来源：http://hz.yj202588.top/gtypxvtgex.html

[L08] 并发请求多个地址
来源：http://hz.svipenyu.cn/gtrswqbfmx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tanke756.top/gtqfldjkjd.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhiwuduotai.top/gtisslrkbf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtqlpmxuof.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtqptduwxw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.bjfxy.top/gterikdugr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jianghu66.top/gttwqeusxm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuanzhike.top/gtrpluyora.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtcvctbnqp.html

================================================================================
来源：http://hz.daria6918.cn/gtqdaatsnd.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtfkdeedcg.html

================================================================================
来源：http://hz.jyoumei.cn/gtjfjuvbqo.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtnaxhoadd.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtxvyycden.html

PHP:  $argv;  $argc;
来源：http://hz.jinghuilouyu.cn/gtthpwydba.html

JS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gthdjwttub.html

TS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtrqjffrdf.html

Java: args 数组（main 方法参数）
来源：http://hz.zhixingplan.top/gtvkgnomol.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtkbnmxtky.html

Ruby: ARGV
来源：http://hz.jqgfzy.top/gtovwafomg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.vqdsnc.cn/gtfwoifsfq.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gtdufbjbsx.html

Py:   os.environ.get("HOME")
来源：http://hz.xylfe.cn/gtfcvgnpgo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gotoacloud.top/gtxsngmljo.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtjvmkwdxh.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtovnnkkib.html

Java: System.getenv("HOME")
来源：http://hz.pengpengdd.cyou/gtcybgkmfl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cashguo.top/gtgmkbhyie.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtvhsxlcma.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtfhtxsazd.html

[M03] 执行外部命令
来源：http://hz.ywan-chungtsiang.top/gtgofeagvc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinghuilouyu.cn/gtvzszdwng.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.mhx1999.top/gtrbbwqaps.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtoqgyrhia.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtrdzmyppg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigufen.top/gtrmajcifr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxuanxn.top/gtxksbmttp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gttiiruwia.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zdqjudy.top/gtjpankank.html

[M04] 获取当前工作目录
来源：http://hz.kuanghao11.cn/gthlfwbqqz.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangtech.top/gtjmgdloab.html

PHP:  getcwd();
来源：http://hz.feifeiyinyue.top/gtrquyazlh.html

JS:   process.cwd()
来源：http://hz.fzhhl.top/gtqcptnavm.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtxoukzrmg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.meibo888.top/gtrcxentos.html

Go:   os.Getwd()
来源：http://hz.svipenyu.cn/gttftvqtkg.html

Ruby: Dir.pwd
来源：http://hz.jqgufenzy.top/gtgodimxsj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aibaodan.cn/gtsgvftvgc.html

[M05] 设置退出码
来源：http://hz.yvedp.cn/gtkkmfypxk.html

Py:   sys.exit(1)
来源：http://hz.vqdsnc.cn/gtlsnmvvnw.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gtgsyntawj.html

JS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtbdtkwwgq.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gteibplwbv.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gtadbmitpa.html

Go:   os.Exit(1)
来源：http://hz.nanxinkj.top/gtxftsgmaj.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gthtzdgaqo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangtech.top/gtcsftxljj.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtlvyltmvi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gtnfoimnaq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guowangkeji.top/gthuwoples.html

JS:   console.error("err")
来源：http://hz.nanxinkj.top/gtqoeczlao.html

TS:   console.error("err")
来源：http://hz.cqqwz.cn/gtdadqozjj.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gtsjxavgwl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.c1oappe.top/gtikgehxdi.html

Ruby: warn "err"
来源：http://hz.shangyingyoupin.top/gtuwajdppw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sufxvd.cn/gtluxnazoc.html

[M07] 判断是否为主入口
来源：http://hz.316326.xyz/gtgudlfdmw.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtkfudewuj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jiagoushi.top/gtfbhagdcv.html

JS:   require.main === module
来源：http://hz.guowangkeji.top/gtklpiivjk.html

TS:   require.main === module
来源：http://hz.gogol.net.cn/gtgzoicfoq.html

Java: public static void main(String[] args)
来源：http://hz.xuanzx.com/gtcdhrorpo.html

Go:   func main()
来源：http://hz.redwolf501.top/gtssnlytbe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.9152youxi.cn/gtbuvdquap.html

C#:   static void Main(string[] args)
来源：http://hz.cdnleiting.top/gtucwtumvf.html

[M08] 获取系统与运行时信息
来源：http://hz.pycfn.com/gtgqnegdwa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gtqwthetdt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtilmybfwm.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtlfsxapjs.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtxapyzyvb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtsqdzerhj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gthewucxbm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gtzyzybvcd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nwbrower.top/gthxfmxube.html

================================================================================
来源：http://hz.jinqigfzy.top/gtyddzswty.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtzrtfrcgb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrooowcba.html

[N01] 二分查找（有序数组）
来源：http://hz.wangdashe.top/gtfnvsgsmh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtnxikxsgq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtwiekelep.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gthfftwqlg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtosbasjrs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daria6918.cn/gtbvthleii.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtbmldjyed.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangdashe.top/gtwjagvmyo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sxryk.cn/gtsxovrkam.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gtsvddgqwi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gthprdkwrp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtwgymdzlc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtpbpqzlti.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtgbjkcwax.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtptlfgtqs.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtawekbngs.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtnywvlvuy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gzhubu.top/gtleootefj.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtexxyykrf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtqmwroidm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gtsdfffjqo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtmfljnxad.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtjgpyfjaf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.snrcjt.cn/gtiyiikgzt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhixingplan.top/gtflbjqvab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zdqjudy.top/gtrvsxpjlc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hammf.cn/gtmfliplen.html

[N04] 斐波那契数列
来源：http://hz.daria6918.cn/gtkkcpjish.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gteudsiruv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.c1oappe.top/gtmnqhrewa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtooofahom.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtgvomrpal.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtfhmyeefr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtyttjpsxa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gtblpeckrg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jyoumei.cn/gtlqrvzxrx.html

[N05] 最大公约数
来源：http://hz.haohaochexian.top/gtbgvdhpav.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtnlotdtdj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.redwolf501.top/gtxyabjkup.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gttljfwwyk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtshgfqnqr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtdglxfbnw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ywan-chungtsiang.top/gtglamowhz.html

Ruby: a.gcd(b)
来源：http://hz.jqgfzy.top/gttrnjckou.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.havefunace.top/gtyobmgauu.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gtwbqlvfxy.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtwnsdkyxd.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258.top/gtgsmuyuhu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtrjltfdvb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtjqmhokgm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yongpay.top/gtsllcszmf.html

Go:   // 双指针从两端比较
来源：http://hz.birdmap.top/gtpvuxgfno.html

Ruby: s == s.reverse
来源：http://hz.hysaishi.cn/gtyxipbkid.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtidcbklab.html

[N07] 两数之和（返回下标）
来源：http://hz.zhijiandao.cn/gtsanhlchr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tian-w.cn/gtqobxfoyt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gttlvawueu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shangyingyoupin.top/gtznjewxua.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gteblboqcd.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtsxgyoxrj.html

Go:   // 手写 map[int]int
来源：http://hz.gotoacloud.top/gtabasbfmk.html

Ruby: // 手写 Hash
来源：http://hz.chenlongwang.top/gtphfsyilo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuanzhike.top/gtfxrekdis.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gtwfyhrvkd.html

Py:   itertools.permutations(arr)
来源：http://hz.ehwqpu.com/gtazzlmesz.html

PHP:  // 手写递归交换
来源：http://hz.chenjidiqi.icu/gtxobzbpfm.html

JS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtpvwflijq.html

TS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtvpjrhueh.html

Java: // 手写回溯递归
来源：http://hz.0kj1m.cn/gtjzxtausi.html

Go:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtbpkxuxkh.html

Ruby: arr.permutation.to_a
来源：http://hz.316326.xyz/gtvlhqphak.html

C#:   // 手写回溯递归
来源：http://hz.tanke756.top/gttspbjqaw.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gttoraujbm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gzhubu.top/gtkztmdhop.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigfzy.top/gtdmnickgt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenlongwang.top/gtigbyoibe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtxfhfxrxr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gtlgkdclox.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nanxuanxn.top/gtguhkhmek.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daria6918.cn/gtrzwkhzvb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxinkj.top/gtfkkielfm.html

[N10] 链表节点定义
来源：http://hz.hywenlv.cn/gtrwmrqvuk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jyoumei.cn/gtnzdvsvgc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.kuanghao11.cn/gteeqwhfti.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gtpvqdhnpo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xingfuxueyuan.xyz/gtkavigjrr.html

Java: class Node { int v; Node next; }
来源：http://hz.hywenlv.cn/gtbgwmxhke.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangkeji.top/gtrplzuens.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ehwqpu.com/gtzjfscvpw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.birdmap.top/gtvhhltfpp.html

[N11] 二叉树中序遍历
来源：http://hz.pycfn.com/gtqrlzbklf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhijiandao.cn/gtbmuckkrh.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtgehscurm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtxmzptdrb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtukrouxvm.html

Java: // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtcalzuzjz.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtkquxqmgb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinghuilouyu.cn/gtnjxmkxec.html

C#:   // 手写递归
来源：http://hz.shzxlz.cn/gtcanbvvmt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cheryme.top/gtvbvgzeyw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.9152youxi.cn/gtiqekrunf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gtjxmkwcej.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtewvpqbeg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtfqriosun.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daxiang520.top/gtmrtftelw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj202588.top/gthmfukran.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhixingplan.top/gtlcksfqbi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtxreghvmp.html

================================================================================
来源：http://hz.chenzaomai.com/gtlewcpxlr.html

O. 并发与异步
来源：http://hz.guannengcc.top/gtvhtngvuz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmjerncmi.html

[O01] 启动一个线程
来源：http://hz.wangdashe.top/gtlavjnrsp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tanke756.top/gtpwmxceim.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sweek.top/gtblqdngkn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenlongwang.top/gtlgyrkboe.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtozprjysg.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gtkcmgnnln.html

Go:   go f()
来源：http://hz.mhx1999.top/gtjvdricvu.html

Ruby: Thread.new { f }
来源：http://hz.yj20258.top/gtauvnzfll.html

C#:   Task.Run(() => F());
来源：http://hz.yongpay.top/gtycgisljf.html

[O02] 使用线程池
来源：http://hz.chenzaomai.com/gtyumkbahc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtubjzqgtv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtiaqnbesq.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gthlraxkoe.html

TS:   // worker_threads 线程池
来源：http://hz.xinyue.icu/gthoixbipu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cqqwz.cn/gteyfgyivo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hfpthk.cn/gtgttdbywb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hfpthk.cn/gtltllthpl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jyoumei.cn/gtofnpmoeo.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtkwvdhcmm.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gtujdqcehx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnqzz.top/gtucufncnz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtvypipkql.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtuekxcqya.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gtwstqnqds.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.meibo888.top/gtlmlpaqmh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhiwuduotai.top/gtuuskborm.html

C#:   lock (gate) { shared++; }
来源：http://hz.hongshengwenyu.top/gtlslbsxcd.html

[O04] 定义异步函数并等待
来源：http://hz.wangdashe.top/gtzhxkmntf.html

Py:   async def f():⏎    await g()
来源：http://hz.chenlongwang.top/gtyqzekwoj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtconpfmlm.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtltzbjxsh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtizlaspvc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jyoumei.cn/gtefyifzbn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gtlyrtxkaw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sweek.top/gtihycrxcs.html

C#:   async Task F() { await G(); }
来源：http://hz.jlsjyb.cn/gtdcxcsdyz.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtjcxgrkqj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cucudq.cn/gtusrdqche.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtkdgjdvvs.html

JS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtbcsefwhd.html

TS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtaernvftj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jyoumei.cn/gtjipeyucv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtpcnhggvp.html

Ruby: threads.map(&:join)
来源：http://hz.hnqzz.top/gtqdilwltw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtboqccjvg.html

[O06] 使用进程池
来源：http://hz.cashguo.top/gtugbrijph.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtmcxekhou.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtqrhsiqmi.html

JS:   // child_process / cluster 模块
来源：http://hz.hammf.cn/gtfendkroi.html

TS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtnenpzrdz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnxiangtu.top/gtnjgemukt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gotoacloud.top/gtgmcwlinp.html

Ruby: // fork 块
来源：http://hz.svipenyu.cn/gtqyyahfyq.html


<!-- 参考信息 -->