代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.yuanzhike.top/gtjtzqnqdz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gtpvujtaaq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtsltltqsf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtgciicmuq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtzjsqyeud.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtnwjklnvm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtwreulxry.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtiewbrqqa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zdqjudy.top/gthjqzlzvo.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtxvvhsyta.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtyltauarq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtlyqbgzdx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtxsksosdb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtskzhxaig.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yonumen.top/gtvbshbicv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gtfkmcwuzw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ehwqpu.com/gtyttckulv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cqqwz.cn/gtqrwmkczq.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gtxrwllauz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cdnleiting.top/gtauzgjyas.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxuanxn.top/gtqgxaeaor.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtfwlzigbp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtdtncyths.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtxomcppvx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gtbpefbjkk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinghuilouyu.cn/gtmdtvccfc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtrvqgmzeq.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gthprtvsfh.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gtgiszslss.html

PHP:  json_decode($body, true);
来源：http://hz.zhongyouzk.top/gtxzjqwvxb.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtqtnekcxl.html

TS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtyuxdppxo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtokyqirfg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuanzhike.top/gtpbchromz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tian-w.cn/gtdaufwwki.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangkeji.top/gtckjagfcr.html

[L07] 处理 HTTP 状态码
来源：http://hz.cheryme.top/gtnyubrnyh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtqnjtbbyw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tanke756.top/gtzmfibfrc.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtnmtewdkc.html

TS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtsxnflbzi.html

Java: resp.statusCode()
来源：http://hz.birdmap.top/gtdczimrpp.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtieyqcfcr.html

Ruby: resp.code.to_i
来源：http://hz.wangshuangyany.cn/gtbldyirjq.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtvjfcnyzj.html

[L08] 并发请求多个地址
来源：http://hz.feifeiyinyue.top/gtjjcqoazs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shangyingyoupin.top/gtrdcmvixz.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydzc1.top/gtiombiteh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtklninnhz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtxyfyxiuz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xingfuxueyuan.xyz/gtrfbjxdga.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daxiang520.top/gtbubkoqnn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangshuangyany.cn/gthkohszmg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ppjwa.cn/gtpgxpcgqt.html

================================================================================
来源：http://hz.pycfn.com/gtcaalkqxk.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtkcxtbqlx.html

================================================================================
来源：http://hz.pycfn.com/gthednmold.html

[M01] 读取命令行参数
来源：http://hz.zhongyouzk.top/gtifjkxlbo.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtpesndqzi.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtkhoefkbs.html

JS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtxfjqgswg.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtddqzpuce.html

Java: args 数组（main 方法参数）
来源：http://hz.hnqzz.top/gtsqlyxbrp.html

Go:   os.Args[1:]
来源：http://hz.smart0.xyz/gtipsrrsac.html

Ruby: ARGV
来源：http://hz.jianghu66.top/gtflhhqxop.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gotoacloud.top/gtbnajpdig.html

[M02] 读取环境变量
来源：http://hz.iojbl.cn/gtutzfiyby.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gtmsziiwwq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxinkj.top/gtyunpbexp.html

JS:   process.env.HOME
来源：http://hz.yj202588.top/gtcjbkrbtv.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtrcazwauw.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtyrhjmwsp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydzc1.top/gtxcgcwrto.html

Ruby: ENV["HOME"]
来源：http://hz.guowangkeji.top/gtymanktij.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtbuqqewxn.html

[M03] 执行外部命令
来源：http://hz.jlsjyb.cn/gtdpqpxcso.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinqigfzy.top/gtfdebjdhw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.kuanghao11.cn/gtcofprmqx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtfbfooflo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtelvevgqj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gtmxfarfia.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sysykeji.top/gtndrjhgby.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fengsongda.top/gteljoafmh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yongpay.top/gtcpsdahge.html

[M04] 获取当前工作目录
来源：http://hz.vqdsnc.cn/gtxoaoouob.html

Py:   os.getcwd()
来源：http://hz.zhaomingkeji.xyz/gtdtegcwtx.html

PHP:  getcwd();
来源：http://hz.pengpengdd.cyou/gtxdyhcelo.html

JS:   process.cwd()
来源：http://hz.daria6918.cn/gttxjnqzvd.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtbcmxrnfz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shzxlz.cn/gtgbcnnhkm.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtmnidinru.html

Ruby: Dir.pwd
来源：http://hz.vqdsnc.cn/gtwbvwdzru.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gtusyrfwrj.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtyyqtwxvx.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtwrzvbvwg.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtwealtqbq.html

JS:   process.exit(1)
来源：http://hz.ydzc1.top/gtdcrjiucq.html

TS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtxmalwlmj.html

Java: System.exit(1)
来源：http://hz.hfpthk.cn/gtrzrfhllq.html

Go:   os.Exit(1)
来源：http://hz.sysykeji.top/gtxslvhlpr.html

Ruby: exit 1
来源：http://hz.fengsongda.top/gtorkfeopj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jlsjyb.cn/gtklovtykq.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtxwgoweku.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jianghu66.top/gtmtfqcdqo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guowangkeji.top/gttiufyvro.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtonjwhabf.html

TS:   console.error("err")
来源：http://hz.yongpay.top/gthhbrmanu.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gtuafekhxo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.kuanghao11.cn/gtdrmtghrm.html

Ruby: warn "err"
来源：http://hz.yueranfly.top/gtpdldfigy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhongyouzk.top/gtkipvkkpl.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtravbqukv.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtqqfhlvxm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuanzx.com/gtkxjadwyp.html

JS:   require.main === module
来源：http://hz.zhoulong.xyz/gterkhvisz.html

TS:   require.main === module
来源：http://hz.nanxuanxn.top/gtstbbvtnw.html

Java: public static void main(String[] args)
来源：http://hz.jinqigufen.top/gtjgylkppo.html

Go:   func main()
来源：http://hz.iojbl.cn/gtonpwxxrd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hammf.cn/gtyunvomlx.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gtbacodxpi.html

[M08] 获取系统与运行时信息
来源：http://hz.birdmap.top/gtxcwtebhq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hfpthk.cn/gtplhblixz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtehkroryf.html

JS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtapvsljrf.html

TS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtsimakdat.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtltxsbocl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tian-w.cn/gtcfaxnddc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guowangkeji.top/gtwycgyvbz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gtqeenxhwl.html

================================================================================
来源：http://hz.zycfv.cn/gtvmhfuguc.html

N. 数据结构与算法
来源：http://hz.dashuyun.cn/gtmwtdpias.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnzmtwclc.html

[N01] 二分查找（有序数组）
来源：http://hz.shangyingyoupin.top/gtnqrpuaun.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.havefunace.top/gttoddvmzk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hysaishi.cn/gtpabqhwgx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtbafntgps.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtsdzessjj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gtzogpxxxh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtbxtvisyh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtjntqdhvc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gtjaizzswq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.meibo888.top/gtmgxvwfym.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtemdcgepo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gthwmjpgkn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtghbmayvr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtqqfbeotr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtegfoocyh.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtzieqaygf.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtvtmwtaag.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtgmrhqdze.html

[N03] 快速排序（分治示例）
来源：http://hz.9152youxi.cn/gtotcotmyv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangshuangyany.cn/gtrbnpsqvv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hongshengwenyu.top/gtisxfzprc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtgdofyyap.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtpgesphel.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.havefunace.top/gtwevjyiox.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gotoacloud.top/gthahvgmbl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pengpengdd.cyou/gtkjavnbga.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtiatfownr.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtwjqqgcgz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gterqfnckw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhongyouzk.top/gtepdkjvwt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtnnrudsbd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gthghigijc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gtemgrlpei.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhoulong.xyz/gtjfeructl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtedrpesgc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhoulong.xyz/gtqfnsgszl.html

[N05] 最大公约数
来源：http://hz.hfpthk.cn/gtxuwvuojp.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtfhkyjpfh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hysaishi.cn/gthvmwesel.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtqatsxlma.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtbyzniiba.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydzc1.top/gtjedyeypf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gtigdbvrcr.html

Ruby: a.gcd(b)
来源：http://hz.ivvv.top/gtbacxasbx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hammf.cn/gtcspswilw.html

[N06] 判断回文字符串
来源：http://hz.yangfankeji.com/gtltyuthby.html

Py:   s == s[::-1]
来源：http://hz.yj20258888.top/gteiqvkooq.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtscyoyyct.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtxjqdaolp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gthhrtcouu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinyuanbaomall.cn/gtrqikzcoy.html

Go:   // 双指针从两端比较
来源：http://hz.guannengcc.top/gtyptyhovj.html

Ruby: s == s.reverse
来源：http://hz.smart0.xyz/gtuhmzrtnu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtvxgnojjo.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gtipjgvdtr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuanzx.com/gtxmfkhzwy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gtasenyypm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtvvahgqqb.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuanzx.com/gttdtqwapt.html

Java: // 手写 HashMap
来源：http://hz.vqdsnc.cn/gtafwejqae.html

Go:   // 手写 map[int]int
来源：http://hz.tanke756.top/gtujavmrgy.html

Ruby: // 手写 Hash
来源：http://hz.gogol.net.cn/gtbyglsqxf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daria6918.cn/gtbkcktcly.html

[N08] 生成全排列
来源：http://hz.aizwys.cn/gtfjonjdsn.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtqrmeemyd.html

PHP:  // 手写递归交换
来源：http://hz.hfpthk.cn/gtynchfdyi.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtkycbwtpb.html

TS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtfijluyus.html

Java: // 手写回溯递归
来源：http://hz.snrcjt.cn/gtlhdmjjkp.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtpnefwgca.html

Ruby: arr.permutation.to_a
来源：http://hz.jyoumei.cn/gtudfoyqay.html

C#:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtgxbdxyus.html

[N09] 栈与队列
来源：http://hz.jinqigfzy.top/gthdewjbiu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.bjfxy.top/gtwewhwhyo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gtsgsmomyl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fzhhl.top/gtdtqaeyyz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gaohongyu789.top/gtjooirijl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gaohongyu789.top/gtmcecdett.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.kuanghao11.cn/gtywprwkva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gthcatekof.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.svipenyu.cn/gtcxxfivzt.html

[N10] 链表节点定义
来源：http://hz.guannengcc.top/gtarwswxdl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.haohaochexian.top/gtjykmzvwr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgufenzy.top/gtbmswetwg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenlongwang.top/gtglktideu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuanzx.com/gtqcsuaisw.html

Java: class Node { int v; Node next; }
来源：http://hz.svipenyu.cn/gtenekaeys.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gthisdjiti.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangdashe.top/gtnsyxuwrh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.c1oappe.top/gtitrsncjm.html

[N11] 二叉树中序遍历
来源：http://hz.guowangkeji.top/gtdtojsibp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtuujwqoyg.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gtczvqbcpp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtrixelggu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtzogxmoea.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtbukajjih.html

Go:   // 手写递归
来源：http://hz.hammf.cn/gtlpbffcmk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgufenzy.top/gtjndsciel.html

C#:   // 手写递归
来源：http://hz.aizwys.cn/gthjqaoeqg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jyoumei.cn/gtjkpwthlh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gtfmkzeakf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhiwuduotai.top/gttjmrrztt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtpumpwfbk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gtlaiojokr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jianghu66.top/gtjczwnvda.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtgcilmsad.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gttvodvgak.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtblfmjwdp.html

================================================================================
来源：http://hz.cdnleiting.top/gtfqhsxrbl.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtcmjdcmfe.html

================================================================================
来源：http://hz.jlsjyb.cn/gtferidbqh.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gtjsqjxvbu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangshuangyany.cn/gtlqxypunk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cqqwz.cn/gtpbjsvxdb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gttjhufvaa.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gtvfvmoufg.html

Java: new Thread(() -> f()).start()
来源：http://hz.cucudq.cn/gtojbluout.html

Go:   go f()
来源：http://hz.nwbrower.top/gteqsvuugl.html

Ruby: Thread.new { f }
来源：http://hz.jianghu66.top/gtmnloafea.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtnwttpwqd.html

[O02] 使用线程池
来源：http://hz.gogol.net.cn/gtwmnlkcpk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.fzhhl.top/gtgeuxbnsb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.mhx1999.top/gtdvpmgrec.html

JS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtzbmdveed.html

TS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtfqzfnrov.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.c1oappe.top/gtgynlqqck.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.svipenyu.cn/gtuwssppol.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.mhx1999.top/gtfwjvdlvc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sweek.top/gtfjrcrfzm.html

[O03] 加锁保护共享数据
来源：http://hz.chenjidiqi.icu/gtqqakxkwj.html

Py:   with lock: shared += 1
来源：http://hz.ydjk.org.cn/gtxwmcuqyq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cqqwz.cn/gtidylnplq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gtdreomrlk.html

TS:   // 同 JS
来源：http://hz.jiagoushi.top/gtsfbyytgu.html

Java: synchronized (this) { shared++; }
来源：http://hz.9152youxi.cn/gtfhnhbrfe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtdnulskou.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtahlgirqe.html

C#:   lock (gate) { shared++; }
来源：http://hz.zycfv.cn/gtuoqgofuc.html

[O04] 定义异步函数并等待
来源：http://hz.zhoulong.xyz/gtsueapnlq.html

Py:   async def f():⏎    await g()
来源：http://hz.xuetiantiany.cn/gtksewdgtl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtcmlysdxz.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gtnwcpwvly.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sweek.top/gtqgqbssug.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhijiandao.cn/gtfbazuaim.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guowangkeji.top/gtnibzpgny.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jyoumei.cn/gtkkudurxw.html

C#:   async Task F() { await G(); }
来源：http://hz.316326.xyz/gtjvmlwmcc.html

[O05] 并发执行并等待全部完成
来源：http://hz.aibaodan.cn/gtuiepzafv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtqhsvcyfo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yongpay.top/gtcxpeaqgs.html

JS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtgjnjmzuc.html

TS:   await Promise.all(tasks)
来源：http://hz.daxiang520.top/gtkvrcintn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtewoqedpi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shuidangran.top/gtmdjxfgzv.html

Ruby: threads.map(&:join)
来源：http://hz.sufxvd.cn/gtvmhsaulv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tanke756.top/gtiwhogitb.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtbgulckhq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.snrcjt.cn/gtyiatmdum.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtaxmaknox.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtrtlvjtjb.html

TS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gtsszsvzor.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhoulong.xyz/gtaugramjc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gtelpmqblt.html

Ruby: // fork 块
来源：http://hz.zhixingplan.top/gtrtutvrqt.html

C#:   Parallel.For
来源：http://hz.hfpthk.cn/gtsajcxzbn.html

================================================================================
来源：http://hz.zhengqikj.top/gtrjqgcypp.html

P. 常用工具函数
来源：http://hz.zhijiandao.cn/gtfbfurpev.html

================================================================================
来源：http://hz.fengsongda.top/gtdqlilbwk.html


<!-- 参考信息 -->