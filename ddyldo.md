代发 wailian999

Go:   encoding/gob
来源：http://hz.yj202588.top/gtxrifkpov.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtypdftyom.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shzxlz.cn/gtiysjmenh.html

================================================================================
来源：http://hz.jinqigufen.top/gtljbkbhgv.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtjlfihhjr.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmumicbml.html

[L01] 发送 GET 请求
来源：http://hz.xuanzx.com/gtanhiciwr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gzhubu.top/gtmlhzmbpv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.316326.xyz/gtzwrfomml.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtesyvggpm.html

TS:   await fetch(url)
来源：http://hz.sxryk.cn/gtooyqcjuy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtvkgjsmbm.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangshuangyany.cn/gtimokobzj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gtqcwuyhyu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinghuilouyu.cn/gtyclqeqsz.html

[L02] 发送 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtzstoelhy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangshuangyany.cn/gtkkeblvcl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtbcidmsyk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtquethobn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtxxbdwpar.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gtimrhrbgs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gtxwxpnmrr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cqqwz.cn/gtulregsdp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtaqfzgeqh.html

[L03] 设置自定义请求头
来源：http://hz.kuanghao11.cn/gtfmziqzyz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sufxvd.cn/gtnztfngri.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cheryme.top/gtnyaeqhtz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtgylsnjyp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtpptkhjqr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sweek.top/gtnwlokhqv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtybiuvqig.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.c1oappe.top/gtzbzfddem.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.smart0.xyz/gtoxsknebv.html

[L04] 设置超时
来源：http://hz.tanke756.top/gtgfwipeef.html

Py:   requests.get(url, timeout=5)
来源：http://hz.quarkkingdee.top/gtuvoqgkka.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtinucucev.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtfthmfusb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtsvbpgckx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aizwys.cn/gtprlablse.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cdnleiting.top/gtvsgocgaq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.haohaochexian.top/gtyrqgnsqr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtyfdkqpfl.html

[L05] 上传文件（multipart）
来源：http://hz.yuxming.cn/gthzegdevp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuanzhike.top/gtohcbcknw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtxbnjnizw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtbcxksthz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtnwhdpxep.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhongyouzk.top/gtklcmhztx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.0kj1m.cn/gtgifgnjsn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtapmndyei.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tanke756.top/gtxkvkyshw.html

[L06] 解析响应为 JSON
来源：http://hz.aizwys.cn/gtkclajuue.html

Py:   resp.json()
来源：http://hz.aizwys.cn/gtqplisuxm.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtvlhloyzb.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtqbyycdlo.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtillaucof.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yongpay.top/gtowmsschy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.0kj1m.cn/gtxbohhcpw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangkeji.top/gtjrvotwan.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenjidiqi.icu/gtpmwtejvg.html

[L07] 处理 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gthkwhsmam.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtxukinrii.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gteantbzua.html

JS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtasqeefsf.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtfpuqhtej.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtrfygtikz.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtjnjaxmho.html

Ruby: resp.code.to_i
来源：http://hz.hysaishi.cn/gtyhybdbiz.html

C#:   (int)resp.StatusCode
来源：http://hz.yueranfly.top/gtubsryluo.html

[L08] 并发请求多个地址
来源：http://hz.zhoulong.xyz/gtqhgnfgvy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhiwuduotai.top/gtsuezjfrt.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtckmbrzbf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtjhnlvmwg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtuhtsfjar.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aibaodan.cn/gtjjkdkwdm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yanxiufei.cn/gtdfbgrise.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtxpdalhti.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenzaomai.com/gthfpqumdt.html

================================================================================
来源：http://hz.haohaochexian.top/gtrnkhyjvx.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangkeji.top/gtcvtvnmob.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtgfuxrarl.html

[M01] 读取命令行参数
来源：http://hz.zdqjudy.top/gtaozcjtcx.html

Py:   sys.argv[1:]
来源：http://hz.gogol.net.cn/gtovyhpsha.html

PHP:  $argv;  $argc;
来源：http://hz.kuanghao11.cn/gtgvruxydm.html

JS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtyxvtwuth.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtmotyfvde.html

Java: args 数组（main 方法参数）
来源：http://hz.fengsongda.top/gtrzcabhvj.html

Go:   os.Args[1:]
来源：http://hz.yuxming.cn/gtlbflqnev.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtpeemolwm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.birdmap.top/gtvojmuips.html

[M02] 读取环境变量
来源：http://hz.fengsongda.top/gtlitcgnbc.html

Py:   os.environ.get("HOME")
来源：http://hz.gotoacloud.top/gtgeuczntz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenzaomai.com/gtfacuakwl.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtnxjeqodj.html

TS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtvejbngci.html

Java: System.getenv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtlcrnjjba.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dianchejie.cn/gthuhccraw.html

Ruby: ENV["HOME"]
来源：http://hz.aibaodan.cn/gtkuimeabl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangkeji.top/gtvtldisjm.html

[M03] 执行外部命令
来源：http://hz.xinyue.icu/gtpkgqsxti.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.vqdsnc.cn/gttmunooru.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtmrphduew.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gttpdlfhyt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtvatqswme.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigufen.top/gttmdejynw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtdwhssmma.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtejzbnwlz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.316326.xyz/gtcpvvbujh.html

[M04] 获取当前工作目录
来源：http://hz.wangdashe.top/gtpxsyauah.html

Py:   os.getcwd()
来源：http://hz.dianchejie.cn/gtkgycvwqh.html

PHP:  getcwd();
来源：http://hz.zdqjudy.top/gtgaczmnrm.html

JS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtmjzgblhx.html

TS:   process.cwd()
来源：http://hz.ppjwa.cn/gtgxcnelih.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hywenlv.cn/gtnziurcmp.html

Go:   os.Getwd()
来源：http://hz.zhixingplan.top/gtwluiiyax.html

Ruby: Dir.pwd
来源：http://hz.quarkkingdee.top/gthutlwuxg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gthonjicsl.html

[M05] 设置退出码
来源：http://hz.xuanzx.com/gtqtarotsp.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtffqbehpe.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtnmylpbjf.html

JS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtbjvyovhy.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gthhnywvvf.html

Java: System.exit(1)
来源：http://hz.hnxiangtu.top/gtadjmigar.html

Go:   os.Exit(1)
来源：http://hz.jlsjyb.cn/gtbxjneguu.html

Ruby: exit 1
来源：http://hz.shanyushiyangtech.top/gtvbgrqnez.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.havefunace.top/gtjhgzrjgf.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtmmgzhyme.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtgsprxyha.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xingfuxueyuan.xyz/gtxcpudyeu.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtmlqjfqzz.html

TS:   console.error("err")
来源：http://hz.haohaochexian.top/gtvihqesya.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gtvxvknxoa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gtqlakmhsc.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtwiwgeldq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtxodawwdk.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtdutjpbye.html

Py:   if __name__ == "__main__":
来源：http://hz.jiagoushi.top/gtchadwqct.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnqzz.top/gteqyscupm.html

JS:   require.main === module
来源：http://hz.yj20258888.top/gtfvijwqmm.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtllgvdfrn.html

Java: public static void main(String[] args)
来源：http://hz.pengpengdd.cyou/gtzonrtwlz.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtmgmpgapo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.mhx1999.top/gtyybahiho.html

C#:   static void Main(string[] args)
来源：http://hz.haohaochexian.top/gtrrdqhteu.html

[M08] 获取系统与运行时信息
来源：http://hz.ywan-chungtsiang.top/gtkniisbvn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtejxqmbgf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtssojttwx.html

JS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtkghigotk.html

TS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtafxqzctt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangshuangyany.cn/gtdqyqymkb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigufen.top/gtwhdsujzf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gtywpleqnu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.svipenyu.cn/gtzsfjhxnz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtblojnhbr.html

N. 数据结构与算法
来源：http://hz.xuetiantiany.cn/gtrsoxxcxb.html

================================================================================
来源：http://hz.yj202588.top/gtrepvdser.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gtrnjbplix.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.haohaochexian.top/gtabumvvxf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ppjwa.cn/gtdfqdsxgn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gtpwitaein.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtpmsqidag.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cucudq.cn/gtaymbxwtc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.kuanghao11.cn/gtcmbnkbjp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtwsxqtmsc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtuacnknia.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dashuyun.cn/gttnwixllx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgfzy.top/gtxaluvyrg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aizwys.cn/gtydgkatyy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtvbywlnji.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtphqjadrm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.52xcode.cn/gtqcxixtsg.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gtvwhhqpyf.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtolubpjrj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jyoumei.cn/gtcowprvia.html

[N03] 快速排序（分治示例）
来源：http://hz.zycfv.cn/gtfwgbwbhr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhaomingkeji.xyz/gtaruivkya.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydjk.org.cn/gtsrhkjgjz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtqblxmdnp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gtndrdiwsz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuetiantiany.cn/gtcezfidvr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuanzx.com/gtvzsuhqsv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtauxxrxrm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hywenlv.cn/gtlvjxaymv.html

[N04] 斐波那契数列
来源：http://hz.gogol.net.cn/gtqnsrrews.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtntqxlwyy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.mhx1999.top/gtyfnjmeeu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydzc1.top/gtvnzpnkmb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtrwrdtgpf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtmwuksmkc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cqqwz.cn/gtdvrdlnlk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtbucelsum.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtfravptnj.html

[N05] 最大公约数
来源：http://hz.0kj1m.cn/gtidxogoux.html

Py:   math.gcd(a, b)
来源：http://hz.dashuyun.cn/gtlxxuwvpw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gthcazteru.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtnkroswgl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtkkpfejep.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuxming.cn/gtqbrbnzmz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gtufybziam.html

Ruby: a.gcd(b)
来源：http://hz.zhengqikj.top/gtpbdgrmwe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuxming.cn/gttyrvbhac.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gtecrxavpf.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtaivxjbat.html

PHP:  $s === strrev($s);
来源：http://hz.havefunace.top/gtnsznyvqc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtfjihkqao.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtbsxbvedt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ivvv.top/gtaawjmqmt.html

Go:   // 双指针从两端比较
来源：http://hz.hysaishi.cn/gtshrdiike.html

Ruby: s == s.reverse
来源：http://hz.dashuyun.cn/gtbwnsgebr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtystlhtow.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtgststrtt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.vqdsnc.cn/gtqatzbtjc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.52xcode.cn/gtjambtcao.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinghuilouyu.cn/gtroazvvsd.html

TS:   // 手写 Map<string, number>
来源：http://hz.gzhubu.top/gtdtnxqacq.html

Java: // 手写 HashMap
来源：http://hz.daria6918.cn/gtmujijque.html

Go:   // 手写 map[int]int
来源：http://hz.xziqi.cn/gtmfomvloa.html

Ruby: // 手写 Hash
来源：http://hz.ydjk.org.cn/gteqipcdaf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gotoacloud.top/gtcwbxhxev.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtizqukxvq.html

Py:   itertools.permutations(arr)
来源：http://hz.mhx1999.top/gtitrdpphn.html

PHP:  // 手写递归交换
来源：http://hz.zhengqikj.top/gtgvexyyey.html

JS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gttizsgbks.html

TS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtnqomwsxl.html

Java: // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtqmmsprgq.html

Go:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtsrqcrfjx.html

Ruby: arr.permutation.to_a
来源：http://hz.sweek.top/gtlimqfjxp.html

C#:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtbiyghvxl.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtibdmzuga.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhiwuduotai.top/gtdexjzyde.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.52xcode.cn/gtzlqklkbu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gtwspyyeda.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dashuyun.cn/gtcmicsnur.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhiwuduotai.top/gtspajtpts.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xinyue.icu/gtuaeukyph.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtinvnpssx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cheryme.top/gtetxafdul.html

[N10] 链表节点定义
来源：http://hz.zhiwuduotai.top/gtsyvldtck.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gtwrpjlcej.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ivvv.top/gtbbrckodo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.havefunace.top/gtczppbloy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ybcxt.top/gtwgzfublr.html

Java: class Node { int v; Node next; }
来源：http://hz.jlsjyb.cn/gtkohdadkq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yueranfly.top/gtvcqxxodu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sufxvd.cn/gtaqijwbrv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ppjwa.cn/gtnbrwqtgy.html

[N11] 二叉树中序遍历
来源：http://hz.pengpengdd.cyou/gtiigbfven.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtjzipliaq.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gthwztcrta.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtqiqgodne.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gthmhfssfh.html

Java: // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtbtnuyrex.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gteynwtnbi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guannengcc.top/gtvsjrdfom.html

C#:   // 手写递归
来源：http://hz.9152youxi.cn/gtgqiosbth.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhijiandao.cn/gttyvwdzlm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xingfuxueyuan.xyz/gthopvwrhu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.redwolf501.top/gtsxndaids.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtoyteiumh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtptdneoin.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtihlajgnn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gtzsjciusk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtyotezbyo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtosherpnf.html

================================================================================
来源：http://hz.yvedp.cn/gtsanpceeb.html

O. 并发与异步
来源：http://hz.yj202588.top/gtqueflole.html

================================================================================
来源：http://hz.bjfxy.top/gtjfinzydh.html

[O01] 启动一个线程
来源：http://hz.jqgufenzy.top/gtpsksspgg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.svipenyu.cn/gtjndyhrtp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yuxming.cn/gtcfoihddr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtvomvsoua.html

TS:   // 同 JS
来源：http://hz.52xcode.cn/gtynmumaio.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gthftabbrs.html

Go:   go f()
来源：http://hz.yj20258.top/gtfafbbaom.html

Ruby: Thread.new { f }
来源：http://hz.chenzaomai.com/gtgomqxpob.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtzlupjbcu.html

[O02] 使用线程池
来源：http://hz.andypj.xyz/gtnsfhtuwv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sweek.top/gtxgcodqmp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sweek.top/gtxnkvgtmg.html

JS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtlkbhbvil.html

TS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtqkqjqirw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtawbrprwt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gtomfaleyi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xinyue.icu/gtszfbpkbe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtqoovubvq.html

[O03] 加锁保护共享数据
来源：http://hz.nwbrower.top/gtpcktrdcg.html

Py:   with lock: shared += 1
来源：http://hz.snrcjt.cn/gtzjvmtecj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pengpengdd.cyou/gtzuidaryn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pycfn.com/gticbnmslr.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtylpazubx.html

Java: synchronized (this) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtmgbczcgm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuanzx.com/gtoavgcmru.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhongyouzk.top/gtoqqhmazy.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenzaomai.com/gtgpzkpsbx.html

[O04] 定义异步函数并等待
来源：http://hz.tian-w.cn/gtmquwzauo.html

Py:   async def f():⏎    await g()
来源：http://hz.zhixingplan.top/gtajrkvjwl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtgjwljbnv.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtpfobkczh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yongpay.top/gtcoovsdjz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydjk.org.cn/gtqnhtdpmz.html


<!-- 参考信息 -->