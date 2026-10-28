代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhoulong.xyz/gtdwuuzxdo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gthrdypggv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gtkdhrffbk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtoifzdbek.html

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtjqtejtef.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gtekwbryxb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gtcjhmxlsp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtwhzqyvnv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtckzqodgz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pycfn.com/gtkcljgign.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtipnqwelr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtdgnbdmsi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gthiobusnl.html

[L04] 设置超时
来源：http://hz.jyoumei.cn/gtqrwjlsjj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jiagoushi.top/gthrkwagnq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtqbsbhzau.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gttsjvrfdn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtqywizpkj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhongyouzk.top/gtkzsxhoiu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtmbrbqctj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.haohaochexian.top/gtlagivpbm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtvuxanlpl.html

[L05] 上传文件（multipart）
来源：http://hz.zhixingplan.top/gtffxeamvg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuxming.cn/gtplxnxgbw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinyuanbaomall.cn/gtezwbhjyv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtfccgazdx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtsgwdirmd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jyoumei.cn/gtxmvbngsd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtsfdnqkbz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gtkurmminx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhengqikj.top/gtyatospsg.html

[L06] 解析响应为 JSON
来源：http://hz.yanxiufei.cn/gtjzhbxprp.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtazfccxcb.html

PHP:  json_decode($body, true);
来源：http://hz.shzxlz.cn/gthlkbpddn.html

JS:   await resp.json()
来源：http://hz.daria6918.cn/gtrkykdafn.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtilgpbexa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtrmykhaxl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj202588.top/gtsehtpxxv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jlsjyb.cn/gtmbczxzxk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtmcnvnfzj.html

[L07] 处理 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtxukrczad.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtnxvqobnh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuxming.cn/gtxnxknhma.html

JS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gttprkesae.html

TS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtzhwmyzif.html

Java: resp.statusCode()
来源：http://hz.jinyuanbaomall.cn/gtgrlopphk.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtcrrovylv.html

Ruby: resp.code.to_i
来源：http://hz.sysykeji.top/gtdizxmzsy.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258888.top/gtgmfesxpc.html

[L08] 并发请求多个地址
来源：http://hz.cqqwz.cn/gtglraltua.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gzhubu.top/gtvxzvcnhl.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtjbgdcpkp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtmejemxmh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtusqswuba.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gtvngenqgd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtobkuptdw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cheryme.top/gtaweucjnm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cashguo.top/gtskunwzii.html

================================================================================
来源：http://hz.ydjk.org.cn/gtymdycjzp.html

M. 命令行 / 进程 / 环境
来源：http://hz.ywan-chungtsiang.top/gtgvhrjego.html

================================================================================
来源：http://hz.daria6918.cn/gtouiaieji.html

[M01] 读取命令行参数
来源：http://hz.jiagoushi.top/gtjtemgzbl.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtiytkujui.html

PHP:  $argv;  $argc;
来源：http://hz.ydjk.org.cn/gtuwccpctq.html

JS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtlohovege.html

TS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gthyftzbrc.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtqtuflpdx.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtxxahqdme.html

Ruby: ARGV
来源：http://hz.nwbrower.top/gtkfpxapbz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtrdblpecw.html

[M02] 读取环境变量
来源：http://hz.guowangkeji.top/gtajlbzxca.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gtjfqnlvmq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtwkhwmxij.html

JS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtkgnisaqb.html

TS:   process.env.HOME
来源：http://hz.c1oappe.top/gtjcusecfq.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtcxrywsio.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ehwqpu.com/gtfmbzrxde.html

Ruby: ENV["HOME"]
来源：http://hz.316326.xyz/gtivxjneub.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydjk.org.cn/gtxxafraxm.html

[M03] 执行外部命令
来源：http://hz.yvedp.cn/gtmzjvtblq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jlsjyb.cn/gtdubkgfoh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtztsrfwsz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtdsomlggh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtvytkjgqn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtqtqvwkca.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ppjwa.cn/gttqudwwze.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtscsdtzns.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigufen.top/gtwgdrufci.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gteahvisxg.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtowzxcefj.html

PHP:  getcwd();
来源：http://hz.c1oappe.top/gtnqscjuxz.html

JS:   process.cwd()
来源：http://hz.smart0.xyz/gtjltvbqpl.html

TS:   process.cwd()
来源：http://hz.birdmap.top/gtxpxdwirm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtavcfhxgd.html

Go:   os.Getwd()
来源：http://hz.daxiang520.top/gtzgorefdr.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtvdrrbhdr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtwzzuujvb.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtkkgyqkdn.html

Py:   sys.exit(1)
来源：http://hz.yj20258.top/gtlrfttnpl.html

PHP:  exit(1);
来源：http://hz.9152youxi.cn/gtyvacudqn.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gtjdrbkwhh.html

TS:   process.exit(1)
来源：http://hz.aizwys.cn/gtsyrwhvrw.html

Java: System.exit(1)
来源：http://hz.yj202588.top/gtqvzaddfz.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtxzavxdec.html

Ruby: exit 1
来源：http://hz.andypj.xyz/gtypbenbdx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.snrcjt.cn/gtyykittsr.html

[M06] 向标准错误输出
来源：http://hz.zhengqikj.top/gtuvwzglek.html

Py:   print("err", file=sys.stderr)
来源：http://hz.9152youxi.cn/gtsgmymczy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtlbfbcrgl.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gttldlrjiy.html

TS:   console.error("err")
来源：http://hz.shzxlz.cn/gtmlqjarvn.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gthtweipvg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dashuyun.cn/gtfqzbenpe.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gtdrfhldoj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gtjbvvjneh.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtlwchuclt.html

Py:   if __name__ == "__main__":
来源：http://hz.ydzc1.top/gtijwvwujl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydzc1.top/gteuigisux.html

JS:   require.main === module
来源：http://hz.fengsongda.top/gtfubdupzw.html

TS:   require.main === module
来源：http://hz.hysaishi.cn/gtrprjivwd.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtixhoqgln.html

Go:   func main()
来源：http://hz.nanxinkj.top/gtoqzdetnd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hfpthk.cn/gtwopblcgu.html

C#:   static void Main(string[] args)
来源：http://hz.sxryk.cn/gtizusjsic.html

[M08] 获取系统与运行时信息
来源：http://hz.316326.xyz/gtehsqerzd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.smart0.xyz/gtxrltybeh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtohbeaqhg.html

JS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtxzdrmtyj.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtkowaufyj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.havefunace.top/gtgixwzqqp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhijiandao.cn/gtudykkojp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gtvqxyxzvd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shuidangran.top/gtdobsbkog.html

================================================================================
来源：http://hz.fengsongda.top/gttcqfxgkn.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gtegwjrwxg.html

================================================================================
来源：http://hz.yvedp.cn/gtcuxdxptm.html

[N01] 二分查找（有序数组）
来源：http://hz.xziqi.cn/gthhiegrjg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtihomfbqp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pycfn.com/gtavfgbsjs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtntxzdfjn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtfuognodq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtplljetbi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtadoxlitt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtlxlcbwlo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtqanswhwp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinqigufen.top/gtkqtjuumk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtjtemcmfj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.9152youxi.cn/gtgyoptfle.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gttkrpyggt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtllxoitbw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aibaodan.cn/gtoyexuhfw.html

Go:   slices.Sort(arr)
来源：http://hz.fengsongda.top/gtolemcvbh.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtygkhstbl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.kuanghao11.cn/gtzeradyde.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gtbwnprbrp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cucudq.cn/gtqxmbafbo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.snrcjt.cn/gtqnvuannn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtxbrnyahp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtqamduibb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ehwqpu.com/gtckmlmtek.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.kuanghao11.cn/gtzkflcxup.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.316326.xyz/gtohpfggna.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangdashe.top/gtmejfzjzn.html

[N04] 斐波那契数列
来源：http://hz.kuanghao11.cn/gthuwmqlwg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.aibaodan.cn/gttberatqt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhengqikj.top/gtyvqlqtas.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtgfyfjjle.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtrfqkszzm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.iojbl.cn/gtvechxexq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenzaomai.com/gtuhudaspi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtwldupiwq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aizwys.cn/gtaeberhmk.html

[N05] 最大公约数
来源：http://hz.chenzaomai.com/gtmlszpdej.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtuxrrkdzl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtgpubnkxw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtqgovckyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtzuxlpjxj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nwbrower.top/gtzkuebskp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nwbrower.top/gtfvbdofpt.html

Ruby: a.gcd(b)
来源：http://hz.tanke756.top/gtgboijqcr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhoulong.xyz/gtyzbwoohs.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtxoschaev.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtsedvrztk.html

PHP:  $s === strrev($s);
来源：http://hz.52xcode.cn/gtzakffhcr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtflikrutt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtevhgmvqd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtmuaojmlq.html

Go:   // 双指针从两端比较
来源：http://hz.zhengqikj.top/gtbshlthio.html

Ruby: s == s.reverse
来源：http://hz.dianchejie.cn/gtcubsglss.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gtpvdxkqfu.html

[N07] 两数之和（返回下标）
来源：http://hz.ehwqpu.com/gtoloviwcx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhixingplan.top/gtbwfyqmkz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sysykeji.top/gtcijrgcrv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tian-w.cn/gtcylihwud.html

TS:   // 手写 Map<string, number>
来源：http://hz.mhx1999.top/gthkcacoxo.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtryihvgom.html

Go:   // 手写 map[int]int
来源：http://hz.nwbrower.top/gtqbalaxdw.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gtcjhsfloz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydzc1.top/gtyzyfysbc.html

[N08] 生成全排列
来源：http://hz.fengsongda.top/gtkmumjmfk.html

Py:   itertools.permutations(arr)
来源：http://hz.cucudq.cn/gtfacnpjzb.html

PHP:  // 手写递归交换
来源：http://hz.hnxiangtu.top/gtinhtqwxw.html

JS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtzvnjmjzl.html

TS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtfafeqzhe.html

Java: // 手写回溯递归
来源：http://hz.guowangkeji.top/gtnaqbekts.html

Go:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtaszugyob.html

Ruby: arr.permutation.to_a
来源：http://hz.ppjwa.cn/gtldudtagu.html

C#:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtqypmphsd.html

[N09] 栈与队列
来源：http://hz.hammf.cn/gtkketornv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tian-w.cn/gtagdlnieg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gtpmholskn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yonumen.top/gtsiqgqvmo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cashguo.top/gtffiyaocu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenlongwang.top/gtalckyxcv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xingfuxueyuan.xyz/gtvwxmtddo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.iojbl.cn/gtxtlgotoe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydjk.org.cn/gtomidnqys.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gtseinjqut.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pengpengdd.cyou/gtefwnxbfx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pycfn.com/gtadbgitql.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jyoumei.cn/gtornsheee.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.smart0.xyz/gtrzstttnf.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtjauzzypf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sufxvd.cn/gtwhysbtkf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.smart0.xyz/gtjeqmpgdr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pengpengdd.cyou/gtopxhvhkz.html

[N11] 二叉树中序遍历
来源：http://hz.jqgfzy.top/gtslcgfdey.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gtjrsydupy.html

PHP:  // 手写递归函数
来源：http://hz.cashguo.top/gthgmcqycd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtbzkqzhvs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtlruptxdr.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtihfrfnii.html

Go:   // 手写递归
来源：http://hz.zhoulong.xyz/gtwilxoapt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhoulong.xyz/gtchrqegrq.html

C#:   // 手写递归
来源：http://hz.hfpthk.cn/gtsianhkpd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenjidiqi.icu/gthstgeykv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtgukgipzd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cqqwz.cn/gtcnowybbg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtowwhbmnv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtrdfkakzb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtxvumgjwj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.52xcode.cn/gtrvkqwzwu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtcegwvmhn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtgurxbgqj.html

================================================================================
来源：http://hz.52xcode.cn/gtdrzldggs.html

O. 并发与异步
来源：http://hz.redwolf501.top/gthyjtucng.html

================================================================================
来源：http://hz.chenzaomai.com/gtvuhvzbmw.html

[O01] 启动一个线程
来源：http://hz.52xcode.cn/gttwrlumsh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhengqikj.top/gthxrufftd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.andypj.xyz/gtnptggzos.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hammf.cn/gtivunhnmk.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtswzhxhjn.html

Java: new Thread(() -> f()).start()
来源：http://hz.xylfe.cn/gteuebqemx.html

Go:   go f()
来源：http://hz.shuidangran.top/gtrgkbndcl.html

Ruby: Thread.new { f }
来源：http://hz.xylfe.cn/gtxfyndalt.html

C#:   Task.Run(() => F());
来源：http://hz.snrcjt.cn/gtcauhpwys.html

[O02] 使用线程池
来源：http://hz.cucudq.cn/gtmltalahy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tianlin.xyz/gtvoelhowr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.haohaochexian.top/gteinsuyaz.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtvzgvxczs.html

TS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtyplbaevh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.fzhhl.top/gtlpoaiagn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shangyingyoupin.top/gtqjhvqkog.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuetiantiany.cn/gtfxopgvsq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtcyzqtnsu.html

[O03] 加锁保护共享数据
来源：http://hz.chenjidiqi.icu/gtrbtvrcvm.html

Py:   with lock: shared += 1
来源：http://hz.zdqjudy.top/gtrmglaizi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtzspxaskh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pengpengdd.cyou/gttpionjyh.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtrtnfuqbz.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnxiangtu.top/gtyxkcmthr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tanke756.top/gtgcrlfqwf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtttfvdiwr.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtnakutkcf.html

[O04] 定义异步函数并等待
来源：http://hz.sufxvd.cn/gtedyeywdn.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gtcthmtvpr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtmljxozhz.html

JS:   async function f() { await g(); }
来源：http://hz.zhongyouzk.top/gtmgyghiqk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xziqi.cn/gtztsdjeag.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydjk.org.cn/gtpbquxcnf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daria6918.cn/gtikszgznp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtoqgacpdq.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigfzy.top/gtzbmuwomb.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenjidiqi.icu/gtnqejgrnk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daxiang520.top/gtkspfferv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.smart0.xyz/gtfavcgojh.html

JS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtlbgjguhg.html

TS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtprhdpfpd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhengqikj.top/gticvwlxuo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtehqncmbe.html

Ruby: threads.map(&:join)
来源：http://hz.xinyue.icu/gtfkndqutu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.haohaochexian.top/gtqjwontpz.html

[O06] 使用进程池
来源：http://hz.iojbl.cn/gtuxgqutyi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gotoacloud.top/gtzcehuhtm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.haohaochexian.top/gtneydxeqf.html

JS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtnluufpkx.html

TS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtrkpybtvl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gtxubdworx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jiagoushi.top/gthriegyty.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gtzvjjbfrk.html


<!-- 参考信息 -->