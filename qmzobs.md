代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangkeji.top/gtxicklrbw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtdkdgnwbh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.mhx1999.top/gttccwargs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtdwjutmqv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtvpgqszhm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj202588.top/gtcqnozjep.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hammf.cn/gtlpgpvuky.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.smart0.xyz/gtnllubpdv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.redwolf501.top/gtnsaqimbc.html

[L04] 设置超时
来源：http://hz.svipenyu.cn/gtwmehggqq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtujfewfwg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gtljsuqwml.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtpbyxsztz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtceotsqyu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtmtlobrzf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.havefunace.top/gtbiyfaqvt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtptdhrkzg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tianlin.xyz/gtjzykanzp.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtxdkhxalt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.haohaochexian.top/gtnkwppnvm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.birdmap.top/gteoogwrbh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtvjbjvimg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtownncywm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtzbtoganw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tanke756.top/gtxehlhwui.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhengqikj.top/gtbxanqflo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shuidangran.top/gtaafpblrx.html

[L06] 解析响应为 JSON
来源：http://hz.haohaochexian.top/gtwulajrco.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtretktggp.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtjmzzawla.html

JS:   await resp.json()
来源：http://hz.havefunace.top/gtddchpyin.html

TS:   await resp.json()
来源：http://hz.9152youxi.cn/gtuashpftv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtrihtqspb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtplnuorxq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xziqi.cn/gthgmqxruj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hysaishi.cn/gtfasogdyc.html

[L07] 处理 HTTP 状态码
来源：http://hz.xinyue.icu/gtpsjalbnc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.bjfxy.top/gtcrilahzu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zdqjudy.top/gtvupmajwq.html

JS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtlqhxzsum.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangkeji.top/gtmogepffo.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtofartxtj.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtmnetdmak.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtwntesosi.html

C#:   (int)resp.StatusCode
来源：http://hz.gaohongyu789.top/gteqlmkcoe.html

[L08] 并发请求多个地址
来源：http://hz.xylfe.cn/gtdgccakgq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtdsgkyaae.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtmgylayrc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtwzvatwus.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtvrwlwzwk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtewphxgob.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtlktbgxui.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtjprahcqm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gtjbmrgdaj.html

================================================================================
来源：http://hz.zdqjudy.top/gtixlnhmzb.html

M. 命令行 / 进程 / 环境
来源：http://hz.cheryme.top/gtkgwazfoq.html

================================================================================
来源：http://hz.birdmap.top/gtmadmdhki.html

[M01] 读取命令行参数
来源：http://hz.hongshengwenyu.top/gtduspxuwk.html

Py:   sys.argv[1:]
来源：http://hz.yonumen.top/gtmhwjghbc.html

PHP:  $argv;  $argc;
来源：http://hz.tanke756.top/gtzzqebijt.html

JS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtxjyyvmzo.html

TS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtpmcabyfv.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtpbwmmrxv.html

Go:   os.Args[1:]
来源：http://hz.shuidangran.top/gtnfbrwuyv.html

Ruby: ARGV
来源：http://hz.jinqigfzy.top/gtykwnkfus.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtzjakctji.html

[M02] 读取环境变量
来源：http://hz.shuidangran.top/gthbpuclrt.html

Py:   os.environ.get("HOME")
来源：http://hz.jlsjyb.cn/gthzrwbqqn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cqqwz.cn/gtyookculw.html

JS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gthimtzqoc.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtsoudxjye.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtlgluvwez.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtdsecocev.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gtdjrsywmw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtveijuxuw.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtymfzmokf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtrmzjmbwn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pycfn.com/gtthywqxtu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtlpraozlv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtwpsyeajn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj202588.top/gtnktqmhno.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fengsongda.top/gtlzozmbnf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtybmuyeva.html

C#:   Process.Start("ls", "-l");
来源：http://hz.snrcjt.cn/gtciucmfyj.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtgdsoqrwx.html

Py:   os.getcwd()
来源：http://hz.zycfv.cn/gtjoyxwkvj.html

PHP:  getcwd();
来源：http://hz.chenzaomai.com/gtjsmienfe.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtdtdpjomx.html

TS:   process.cwd()
来源：http://hz.sufxvd.cn/gtyrwagxoj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.quarkkingdee.top/gtpaibwluv.html

Go:   os.Getwd()
来源：http://hz.vqdsnc.cn/gtmedccega.html

Ruby: Dir.pwd
来源：http://hz.sxryk.cn/gtwuzggfhl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtrvqfbefv.html

[M05] 设置退出码
来源：http://hz.pengpengdd.cyou/gtvxoylsxx.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtdaklqpul.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gtcvehwcwi.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gtktkwjwqt.html

TS:   process.exit(1)
来源：http://hz.guannengcc.top/gtanrobzfs.html

Java: System.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtkydqhfly.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtdqplkqmf.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gthzhqbmdw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtcytztfog.html

[M06] 向标准错误输出
来源：http://hz.aizwys.cn/gtschotxpa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gtexlvdngk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtqvhysoro.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtgkezfkia.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gtfwlbwnzy.html

Java: System.err.println("err")
来源：http://hz.gzhubu.top/gtgvjymeaf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gttbjjatou.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gttpfpgmfp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gaohongyu789.top/gtafookvvj.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtmpiktlvj.html

Py:   if __name__ == "__main__":
来源：http://hz.vqdsnc.cn/gtxohloejk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtgvlfjayg.html

JS:   require.main === module
来源：http://hz.xylfe.cn/gtdrafqkqt.html

TS:   require.main === module
来源：http://hz.sweek.top/gtvavrytob.html

Java: public static void main(String[] args)
来源：http://hz.ppjwa.cn/gttvytmlnv.html

Go:   func main()
来源：http://hz.ivvv.top/gttetqrals.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cucudq.cn/gtbwujsvyk.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gtboidtdvb.html

[M08] 获取系统与运行时信息
来源：http://hz.aizwys.cn/gtqlmegbtt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhixingplan.top/gtitdkwufg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gtrjkcrzjs.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtdmyvskwn.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtzkugfwfv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yonumen.top/gtruuzbbib.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenjidiqi.icu/gtbohozxbt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xingfuxueyuan.xyz/gtsxbwokmi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtobcscwcx.html

================================================================================
来源：http://hz.c1oappe.top/gtosrvxucv.html

N. 数据结构与算法
来源：http://hz.yvedp.cn/gtkqnrncdn.html

================================================================================
来源：http://hz.yj202588.top/gttvwclcar.html

[N01] 二分查找（有序数组）
来源：http://hz.xuetiantiany.cn/gtpbfuckjz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtcizqphpn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtqkpgzztc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtusrldmxd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtnwnjvtrm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gtdyvqrvao.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtsmcpygcj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zycfv.cn/gtoqnpvscf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtwtonneqf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtffbqbsma.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yongpay.top/gtlqfpkfoa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenjidiqi.icu/gtdeuwltoo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtriukglpg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtkeutqewo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtmeeqfwnb.html

Go:   slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtlrbxlmjb.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtxgfxtkyx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtbrequjbj.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigfzy.top/gtxohlxljx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hfpthk.cn/gtasbfnfhf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydjk.org.cn/gtavcnbiex.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtfhqrjgyy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtloijdyac.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuetiantiany.cn/gtfwqydokg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtycjvcywq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhixingplan.top/gtpkyhvsvp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258888.top/gtggqonvsx.html

[N04] 斐波那契数列
来源：http://hz.mhx1999.top/gtobcnuexr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtmkrabgns.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shuidangran.top/gtakqlibhz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtfnthjich.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtpyfabrwo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtgymalmfg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenjidiqi.icu/gtikyqbwyn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtojaktcfh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhixingplan.top/gtyrcgxsus.html

[N05] 最大公约数
来源：http://hz.kuanghao11.cn/gtwzxtrpap.html

Py:   math.gcd(a, b)
来源：http://hz.feifeiyinyue.top/gtuonceprw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cqqwz.cn/gtnohimopc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtksfnwelx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtzcewpzpi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shzxlz.cn/gtzdchpupk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.9152youxi.cn/gtwzslfpzg.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtqlflrabk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtkgjrhqrq.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtojtezopy.html

Py:   s == s[::-1]
来源：http://hz.zhiwuduotai.top/gtizwbgcyf.html

PHP:  $s === strrev($s);
来源：http://hz.0kj1m.cn/gteuyuzwcp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtemvftutn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtoeypqctc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gtlxfkxfsn.html

Go:   // 双指针从两端比较
来源：http://hz.chenjidiqi.icu/gtquutanpa.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtsdnqetrf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtetmytqwn.html

[N07] 两数之和（返回下标）
来源：http://hz.vqdsnc.cn/gtngwzidry.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sxryk.cn/gtjrjkugwr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.9152youxi.cn/gtouacuslr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.0kj1m.cn/gtxvwanija.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gtelikujqx.html

Java: // 手写 HashMap
来源：http://hz.shzxlz.cn/gttdhataje.html

Go:   // 手写 map[int]int
来源：http://hz.svipenyu.cn/gtejfmdqas.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gtkuhnhxsh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangshuangyany.cn/gtwrchhkzd.html

[N08] 生成全排列
来源：http://hz.dashuyun.cn/gtkijdpflr.html

Py:   itertools.permutations(arr)
来源：http://hz.xuetiantiany.cn/gtezgsxibp.html

PHP:  // 手写递归交换
来源：http://hz.cashguo.top/gtdzakaxva.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gttlhiqqtl.html

TS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtoveqfvfv.html

Java: // 手写回溯递归
来源：http://hz.nanxinkj.top/gtxlgrjtus.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gturvbafdx.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258888.top/gtkizruome.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtkfqpjfrb.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtkdbwnpgz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hnxiangtu.top/gtqqessnsa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.9152youxi.cn/gtoyfvvigl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtjprmzwtr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gtxtmchquh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtfykyyyxv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yangfankeji.com/gtfgutnqte.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.c1oappe.top/gtyhzejfaz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jqgfzy.top/gtxatuufui.html

[N10] 链表节点定义
来源：http://hz.zhixingplan.top/gtbqpvcfev.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gtfxwatuzp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhengqikj.top/gtwnpatqjk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gtsownwbjg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258.top/gtphmjzffn.html

Java: class Node { int v; Node next; }
来源：http://hz.kuanghao11.cn/gtqzpwudbs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hongshengwenyu.top/gtuelxgpyy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gtcalcvtef.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gthhanojtf.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtucjdduur.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangdashe.top/gtycapzzxa.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtargmgraa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtvlflsgaw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtaxvjsbaf.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gtfasybdrr.html

Go:   // 手写递归
来源：http://hz.jianghu66.top/gtwagakopm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pengpengdd.cyou/gtomzzwltx.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gthzhmkaoo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258.top/gtfsbvypel.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxinkj.top/gtbinfryct.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hfpthk.cn/gtdomuewxk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gthpszgafk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtjsdsplay.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnqzz.top/gtnxjerqhp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sufxvd.cn/gtvpjmyxkp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gthtjavvjl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtcvrkzmhv.html

================================================================================
来源：http://hz.yj20258.top/gtrfdacfze.html

O. 并发与异步
来源：http://hz.cheryme.top/gtyichpqwk.html

================================================================================
来源：http://hz.dashuyun.cn/gtaxanedcr.html

[O01] 启动一个线程
来源：http://hz.sxryk.cn/gtxgiyvxip.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.316326.xyz/gtoeqtwnre.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.andypj.xyz/gtymqhknou.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtqliybkrl.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtnkyjsvan.html

Java: new Thread(() -> f()).start()
来源：http://hz.shzxlz.cn/gtyrqoyfab.html

Go:   go f()
来源：http://hz.aizwys.cn/gtkdojsezy.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtlfxcpwnf.html

C#:   Task.Run(() => F());
来源：http://hz.cheryme.top/gtswbqzhre.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gtqckrqytt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.birdmap.top/gtvptivjjp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hnqzz.top/gtwftobbgc.html

JS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtmooltydg.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtcsnbtawk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.kuanghao11.cn/gtvlgajjni.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yvedp.cn/gtnbbsgshs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgfzy.top/gtdpnluodd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sxryk.cn/gthwrqktuu.html

[O03] 加锁保护共享数据
来源：http://hz.hfpthk.cn/gtezbbkgyq.html

Py:   with lock: shared += 1
来源：http://hz.nwbrower.top/gtlsuydwna.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinghuilouyu.cn/gthsicjtoz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenlongwang.top/gtoolatcxm.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gttaqedany.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtaywwwvgr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yanxiufei.cn/gtuiqjxvyk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuxming.cn/gtuankpqmc.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxinkj.top/gtengqbush.html

[O04] 定义异步函数并等待
来源：http://hz.aibaodan.cn/gtghamynvc.html

Py:   async def f():⏎    await g()
来源：http://hz.ehwqpu.com/gtnmmkzvfy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenlongwang.top/gtuavmwvak.html

JS:   async function f() { await g(); }
来源：http://hz.snrcjt.cn/gtapxfdsab.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtihnknlqe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtqxyryhwv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.andypj.xyz/gtekzwpeiz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gtvcfzayet.html

C#:   async Task F() { await G(); }
来源：http://hz.ivvv.top/gtsynaoxiq.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtirpcbttl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aibaodan.cn/gtojwppfzr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ehwqpu.com/gtvuiffotu.html

JS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtrahadvwl.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtbveedrwi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtrsngvbic.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.feifeiyinyue.top/gtzqyvciwc.html

Ruby: threads.map(&:join)
来源：http://hz.kuanghao11.cn/gtnqglolmw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yangfankeji.com/gtkwjrcnrx.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtjvdgioww.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtjgwaujjx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guannengcc.top/gtmwhzcfsw.html

JS:   // child_process / cluster 模块
来源：http://hz.yj20258.top/gtwazbsxni.html

TS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtysoengyd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gtdcechvmz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ivvv.top/gtsirprnqo.html

Ruby: // fork 块
来源：http://hz.pycfn.com/gtbbnexlsa.html

C#:   Parallel.For
来源：http://hz.cheryme.top/gtwxfnnyfa.html

================================================================================
来源：http://hz.gotoacloud.top/gtbcahaisc.html

P. 常用工具函数
来源：http://hz.cheryme.top/gtrsbnymew.html

================================================================================
来源：http://hz.hammf.cn/gtlfsksmyn.html


<!-- 参考信息 -->