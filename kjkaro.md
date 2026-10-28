代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258.top/gtmjbjcxko.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gtycupypwk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtrpspxjrj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtkbpvytcs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fengsongda.top/gtlhjaohsx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtcxuprlca.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gzhubu.top/gtnmmlcxss.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gtaqwcezat.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gtfwsdyefy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gtbtsiylar.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ppjwa.cn/gtwfstqgad.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gttyiizwbl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtonfloeyj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aizwys.cn/gtnbnovtxl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtinntwlfa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtlftgwqmq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtwmtkcrmz.html

[L04] 设置超时
来源：http://hz.cdnleiting.top/gthaibnpde.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gtgaatlbaj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xingfuxueyuan.xyz/gtxwhdnouo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gtbsmytsqn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gthkhklkwi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtbqhydduf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtoywvladz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gtgxwenhry.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtpoqyeorz.html

[L05] 上传文件（multipart）
来源：http://hz.pycfn.com/gtyadtwbva.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtcbaoyjhj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zdqjudy.top/gtaikeabrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtcyvbemot.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtrmkctzyl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gtpsjobawo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtjyqmzuqk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.iojbl.cn/gttnkbktkz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.feifeiyinyue.top/gtvjakqxzk.html

[L06] 解析响应为 JSON
来源：http://hz.fengsongda.top/gttbjxjspw.html

Py:   resp.json()
来源：http://hz.chenzaomai.com/gtnzgejvdc.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigfzy.top/gthwyllcly.html

JS:   await resp.json()
来源：http://hz.9152youxi.cn/gtivansbsx.html

TS:   await resp.json()
来源：http://hz.gotoacloud.top/gtfqcqtgly.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtopfwnmpt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtqbrgvobt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtemxiwwfk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tanke756.top/gtrlxuvunu.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gthpkriynq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guowangkeji.top/gtnvncdmut.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.bjfxy.top/gtnbpttswa.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtmbidcjcb.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtmzpmznsk.html

Java: resp.statusCode()
来源：http://hz.zhixingplan.top/gttfywhcdw.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gtmaktemkh.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gtzjftddsq.html

C#:   (int)resp.StatusCode
来源：http://hz.xuanzx.com/gtsgcttirz.html

[L08] 并发请求多个地址
来源：http://hz.pycfn.com/gtserwtypx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.svipenyu.cn/gtqgghvziv.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxuanxn.top/gtzqbraucy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtbvfuhala.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtlzeixpch.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jyoumei.cn/gtmfsbzsxo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jlsjyb.cn/gtxoxxpcfn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.52xcode.cn/gtvxyqxxkp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgfzy.top/gtbakxaofj.html

================================================================================
来源：http://hz.hnqzz.top/gtaaxnwhxi.html

M. 命令行 / 进程 / 环境
来源：http://hz.nwbrower.top/gtjubbkztq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjcibfwlr.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtgraepekx.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gttvleofbo.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtvmxtibxw.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gthsphceqh.html

TS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtxlpaytxe.html

Java: args 数组（main 方法参数）
来源：http://hz.jianghu66.top/gtrefgeepe.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtkjthxaaq.html

Ruby: ARGV
来源：http://hz.xinyue.icu/gtrpgrhegy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtrngjoyxs.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtklkxosoo.html

Py:   os.environ.get("HOME")
来源：http://hz.gaohongyu789.top/gtovehkulk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtwkrnzswr.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtuldvwviq.html

TS:   process.env.HOME
来源：http://hz.xuetiantiany.cn/gteyhjajhy.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gteoiinjbq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ppjwa.cn/gtywejgohj.html

Ruby: ENV["HOME"]
来源：http://hz.bjfxy.top/gtwhpyvwvq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258888.top/gtpbvgehmo.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtpawqhpir.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hongshengwenyu.top/gtgvlpttht.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ehwqpu.com/gtbihsthfs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtbwffcxwt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtqwecfpbj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtzkdfbhdb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gtjjpdsjdo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gthptqckkw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtvmlspykg.html

[M04] 获取当前工作目录
来源：http://hz.ppjwa.cn/gtwirftypa.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtggojwnil.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtmubyplzz.html

JS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtkjpqqyid.html

TS:   process.cwd()
来源：http://hz.dashuyun.cn/gtshkvfiin.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cheryme.top/gtmdsjyrlm.html

Go:   os.Getwd()
来源：http://hz.yonumen.top/gtmtwwncza.html

Ruby: Dir.pwd
来源：http://hz.cashguo.top/gtmitcfeom.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuxming.cn/gtecwczekn.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtoiirsnos.html

Py:   sys.exit(1)
来源：http://hz.jinghuilouyu.cn/gthdgdmzrx.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtfzywlzsm.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtiaaqfodf.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtzontzfdb.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtmaemnjve.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtdldmhlpr.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gtsgqavnry.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hywenlv.cn/gtjvgnlvyl.html

[M06] 向标准错误输出
来源：http://hz.yvedp.cn/gtfzpdmcik.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydjk.org.cn/gtgvysvils.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wangdashe.top/gttozqikdm.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtnvcxkqlt.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtrjbmiiar.html

Java: System.err.println("err")
来源：http://hz.c1oappe.top/gtyskqpohi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtlwklkzfb.html

Ruby: warn "err"
来源：http://hz.yueranfly.top/gtvfecvkml.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.redwolf501.top/gtbcsltwdx.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtzhjtruui.html

Py:   if __name__ == "__main__":
来源：http://hz.mhx1999.top/gtncuxggph.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.c1oappe.top/gtjqcdgfym.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtykejhean.html

TS:   require.main === module
来源：http://hz.ydzc1.top/gtmleirxzc.html

Java: public static void main(String[] args)
来源：http://hz.cashguo.top/gtbloriyqt.html

Go:   func main()
来源：http://hz.gogol.net.cn/gtlisblnuc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yongpay.top/gtkwfykdcs.html

C#:   static void Main(string[] args)
来源：http://hz.yj202588.top/gtwzaczjce.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtdmqyjsaa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jlsjyb.cn/gtofciqupl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zycfv.cn/gtacirsmhk.html

JS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtutluaytg.html

TS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtvykqxord.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnqzz.top/gtocejcnyy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtounjbhsd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guowangkeji.top/gtxzwgjrzv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinyuanbaomall.cn/gtfdahuyxo.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqvcammiw.html

N. 数据结构与算法
来源：http://hz.zhixingplan.top/gtyeecfuoe.html

================================================================================
来源：http://hz.daria6918.cn/gtbhqerbye.html

[N01] 二分查找（有序数组）
来源：http://hz.redwolf501.top/gtvuihutar.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtnbkgdmrf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtpenftsfb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gthacinpug.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtvzedxjzx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cqqwz.cn/gttsvdfkct.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.guannengcc.top/gttipusuqr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtmjpdviij.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.redwolf501.top/gthjhmxxgd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhengqikj.top/gtkaovznlz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtaigwtsvd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnqzz.top/gtwmtrngur.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtdkuaqcfg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtxbrtgoyo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.mhx1999.top/gtznkqhmrd.html

Go:   slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtgeansjgl.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtgmtrskzx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtaykowgar.html

[N03] 快速排序（分治示例）
来源：http://hz.yj202588.top/gtyxjzptfn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtcvetkrhj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydzc1.top/gtvpwugfgy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtxiqcnqmn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yueranfly.top/gtzulbzlzz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ydjk.org.cn/gttutkajlf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tanke756.top/gtgfyueveb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gtrfjuxywz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ybcxt.top/gtrjdktmvz.html

[N04] 斐波那契数列
来源：http://hz.daria6918.cn/gtoasfzdeh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtaozxxixl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhoulong.xyz/gtgyhzqzqs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtilfgggri.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtyefufaal.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtoheszgbg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydjk.org.cn/gtdehptcly.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtfnivtpte.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.c1oappe.top/gtdzscxwja.html

[N05] 最大公约数
来源：http://hz.ppjwa.cn/gtzrtshbcq.html

Py:   math.gcd(a, b)
来源：http://hz.yvedp.cn/gthleukcqp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinyuanbaomall.cn/gtmdpajccb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtnegmfkqs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtrhvukzyy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhiwuduotai.top/gtmypafkvx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinyuanbaomall.cn/gtyzzmmyvt.html

Ruby: a.gcd(b)
来源：http://hz.ehwqpu.com/gtizaisrot.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ivvv.top/gtbitgtoqt.html

[N06] 判断回文字符串
来源：http://hz.nwbrower.top/gtqpmqeodr.html

Py:   s == s[::-1]
来源：http://hz.yangfankeji.com/gtccuolari.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtyjduiqzc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtxnvqviol.html

TS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtrdvzyzfo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sysykeji.top/gtmzgrifii.html

Go:   // 双指针从两端比较
来源：http://hz.jqgufenzy.top/gtgiavacuj.html

Ruby: s == s.reverse
来源：http://hz.yangfankeji.com/gtybfwttgt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtlytvrlfn.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gtohpaieos.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tianlin.xyz/gtgzelgesq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gtdvdzhafu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cdnleiting.top/gtqwetzbav.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtxbmwkvfx.html

Java: // 手写 HashMap
来源：http://hz.pengpengdd.cyou/gtwvdnesgz.html

Go:   // 手写 map[int]int
来源：http://hz.bjfxy.top/gtsryzvfxa.html

Ruby: // 手写 Hash
来源：http://hz.dashuyun.cn/gtzmmgpgjx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.andypj.xyz/gtkqjxkdau.html

[N08] 生成全排列
来源：http://hz.cheryme.top/gtsipmedvb.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtqevswsqc.html

PHP:  // 手写递归交换
来源：http://hz.zdqjudy.top/gtxwgeykph.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtpqzhojth.html

TS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gthoizfowu.html

Java: // 手写回溯递归
来源：http://hz.gogol.net.cn/gtikgisbcg.html

Go:   // 手写回溯递归
来源：http://hz.sweek.top/gtwqbtncaf.html

Ruby: arr.permutation.to_a
来源：http://hz.shuidangran.top/gtjnszuwab.html

C#:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtaodzqpjd.html

[N09] 栈与队列
来源：http://hz.ybcxt.top/gtifxydpjf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.svipenyu.cn/gtjhpnezdt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xziqi.cn/gtwzlmddvi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtqacqhqhk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yongpay.top/gtpjepeuxy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gttlrrqzrb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258888.top/gtuvmacfym.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuanzx.com/gtxgxymwdd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hongshengwenyu.top/gtghiqdcdq.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtejneysqx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenlongwang.top/gtitbfviax.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xingfuxueyuan.xyz/gtvrehupvx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinghuilouyu.cn/gtgwdpneup.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxinkj.top/gtuiknmjld.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgfzy.top/gtqoyevcxb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xylfe.cn/gtzqdefglq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hammf.cn/gtmnvhzkwt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.daxiang520.top/gtmegyxqdt.html

[N11] 二叉树中序遍历
来源：http://hz.zhoulong.xyz/gtdtuqwgff.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gtqmvtukib.html

PHP:  // 手写递归函数
来源：http://hz.birdmap.top/gtyvawwooz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtrvxlrfwl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gteeuzjmbr.html

Java: // 手写递归
来源：http://hz.shuidangran.top/gtizijnbda.html

Go:   // 手写递归
来源：http://hz.tianlin.xyz/gtebsmkjps.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xylfe.cn/gtntxyggso.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtqmmhbmxw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gtfazzhgvp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258888.top/gtozzlbmgu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.c1oappe.top/gtkilkziku.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtoezqtaht.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtlqhbujox.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtcsplyiwg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hywenlv.cn/gtmrezldiw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gtoaionsnf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtxipeaqky.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtkjgcvzqo.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtlvynexlu.html

================================================================================
来源：http://hz.ybcxt.top/gtmqruyoqg.html

[O01] 启动一个线程
来源：http://hz.wangdashe.top/gtlujmzwnr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangdashe.top/gtdxijxwlg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hongshengwenyu.top/gtxpyrupga.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangdashe.top/gtbnezbavk.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtoqmlwpnr.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gturwakuhy.html

Go:   go f()
来源：http://hz.tanke756.top/gtehqkdnki.html

Ruby: Thread.new { f }
来源：http://hz.zhoulong.xyz/gtgsjcyxen.html

C#:   Task.Run(() => F());
来源：http://hz.aibaodan.cn/gtgtvulekm.html

[O02] 使用线程池
来源：http://hz.hywenlv.cn/gtdyrxrncp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtqiydwdxz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhiwuduotai.top/gtoufsdzoi.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtgruispmm.html

TS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtzwadobjp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.smart0.xyz/gthlniwvof.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.meibo888.top/gtrmlsthgk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hysaishi.cn/gtqjdlsdpn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtllmhquwk.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtchmkwlmg.html

Py:   with lock: shared += 1
来源：http://hz.chenzaomai.com/gtesqmerqz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258.top/gtubiycdzh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhixingplan.top/gthejpdinc.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtfrmilnfz.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydjk.org.cn/gtwpjyiuaa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.vqdsnc.cn/gtoyfjqbqw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cashguo.top/gtgkahdjze.html

C#:   lock (gate) { shared++; }
来源：http://hz.ppjwa.cn/gtighnzacj.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gtkcezebaj.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtbymajzee.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gttgobqyjh.html

JS:   async function f() { await g(); }
来源：http://hz.jianghu66.top/gthyqxwvek.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.feifeiyinyue.top/gtwxirwgea.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hfpthk.cn/gtdhkcszws.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guannengcc.top/gtlxsbqjbo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gtvjixqlbo.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigfzy.top/gtecigugww.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtrmxkmnnj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ybcxt.top/gtnilatvvw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.havefunace.top/gtrrejyelg.html

JS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtdbvjgsad.html

TS:   await Promise.all(tasks)
来源：http://hz.0kj1m.cn/gtzcyopuxm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gtryvwxyuf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xinyue.icu/gthlmtfque.html

Ruby: threads.map(&:join)
来源：http://hz.tianlin.xyz/gtutytecri.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guannengcc.top/gtcasfohqq.html

[O06] 使用进程池
来源：http://hz.aizwys.cn/gtcekqrbae.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guannengcc.top/gtnzazqhxo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangkeji.top/gturanyfxx.html

JS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtvtgdyjum.html


<!-- 参考信息 -->