代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gtgtmikyqq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gtflsmoyxk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtplfuqtmz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtlvzfjyyi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuetiantiany.cn/gtgzkclybz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtwyxegfhp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.haohaochexian.top/gtorsylhow.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtowurblyo.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gtqhskildw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gtotwqmrfo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydzc1.top/gtdatoutrn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtxmnvtvoy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtxfgulazz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtzmjnvrol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtlkqjzwpm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtkkumsbnd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fengsongda.top/gtpxicbquy.html

[L04] 设置超时
来源：http://hz.xziqi.cn/gtxikygdxv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxuanxn.top/gtjqjdrifu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenjidiqi.icu/gtvpcuqhrw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtxtmotaew.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gthglvvwed.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yangfankeji.com/gtbjpsfvnf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.kuanghao11.cn/gtihhhcieh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtmcoagfwd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.mhx1999.top/gtrwcbmkxk.html

[L05] 上传文件（multipart）
来源：http://hz.nanxuanxn.top/gtjuknbguc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtzbdhdjir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtdsmckoio.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtgdnjhtin.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtsigngnit.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtmkqlabvd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.smart0.xyz/gtwmoyvorn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtdcyroadv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hammf.cn/gtfrxvgkbi.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtovnjmizu.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtzpxznulo.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtreutxijb.html

JS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gteegfmzsd.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtahdxdutd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cheryme.top/gtugnktmjw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tianlin.xyz/gtapjinfdm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gthstdoufn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cucudq.cn/gtkvgdgyzy.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gtuurfqntl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jyoumei.cn/gtatgnqaum.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gtrxsntjfj.html

JS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtvxmlfwqt.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtmwjnwnnd.html

Java: resp.statusCode()
来源：http://hz.xinyue.icu/gtqmbefopf.html

Go:   resp.StatusCode
来源：http://hz.hnxiangtu.top/gtxxhqxruz.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtewapxqlm.html

C#:   (int)resp.StatusCode
来源：http://hz.shuidangran.top/gtsjdpoyzr.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtmiehjgzq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258888.top/gtehhexvqy.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gtlzhekjub.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtlyoainox.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtrojhxuom.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.iojbl.cn/gtktcntjxv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shuidangran.top/gtxtlpzpcp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtpqpszlzm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gtkvejizhb.html

================================================================================
来源：http://hz.haohaochexian.top/gtpuuuvazo.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtwrfcnibv.html

================================================================================
来源：http://hz.hammf.cn/gtsoxgvgjn.html

[M01] 读取命令行参数
来源：http://hz.mhx1999.top/gtewqwaxkx.html

Py:   sys.argv[1:]
来源：http://hz.jiagoushi.top/gtrjgqdbyk.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtoqivrlxs.html

JS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtaqmwwlms.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gttkjulxjp.html

Java: args 数组（main 方法参数）
来源：http://hz.aibaodan.cn/gtvgozjtxx.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtblppblub.html

Ruby: ARGV
来源：http://hz.guowangkeji.top/gtecisyicf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gttxyomoji.html

[M02] 读取环境变量
来源：http://hz.tianlin.xyz/gttwrvzysw.html

Py:   os.environ.get("HOME")
来源：http://hz.gzhubu.top/gtyldvmumf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gtdrfdatlz.html

JS:   process.env.HOME
来源：http://hz.sxryk.cn/gtrgpxliif.html

TS:   process.env.HOME
来源：http://hz.iojbl.cn/gtnrmeoxlp.html

Java: System.getenv("HOME")
来源：http://hz.snrcjt.cn/gttsxmeden.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtfkgheeds.html

Ruby: ENV["HOME"]
来源：http://hz.fengsongda.top/gtlgihouen.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtfpmybafy.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gttmgvygho.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nwbrower.top/gtemiklgll.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pengpengdd.cyou/gtlsgtquyo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtvwvaxoip.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gthmgcubos.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xinyue.icu/gtpcknhcms.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yvedp.cn/gtdkuhavcj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtwdttbsnp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yongpay.top/gtezwmqyyo.html

[M04] 获取当前工作目录
来源：http://hz.shuidangran.top/gtstmqmwrj.html

Py:   os.getcwd()
来源：http://hz.jinyuanbaomall.cn/gtqqjktkxn.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtpbekgtkp.html

JS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtceewglxq.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtdfgmftak.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydzc1.top/gtudscmkza.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gtogwbxvpp.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gtigegocmh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgufenzy.top/gtveqfhncu.html

[M05] 设置退出码
来源：http://hz.zhengqikj.top/gtgwatsqih.html

Py:   sys.exit(1)
来源：http://hz.zhixingplan.top/gtfxqrkbli.html

PHP:  exit(1);
来源：http://hz.bjfxy.top/gtkxbhoasv.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtgeffchbe.html

TS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtgbvmpqkw.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtcarnydod.html

Go:   os.Exit(1)
来源：http://hz.jlsjyb.cn/gtdiediqnf.html

Ruby: exit 1
来源：http://hz.yueranfly.top/gtbakylvte.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yonumen.top/gtiwvajzts.html

[M06] 向标准错误输出
来源：http://hz.quarkkingdee.top/gtpcfycyzm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtydpzhtxz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.feifeiyinyue.top/gtrqogqgwx.html

JS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtjalrxths.html

TS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtidtpetoc.html

Java: System.err.println("err")
来源：http://hz.fengsongda.top/gtjipynnsb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtxoevqwmq.html

Ruby: warn "err"
来源：http://hz.xuetiantiany.cn/gtlazegwmn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtymdgqhke.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gteuydgtjm.html

Py:   if __name__ == "__main__":
来源：http://hz.sysykeji.top/gtljjnierk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hysaishi.cn/gtsoytohhz.html

JS:   require.main === module
来源：http://hz.jinqigufen.top/gtnfgkfcdj.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gtlugnsvos.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtgoriqnmc.html

Go:   func main()
来源：http://hz.tianlin.xyz/gtmnfwzawo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sxryk.cn/gtnijxnevh.html

C#:   static void Main(string[] args)
来源：http://hz.zhixingplan.top/gtctvvumhm.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gtpsbjwcaj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gthvchzamf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gtbbxpwfms.html

JS:   process.platform;  process.version
来源：http://hz.yuxming.cn/gtmqzurvlz.html

TS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtoewyxjch.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aibaodan.cn/gtlskvrrwz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuxming.cn/gtpzbqujen.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtppwvtiuz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aizwys.cn/gtgacgnasn.html

================================================================================
来源：http://hz.xziqi.cn/gtfhwbckec.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtrohamasj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtplteqcxq.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gthftcxxsr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtftobgzgl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.vqdsnc.cn/gtfncriswj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtfrbrzmta.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtwnexnalc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yonumen.top/gthugzfxen.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtbcoecpcg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtvcsmccrs.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtvauuwicn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gaohongyu789.top/gtwvzscyyk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtwvercmsi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aizwys.cn/gtcvcxpiqg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtmqxyihnx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtixfqcfpu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gtcxeknkrv.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtyilqryyj.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtdiviohfo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gtogjeaioz.html

[N03] 快速排序（分治示例）
来源：http://hz.xylfe.cn/gtdnaorotb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigufen.top/gtmpwreiai.html

PHP:  // 递归实现，或用 usort
来源：http://hz.0kj1m.cn/gtfnldchdu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtmpjslvkl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gttcyviere.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.kuanghao11.cn/gtyejciexi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xinyue.icu/gtwrdaztvg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgufenzy.top/gtxwacjrqb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xylfe.cn/gtxzgarutr.html

[N04] 斐波那契数列
来源：http://hz.zhengqikj.top/gtijbjqamd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtkmpfdvqt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtiyioisvx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtsalxkhnn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gogol.net.cn/gtendjbzzg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gotoacloud.top/gtwccblate.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.iojbl.cn/gtsouczomz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtzbzpgnva.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtaxbyythj.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gtgncbqunf.html

Py:   math.gcd(a, b)
来源：http://hz.c1oappe.top/gtkahdwrjw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hfpthk.cn/gtfryhjvtv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtawkiiqkx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtcikjfues.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gtwgpybrrs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtxmpfbdkv.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtxiecfthg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jyoumei.cn/gtocuythpn.html

[N06] 判断回文字符串
来源：http://hz.zhengqikj.top/gtamacvrcq.html

Py:   s == s[::-1]
来源：http://hz.fengsongda.top/gthwltdaoi.html

PHP:  $s === strrev($s);
来源：http://hz.gaohongyu789.top/gtkulxafgl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtudorhwge.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtgyelhbnv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.52xcode.cn/gtpjaevfhn.html

Go:   // 双指针从两端比较
来源：http://hz.guannengcc.top/gtqvqlgytc.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtikjtheyt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtfgogmbis.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtbjxmvtql.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtfxrzdccl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhixingplan.top/gtbxwmftpc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.svipenyu.cn/gtdptetmdb.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtfbuutxpa.html

Java: // 手写 HashMap
来源：http://hz.jinqigfzy.top/gtxkazuawz.html

Go:   // 手写 map[int]int
来源：http://hz.gzhubu.top/gtotmfcsxe.html

Ruby: // 手写 Hash
来源：http://hz.wangshuangyany.cn/gtcwajzdji.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.redwolf501.top/gtlgezwyle.html

[N08] 生成全排列
来源：http://hz.cqqwz.cn/gtczlymugm.html

Py:   itertools.permutations(arr)
来源：http://hz.jyoumei.cn/gtnvbdeinv.html

PHP:  // 手写递归交换
来源：http://hz.52xcode.cn/gtuyvbvkyh.html

JS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtutwphjjg.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gttccqfkts.html

Java: // 手写回溯递归
来源：http://hz.sysykeji.top/gtwnssmhxa.html

Go:   // 手写回溯递归
来源：http://hz.tanke756.top/gtqhltacgf.html

Ruby: arr.permutation.to_a
来源：http://hz.chenzaomai.com/gtmzypnwaq.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gturbvytcr.html

[N09] 栈与队列
来源：http://hz.jqgfzy.top/gtpqpcecxe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.havefunace.top/gtcmytpnxy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hammf.cn/gtgapxghtj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fengsongda.top/gtirhzumyh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.snrcjt.cn/gtjvrtwlvw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gtaohuzifg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gotoacloud.top/gtiftsbzcz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cashguo.top/gtcldhnrzu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtuhmravet.html

[N10] 链表节点定义
来源：http://hz.quarkkingdee.top/gtbrbxvnpe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hywenlv.cn/gtietkcekp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenjidiqi.icu/gtabldkbqe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhaomingkeji.xyz/gtyjilqqks.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtfeooqign.html

Java: class Node { int v; Node next; }
来源：http://hz.hywenlv.cn/gtixxcbvwg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnxiangtu.top/gtfzvuqigw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.havefunace.top/gttwwtszwg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenlongwang.top/gtaokooryw.html

[N11] 二叉树中序遍历
来源：http://hz.andypj.xyz/gtbexitruo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.smart0.xyz/gtdpiczpvg.html

PHP:  // 手写递归函数
来源：http://hz.snrcjt.cn/gttfixvbzb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gthpkecmij.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtgwmdzsrp.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtslisabqc.html

Go:   // 手写递归
来源：http://hz.yangfankeji.com/gtepruanxm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.vqdsnc.cn/gtaizwuocm.html

C#:   // 手写递归
来源：http://hz.nanxinkj.top/gtprrhgoao.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhixingplan.top/gtgerourbx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhongyouzk.top/gtflzxnfdp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fengsongda.top/gtapckcavy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtlqpxrugb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtscrpmhrs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhongyouzk.top/gtfjbhyako.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tianlin.xyz/gtdndkjwrl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pycfn.com/gtlicithzm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gthyayqybc.html

================================================================================
来源：http://hz.zdqjudy.top/gtwitibzra.html

O. 并发与异步
来源：http://hz.ywan-chungtsiang.top/gtminyrfzj.html

================================================================================
来源：http://hz.nwbrower.top/gtewweuwut.html

[O01] 启动一个线程
来源：http://hz.xingfuxueyuan.xyz/gtkbimphwr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258.top/gtcmmgzcig.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xziqi.cn/gtxtixqmfg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gthqwvfsjc.html

TS:   // 同 JS
来源：http://hz.aizwys.cn/gtfvwxqbgl.html

Java: new Thread(() -> f()).start()
来源：http://hz.hammf.cn/gtmqaykqss.html

Go:   go f()
来源：http://hz.hnxiangtu.top/gtzaoatymm.html

Ruby: Thread.new { f }
来源：http://hz.hongshengwenyu.top/gtmcgckkty.html

C#:   Task.Run(() => F());
来源：http://hz.xylfe.cn/gtpdadrsrl.html

[O02] 使用线程池
来源：http://hz.tianlin.xyz/gtrlxihbmn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhoulong.xyz/gtrbhsufxq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtzkpuvqll.html

JS:   // worker_threads 线程池
来源：http://hz.hnxiangtu.top/gtddbxieza.html

TS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtfbmmdgwa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daxiang520.top/gtflqvbfjj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gotoacloud.top/gtzqdjwpwk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtybgwtnhy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhongyouzk.top/gtfsqygbpi.html

[O03] 加锁保护共享数据
来源：http://hz.gaohongyu789.top/gtwodsorsy.html

Py:   with lock: shared += 1
来源：http://hz.jinqigfzy.top/gtpavnrjah.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sufxvd.cn/gtrmwrhwel.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gtoicsljko.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gthmjjechs.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigufen.top/gtgdgylyoe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gotoacloud.top/gtclppmiyf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtasqnhhrc.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigufen.top/gtrerqjijm.html

[O04] 定义异步函数并等待
来源：http://hz.aibaodan.cn/gtfxfqeohe.html

Py:   async def f():⏎    await g()
来源：http://hz.fzhhl.top/gtepoyygjm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.birdmap.top/gthztfatos.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtewmeeneh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gtcsanmvvw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuetiantiany.cn/gtcuimzqxv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258888.top/gtlgxmyxcb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtierwefvm.html

C#:   async Task F() { await G(); }
来源：http://hz.zycfv.cn/gtcyarnuyu.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgufenzy.top/gtbvmmejca.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cdnleiting.top/gtjjfnsvrv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.haohaochexian.top/gthoddtapv.html

JS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gteztiaebc.html

TS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtqbxepxex.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydzc1.top/gtepvocygr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtrxztehfh.html

Ruby: threads.map(&:join)
来源：http://hz.zhengqikj.top/gtnapyqnvq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhijiandao.cn/gtkvwlfych.html

[O06] 使用进程池
来源：http://hz.shanyushiyangkeji.top/gtehuiwzev.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hfpthk.cn/gtdbuqanvi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtpyxmntfa.html

JS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gthngajrpo.html


<!-- 参考信息 -->