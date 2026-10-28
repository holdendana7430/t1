代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.9152youxi.cn/gtoxtjtccz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtorgqzftp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtvhftvbeq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtgssfuhvw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gtulkzxtvr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.9152youxi.cn/gtheffbauo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fengsongda.top/gtatuowdys.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtavhmdcrk.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gteaviwhgv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jlsjyb.cn/gtpgeflfrz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gtahgcsrbh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtmngfcgjs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtgygkmysv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cashguo.top/gtjnmuybax.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtosarnkah.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtwlstxerg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guannengcc.top/gtninmetys.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtmbjfrfgh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shangyingyoupin.top/gtylemrrts.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gthtlzhlds.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtsjdxwmzu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtaoimejqs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtphxyennq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sxryk.cn/gtkeuhypbb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangdashe.top/gtricexbbk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xziqi.cn/gtisyduoyn.html

[L05] 上传文件（multipart）
来源：http://hz.sxryk.cn/gtvjfvugsa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xziqi.cn/gthpfkbbvd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hammf.cn/gtxaotvwwv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtnawkbtxg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtglsdxtap.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhaomingkeji.xyz/gtyjddituu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtzuxqwlht.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtfcctsbrm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.feifeiyinyue.top/gtcqpkdkev.html

[L06] 解析响应为 JSON
来源：http://hz.jlsjyb.cn/gtuglwsets.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtliigiuxm.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtokanzfma.html

JS:   await resp.json()
来源：http://hz.tian-w.cn/gtqvkfgoxv.html

TS:   await resp.json()
来源：http://hz.yuanzhike.top/gtyoensrqf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtdgbtgrfn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtbxwvbjld.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtcmdygbna.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuetiantiany.cn/gtaiciqoax.html

[L07] 处理 HTTP 状态码
来源：http://hz.aizwys.cn/gttshhxvyq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj202588.top/gtekljooil.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cashguo.top/gtgzkujlug.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtqxqquxok.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtenyobytq.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtlhdxuioy.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtdzfonkgq.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtxffwmioi.html

C#:   (int)resp.StatusCode
来源：http://hz.cqqwz.cn/gthnzzrvro.html

[L08] 并发请求多个地址
来源：http://hz.kuanghao11.cn/gtemdkfqqi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtdqcjykwc.html

PHP:  curl_multi_init() 系列
来源：http://hz.bjfxy.top/gtbgnjbxqo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtpwstuaot.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtlvgagdfz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtbtxousfr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aizwys.cn/gtasrfuzbc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuetiantiany.cn/gtlixfdzdw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.smart0.xyz/gtmuczfvvy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtliyinlvp.html

M. 命令行 / 进程 / 环境
来源：http://hz.svipenyu.cn/gtxkxkbeye.html

================================================================================
来源：http://hz.52xcode.cn/gtnjdijbhu.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtvfnrnwrf.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gthqgyutqz.html

PHP:  $argv;  $argc;
来源：http://hz.xuanzx.com/gtkflymtcl.html

JS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtjhzmvpzf.html

TS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtqnuruyge.html

Java: args 数组（main 方法参数）
来源：http://hz.52xcode.cn/gtnedcjtfr.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gtifepocau.html

Ruby: ARGV
来源：http://hz.xuetiantiany.cn/gtzylxnabi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtufznhgeb.html

[M02] 读取环境变量
来源：http://hz.redwolf501.top/gtfirihjdr.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtxjttrsci.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtcxymthca.html

JS:   process.env.HOME
来源：http://hz.daxiang520.top/gtitmemtco.html

TS:   process.env.HOME
来源：http://hz.gzhubu.top/gtpzpncxbt.html

Java: System.getenv("HOME")
来源：http://hz.wangdashe.top/gtoeapupds.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.havefunace.top/gtidvtwzgs.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtmhgbsmsn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtovxoozpz.html

[M03] 执行外部命令
来源：http://hz.birdmap.top/gtaonfrtzu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtygcwibbl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtimmimfjh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtvrpyjunl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtooatvvgz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtikvhrbau.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258.top/gtaplhghkx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nwbrower.top/gteermwthu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtqurmzzkb.html

[M04] 获取当前工作目录
来源：http://hz.nanxuanxn.top/gtonoyudce.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gteuhxulli.html

PHP:  getcwd();
来源：http://hz.yuanzhike.top/gtlcaimiew.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtuipbvdun.html

TS:   process.cwd()
来源：http://hz.shzxlz.cn/gtgcwgpblz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtvotadkfn.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gttakxhmbw.html

Ruby: Dir.pwd
来源：http://hz.ydjk.org.cn/gtitdwamgf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gogol.net.cn/gtmsocrllm.html

[M05] 设置退出码
来源：http://hz.feifeiyinyue.top/gthogndgdi.html

Py:   sys.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtgqwuvfnj.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtjxzonprw.html

JS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtoaoifgeq.html

TS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtbejqlydu.html

Java: System.exit(1)
来源：http://hz.daria6918.cn/gtydsqcsym.html

Go:   os.Exit(1)
来源：http://hz.yueranfly.top/gtqzyfuqgz.html

Ruby: exit 1
来源：http://hz.316326.xyz/gtrafhfjej.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinghuilouyu.cn/gtkhhxwkln.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gtuuchsyyj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shangyingyoupin.top/gtckkilhep.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sufxvd.cn/gtqvhslubh.html

JS:   console.error("err")
来源：http://hz.yueranfly.top/gtuqlenari.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtdwpddrxi.html

Java: System.err.println("err")
来源：http://hz.sweek.top/gtapemnzvc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jianghu66.top/gtovjpwmrt.html

Ruby: warn "err"
来源：http://hz.zhoulong.xyz/gtfdsrfrmj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigfzy.top/gtrlplxcnq.html

[M07] 判断是否为主入口
来源：http://hz.wangdashe.top/gtinhjznva.html

Py:   if __name__ == "__main__":
来源：http://hz.zhaomingkeji.xyz/gtdwnuryig.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuxming.cn/gtkfzvqpps.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtasdecmci.html

TS:   require.main === module
来源：http://hz.jqgufenzy.top/gtfzzwipab.html

Java: public static void main(String[] args)
来源：http://hz.pengpengdd.cyou/gtzzbyrlyp.html

Go:   func main()
来源：http://hz.gaohongyu789.top/gtmbziiaex.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ivvv.top/gtmgydjxzh.html

C#:   static void Main(string[] args)
来源：http://hz.redwolf501.top/gtsuixmwgx.html

[M08] 获取系统与运行时信息
来源：http://hz.ppjwa.cn/gtxnubeied.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtvlqhnmls.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shanyushiyangkeji.top/gtybcoqmpy.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtbkdrurel.html

TS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtltmxcgud.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtmkqvbqzt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhongyouzk.top/gtogomthfv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gogol.net.cn/gtvaiueonx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhiwuduotai.top/gtqfwpdwub.html

================================================================================
来源：http://hz.tanke756.top/gtuagjkdmq.html

N. 数据结构与算法
来源：http://hz.c1oappe.top/gtrffynfpy.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvbbvpfyk.html

[N01] 二分查找（有序数组）
来源：http://hz.yuanzhike.top/gtdxschsas.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigfzy.top/gtsnsokfbi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sxryk.cn/gtswiumpjq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtxdtjotxy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtkklzykbn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtptmlujkb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtrpuguybb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.mhx1999.top/gtiaaciywj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gtzmkgdhue.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shuidangran.top/gtiplhcyiz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtiitpwwvk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtsrbnywzx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtaniyikrq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtpptcjokv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigufen.top/gtyaqlzirx.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtzxeolkxm.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtgfqeatbc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuxming.cn/gtrhzplohj.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtcfolwvbp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgfzy.top/gtykseuuzr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gtalvyicem.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtmoqzgiak.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtoiketbft.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtgbaivwsh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtunbwmlua.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.meibo888.top/gtpwagucnd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aibaodan.cn/gtxssipltz.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gtzzpxmmbs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtzcpgipki.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sxryk.cn/gtiolalrox.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtawjxkwhk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtatahlzkc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtxcbtxkpu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtlmekjtxv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtqtnzguim.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.haohaochexian.top/gtkulztqoe.html

[N05] 最大公约数
来源：http://hz.0kj1m.cn/gtxltckqev.html

Py:   math.gcd(a, b)
来源：http://hz.snrcjt.cn/gtqdolhyxo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gttdonpkct.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtgkdxvmar.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nwbrower.top/gtyceouckg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xziqi.cn/gtvqzoowpj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydjk.org.cn/gtynpnkrya.html

Ruby: a.gcd(b)
来源：http://hz.shuidangran.top/gtvfiyksht.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgfzy.top/gtcfovwuki.html

[N06] 判断回文字符串
来源：http://hz.xinyue.icu/gtuspmzfbg.html

Py:   s == s[::-1]
来源：http://hz.havefunace.top/gtavxcnfyz.html

PHP:  $s === strrev($s);
来源：http://hz.nanxinkj.top/gteiprfqyh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtpjqzpgqp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtfiyyetkb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtwzupwkhm.html

Go:   // 双指针从两端比较
来源：http://hz.xingfuxueyuan.xyz/gtqxkdidkp.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtdnrzijdw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtepbtldap.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gtxlkxhkbl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fzhhl.top/gtqswflknl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.bjfxy.top/gttibosewx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ivvv.top/gthricxfhw.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtmcbqmuzr.html

Java: // 手写 HashMap
来源：http://hz.meibo888.top/gtstixfoth.html

Go:   // 手写 map[int]int
来源：http://hz.fzhhl.top/gtazemwskd.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtqpkuvzsg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yongpay.top/gtnlwxpsoj.html

[N08] 生成全排列
来源：http://hz.fengsongda.top/gtqtwtjzfo.html

Py:   itertools.permutations(arr)
来源：http://hz.jyoumei.cn/gtwfbdrmdy.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtidnuplgu.html

JS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtwsyxqxtk.html

TS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtonxlrwzb.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gthbgbbtcw.html

Go:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtnvmqdsjj.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gtxhlrnrjf.html

C#:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtoasbdfnx.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtbogztchq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ywan-chungtsiang.top/gtkxnpjwxs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hfpthk.cn/gtutajydni.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gttcplctmw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgfzy.top/gtkjkjqeqj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinghuilouyu.cn/gtwhrrrqch.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258.top/gtayhetgac.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zdqjudy.top/gtibxzalfo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtrfvxwsff.html

[N10] 链表节点定义
来源：http://hz.cashguo.top/gtckfgmtky.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shzxlz.cn/gtuibiejug.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gogol.net.cn/gtrldgwqix.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangshuangyany.cn/gttryrlfgl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtutealybe.html

Java: class Node { int v; Node next; }
来源：http://hz.zhaomingkeji.xyz/gtafghlybo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fzhhl.top/gtvfedjrij.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shzxlz.cn/gtoeteqfbe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtrcbapiza.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gthhrhfgwb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xinyue.icu/gtcxiappeb.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtptrrswer.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtqxlraabp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtebekjksk.html

Java: // 手写递归
来源：http://hz.cashguo.top/gtdfkfglms.html

Go:   // 手写递归
来源：http://hz.jianghu66.top/gtaqskmtij.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yanxiufei.cn/gtvapxxglk.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gtkatowsmc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gttjzbrkuh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtjckddtws.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuanzx.com/gtqtndbqru.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gteorwmmfb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtisclkoer.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtupuaafnk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gttfpznltf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtbvrghsgl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtyvfdjoxd.html

================================================================================
来源：http://hz.ivvv.top/gtymejpngg.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtcdszuely.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrpksoogr.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gthxvdelzk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daxiang520.top/gtmmpdkgyl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gtccfursxf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cucudq.cn/gtzqpnpjwf.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtfgrfdyvi.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtpqrbyhde.html

Go:   go f()
来源：http://hz.yj202588.top/gtgmzcojwb.html

Ruby: Thread.new { f }
来源：http://hz.hywenlv.cn/gtpstpcbsg.html

C#:   Task.Run(() => F());
来源：http://hz.dashuyun.cn/gtvjdhjgpf.html

[O02] 使用线程池
来源：http://hz.nwbrower.top/gtxjtveqjy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangtech.top/gtjsiabxsx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.fengsongda.top/gtsndezwml.html

JS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtddexefra.html

TS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtrqvddiae.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daxiang520.top/gtmfijfmcf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shuidangran.top/gtyzsyzwta.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gtvhwmkacu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xziqi.cn/gtzxswtqtj.html

[O03] 加锁保护共享数据
来源：http://hz.wangshuangyany.cn/gtaivygypl.html

Py:   with lock: shared += 1
来源：http://hz.jqgfzy.top/gtpealjdkt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.iojbl.cn/gtndkkfdox.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dianchejie.cn/gtrszncwnn.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtvbpmxvia.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtgikcchre.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gthksbfzxa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgfzy.top/gtqnuzzqni.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj202588.top/gtecwsztsk.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtgvldlntf.html

Py:   async def f():⏎    await g()
来源：http://hz.yanxiufei.cn/gtnbstnvnm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dashuyun.cn/gtfyizsvsr.html

JS:   async function f() { await g(); }
来源：http://hz.vqdsnc.cn/gthonzuprk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxinkj.top/gtshzizsmx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shangyingyoupin.top/gthdnqgqlb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.havefunace.top/gtznelgyme.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gttjtptmid.html

C#:   async Task F() { await G(); }
来源：http://hz.shangyingyoupin.top/gtpfxyrcdm.html

[O05] 并发执行并等待全部完成
来源：http://hz.sufxvd.cn/gtuctmblqg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtnwiyehtj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hywenlv.cn/gtozfukhma.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtvzypdjrs.html

TS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtegrqvpwk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jyoumei.cn/gtkgrqxuym.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhengqikj.top/gtxzfbyhox.html

Ruby: threads.map(&:join)
来源：http://hz.dianchejie.cn/gtdnuuhzrc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuanzx.com/gtzsmlhrah.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gtxjhgmymj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gtcqbbxrxb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhengqikj.top/gtvfatgjdd.html

JS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtdbrjxmiy.html


<!-- 参考信息 -->