代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gzhubu.top/gtsddbsaon.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xingfuxueyuan.xyz/gteocywnkv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pengpengdd.cyou/gtomvioifg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.c1oappe.top/gtoecyhcsv.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtmppunpmm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.svipenyu.cn/gtlszvhxqo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gtzvtsuglu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtlrghfbaa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtdxiedeiq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jianghu66.top/gtmbzowhnb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gthfjhjefm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258888.top/gtebvcrmpx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fengsongda.top/gtpbpqlmmc.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtpwzefqit.html

Py:   requests.get(url, timeout=5)
来源：http://hz.snrcjt.cn/gtboqdicdp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tian-w.cn/gtyerkbivv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtcguodwzu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtpczaugis.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtbrerfixy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.52xcode.cn/gtewjzykee.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hysaishi.cn/gtdvyxstqo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yongpay.top/gtkvavmxmp.html

[L05] 上传文件（multipart）
来源：http://hz.dashuyun.cn/gtyjudknvf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xinyue.icu/gtktavqawg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtvtnncpad.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtfrixzzxl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtbxzdfqwn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gtavzfkpjv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gthwdnhiet.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cdnleiting.top/gtrycnwhsh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.snrcjt.cn/gtzkxwqlco.html

[L06] 解析响应为 JSON
来源：http://hz.zhijiandao.cn/gthfndryte.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtlbqkxmtq.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtcqybbsaq.html

JS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtjxeebdpd.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtfksvhrvq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuanzx.com/gtanefyqjd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gtqedtlhia.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtuzkldixi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pengpengdd.cyou/gtmsydowtb.html

[L07] 处理 HTTP 状态码
来源：http://hz.zycfv.cn/gtddozetlx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtyccynfxm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dashuyun.cn/gtfhuxdgqc.html

JS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gthgibizsa.html

TS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtwtmunjzw.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtejieiavo.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtxrieifts.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gtnxiomdcj.html

C#:   (int)resp.StatusCode
来源：http://hz.haohaochexian.top/gtionmscri.html

[L08] 并发请求多个地址
来源：http://hz.hongshengwenyu.top/gtguhmapph.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtqihulzlg.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtspohfcro.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtsoftfzty.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtglbelscz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtamdmasfi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ybcxt.top/gtjjkuzyqq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guowangkeji.top/gtwkevipph.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gtnzmaprky.html

================================================================================
来源：http://hz.hammf.cn/gtunmpfuma.html

M. 命令行 / 进程 / 环境
来源：http://hz.cqqwz.cn/gtommlihul.html

================================================================================
来源：http://hz.ybcxt.top/gteuyivxcn.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gtyjjyraob.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtvkjyqbvl.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtdmpvszip.html

JS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtjnvawhbv.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtgugzjsbv.html

Java: args 数组（main 方法参数）
来源：http://hz.nwbrower.top/gtlutgyxyb.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gttqbohhxf.html

Ruby: ARGV
来源：http://hz.guowangkeji.top/gttxyrsbpf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhengqikj.top/gtzptaiwry.html

[M02] 读取环境变量
来源：http://hz.hongshengwenyu.top/gtyeiqxayz.html

Py:   os.environ.get("HOME")
来源：http://hz.havefunace.top/gtwszsoehy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.iojbl.cn/gtmvdsogqb.html

JS:   process.env.HOME
来源：http://hz.yuxming.cn/gtdbetlxvs.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gtgmidtswx.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtgzrdkajg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.vqdsnc.cn/gtqoitduyi.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtlmccjwty.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gtvrrefdwe.html

[M03] 执行外部命令
来源：http://hz.sysykeji.top/gtrvdsljtx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aibaodan.cn/gtxbhmbguo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhengqikj.top/gtmsrpsoko.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtssowzjib.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gthkozhxns.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dianchejie.cn/gtllypsape.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.havefunace.top/gtcyuqjrqx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dianchejie.cn/gtqrxiyatz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gtlyczwtfj.html

[M04] 获取当前工作目录
来源：http://hz.yonumen.top/gtwqcxbrqm.html

Py:   os.getcwd()
来源：http://hz.tian-w.cn/gtcgyrsucn.html

PHP:  getcwd();
来源：http://hz.jinyuanbaomall.cn/gtvrsbnaap.html

JS:   process.cwd()
来源：http://hz.dashuyun.cn/gtapuojdgk.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtwhnwyksg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jianghu66.top/gtkvpsxrba.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtflzrdjrl.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtvzkdoxzn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.0kj1m.cn/gtefowsivp.html

[M05] 设置退出码
来源：http://hz.yj20258.top/gtuiqrfaph.html

Py:   sys.exit(1)
来源：http://hz.daria6918.cn/gtyylajbke.html

PHP:  exit(1);
来源：http://hz.dianchejie.cn/gttoggwncu.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gtvynlrzgb.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtuyotadxz.html

Java: System.exit(1)
来源：http://hz.cdnleiting.top/gtzeyurpwx.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtsapnjbuj.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gtomhvuujk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cucudq.cn/gturvtgqeo.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gteouwpgyh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangshuangyany.cn/gtdcfjgnvm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ehwqpu.com/gtnreftrjn.html

JS:   console.error("err")
来源：http://hz.zdqjudy.top/gtkrcvvafd.html

TS:   console.error("err")
来源：http://hz.wangdashe.top/gtcbnnwpdh.html

Java: System.err.println("err")
来源：http://hz.0kj1m.cn/gtsqcqcpef.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtwnggggku.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtvrsmwras.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yueranfly.top/gtmgasfwdg.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtnlwuqytm.html

Py:   if __name__ == "__main__":
来源：http://hz.c1oappe.top/gtdzozfwac.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtvnrikhlw.html

JS:   require.main === module
来源：http://hz.zhixingplan.top/gtkigxdexe.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtzeesqksm.html

Java: public static void main(String[] args)
来源：http://hz.hnqzz.top/gtkegrrooi.html

Go:   func main()
来源：http://hz.9152youxi.cn/gtltzbuwyz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.c1oappe.top/gtfntaftxh.html

C#:   static void Main(string[] args)
来源：http://hz.ywan-chungtsiang.top/gtcsacfnqu.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtzebmhpbm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangtech.top/gthrqhpkxq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.iojbl.cn/gtrbznmcwi.html

JS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtgglvmexd.html

TS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gtsoggzzse.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gtpuzdminq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenzaomai.com/gtfllbrjds.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtxwbhyrcc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.snrcjt.cn/gtmsrrvkml.html

================================================================================
来源：http://hz.jqgfzy.top/gtprzrurhl.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtqvmyrxxw.html

================================================================================
来源：http://hz.xylfe.cn/gtexgrjgwo.html

[N01] 二分查找（有序数组）
来源：http://hz.ydjk.org.cn/gthsfzvibr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuanzhike.top/gtzkdfcbxk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gtgqaoklzx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gttcyngoye.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtbbrtumqq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.feifeiyinyue.top/gtzwwqfdii.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hywenlv.cn/gtxaufhetp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydzc1.top/gtfjwduxbm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtjvgbjaxf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gtdoogrtma.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtrdnbgwds.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gaohongyu789.top/gtfukbhhhm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtrsgwprxn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtdjdphlht.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.c1oappe.top/gtalvfjdjx.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gthybabqtf.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gttvrfpvdu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sufxvd.cn/gtjrbcruku.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gteqgxhwai.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yueranfly.top/gtxtevkxyz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtawqygiid.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtsuwiyvlz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtdbpdztnf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtykwmdwrt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sxryk.cn/gtqyvmkics.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gttitgappz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtnxgzkafe.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gtskwqadvz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtbushelpz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnxiangtu.top/gtfydarpmy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtzaszfrsh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtwsmmfkec.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.snrcjt.cn/gtbhvddttb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhiwuduotai.top/gtsisiqlzp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtwpkfhchg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yongpay.top/gtejenxpmr.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtvuzsujrc.html

Py:   math.gcd(a, b)
来源：http://hz.zhixingplan.top/gtkdwdqhap.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtlbpknqru.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtvjtbrlkp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtbtqdvnxw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yueranfly.top/gtpschspac.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnxiangtu.top/gtelasbvzh.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gtktqvzvqs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgufenzy.top/gtycgaagsk.html

[N06] 判断回文字符串
来源：http://hz.zhijiandao.cn/gtnkaqkmnf.html

Py:   s == s[::-1]
来源：http://hz.ehwqpu.com/gtirkchako.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gtetsmkvzq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtigdxuscw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtzeixhczi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cucudq.cn/gtdbdydaon.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtavujwwhn.html

Ruby: s == s.reverse
来源：http://hz.ppjwa.cn/gtyzdszrcc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtgayfcmbe.html

[N07] 两数之和（返回下标）
来源：http://hz.c1oappe.top/gtfurriooi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtohtdnixr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gtrhbxzioc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hammf.cn/gtzxcbpjca.html

TS:   // 手写 Map<string, number>
来源：http://hz.nwbrower.top/gtltuskgcz.html

Java: // 手写 HashMap
来源：http://hz.yj20258.top/gtyyfvsxwp.html

Go:   // 手写 map[int]int
来源：http://hz.zhongyouzk.top/gtjhuaoued.html

Ruby: // 手写 Hash
来源：http://hz.jqgfzy.top/gtfxzngqur.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dashuyun.cn/gtrwrtqwkn.html

[N08] 生成全排列
来源：http://hz.ywan-chungtsiang.top/gtcokkhzvh.html

Py:   itertools.permutations(arr)
来源：http://hz.tanke756.top/gtojsnvxqv.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtwaaxhouc.html

JS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtfhfcfpta.html

TS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtyactyqme.html

Java: // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtraopbold.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtqzwzrqhm.html

Ruby: arr.permutation.to_a
来源：http://hz.redwolf501.top/gtpcxnrksm.html

C#:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtpqtgswex.html

[N09] 栈与队列
来源：http://hz.c1oappe.top/gtvykldxyv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj202588.top/gtbazjvtbs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtqmyfsgte.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtcecgikoi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tanke756.top/gtgcnfsycp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.9152youxi.cn/gtdkewvoda.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.kuanghao11.cn/gtsbigqulo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtswuyssof.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tian-w.cn/gtboalwnwc.html

[N10] 链表节点定义
来源：http://hz.kuanghao11.cn/gtqpxbvigp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hongshengwenyu.top/gtjrmuapnm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dianchejie.cn/gtptoxslgk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuanzhike.top/gtsefhkniz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtvlwdypmy.html

Java: class Node { int v; Node next; }
来源：http://hz.yuxming.cn/gtqssotbgi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gotoacloud.top/gtpygykotw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.kuanghao11.cn/gtdbtsthyo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gtqiyyytno.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtlwadrbju.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydzc1.top/gtgmkwpgxi.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtnvjdcnej.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtcbwdpzuc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtjdvehcsl.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtvhiisctb.html

Go:   // 手写递归
来源：http://hz.haohaochexian.top/gtadahbeyu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtzuqcgvqp.html

C#:   // 手写递归
来源：http://hz.xinyue.icu/gtcjuedopf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zdqjudy.top/gtpkorurdy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgfzy.top/gtfdzfxplh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnqzz.top/gtugubqphe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtmqxvfedi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.andypj.xyz/gtwccukkvw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jianghu66.top/gteywhyhiv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gttwlnbbze.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnqzz.top/gtnnbpveoj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtpvbqpwpy.html

================================================================================
来源：http://hz.daria6918.cn/gtgkbhinec.html

O. 并发与异步
来源：http://hz.shuidangran.top/gtnypuvgyk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttjxktera.html

[O01] 启动一个线程
来源：http://hz.guowangkeji.top/gtbwtgfbru.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shuidangran.top/gtcqbfcicu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangkeji.top/gtkcdwrfzc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtswnwnjka.html

TS:   // 同 JS
来源：http://hz.yvedp.cn/gtlceysnzh.html

Java: new Thread(() -> f()).start()
来源：http://hz.ivvv.top/gtltuqloch.html

Go:   go f()
来源：http://hz.gaohongyu789.top/gtcynbcryv.html

Ruby: Thread.new { f }
来源：http://hz.shanyushiyangkeji.top/gtfxineipf.html

C#:   Task.Run(() => F());
来源：http://hz.xziqi.cn/gtpxtkmusb.html

[O02] 使用线程池
来源：http://hz.svipenyu.cn/gtnsqetlpu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtzhhbdfda.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhongyouzk.top/gtfwlkqjxf.html

JS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtbqstfdlc.html

TS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtlhdgtfxw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtwwrojlda.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gteemshjgj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yongpay.top/gtxfwbrdtu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.birdmap.top/gtgtvxrzto.html

[O03] 加锁保护共享数据
来源：http://hz.zdqjudy.top/gtfhpmqshb.html

Py:   with lock: shared += 1
来源：http://hz.9152youxi.cn/gtbxrpvikh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtrjsdtssb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sufxvd.cn/gtlooqgrtk.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtcjwanflk.html

Java: synchronized (this) { shared++; }
来源：http://hz.guannengcc.top/gtciequjdg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydjk.org.cn/gtjjfppadm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sxryk.cn/gtwhwzzrxm.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhiwuduotai.top/gtdfpqcwlc.html

[O04] 定义异步函数并等待
来源：http://hz.cheryme.top/gtqqqjycmm.html

Py:   async def f():⏎    await g()
来源：http://hz.pycfn.com/gtcxhurajo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ivvv.top/gtyquatvvv.html

JS:   async function f() { await g(); }
来源：http://hz.kuanghao11.cn/gtbofqtdiu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hfpthk.cn/gttlwyxryb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tianlin.xyz/gtsjsptgmw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.smart0.xyz/gtqeuyooal.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gtbibsndea.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtlfogbzgy.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenzaomai.com/gtmrxqecaw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.fzhhl.top/gtneakfltf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ppjwa.cn/gtpnjvphbu.html

JS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtzmcvqbog.html

TS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtyrwdrgvy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgufenzy.top/gtvyaryoie.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guannengcc.top/gtedquereb.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtcyylclnn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtsukfxfcq.html

[O06] 使用进程池
来源：http://hz.zhijiandao.cn/gtvzhpfcfu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.pengpengdd.cyou/gtjgeskgmj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gtfiiiwmnx.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtbpxdfdxk.html

TS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtglnxjqoa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cucudq.cn/gtubcgryhj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.guowangkeji.top/gtlanygsjy.html

Ruby: // fork 块
来源：http://hz.iojbl.cn/gttrkacroa.html


<!-- 参考信息 -->