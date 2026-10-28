代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.9152youxi.cn/gtttmredcf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtsimqfhnk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.316326.xyz/gtdrxgtsuw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ivvv.top/gtjozdpmqd.html

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtwxjnlhmp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hongshengwenyu.top/gtcgzlizhb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sweek.top/gtufcxszra.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gtnvwpsobo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtyliaqhvv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ivvv.top/gtqymxjseh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtcevdddba.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yongpay.top/gtxozgszxy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtvqqixmub.html

[L04] 设置超时
来源：http://hz.zhoulong.xyz/gtbnqwnkau.html

Py:   requests.get(url, timeout=5)
来源：http://hz.birdmap.top/gtypkcqrbu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtwubfzgpp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtsdyfjrag.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtfdtlgmst.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xingfuxueyuan.xyz/gtpafnwxss.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxuanxn.top/gtibxuxgst.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtqkuzdovm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinghuilouyu.cn/gtqrfwqnxj.html

[L05] 上传文件（multipart）
来源：http://hz.xylfe.cn/gtaukenygk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtwtfallsk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.kuanghao11.cn/gtinlrarqk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gthiidojgd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtxynfhotu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dianchejie.cn/gthtmmuydp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtrvjgnzcn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxinkj.top/gtdtngfjxv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gtcwrirhlm.html

[L06] 解析响应为 JSON
来源：http://hz.gogol.net.cn/gtslqawjto.html

Py:   resp.json()
来源：http://hz.quarkkingdee.top/gtmiwusljt.html

PHP:  json_decode($body, true);
来源：http://hz.xuanzx.com/gtdkyelxrm.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtakjuadmv.html

TS:   await resp.json()
来源：http://hz.svipenyu.cn/gtghvlktpl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhixingplan.top/gthkguepva.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenzaomai.com/gtulpsnebk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangshuangyany.cn/gtrwnghovd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtrmuxbknt.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gtprwvgtxh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jiagoushi.top/gtxwewjfmr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtewclxfkc.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtjyymverg.html

TS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtpkokards.html

Java: resp.statusCode()
来源：http://hz.zhoulong.xyz/gtpaohuizl.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtirqbvtzt.html

Ruby: resp.code.to_i
来源：http://hz.mhx1999.top/gtfiovjpht.html

C#:   (int)resp.StatusCode
来源：http://hz.zdqjudy.top/gtjjabhlfe.html

[L08] 并发请求多个地址
来源：http://hz.zdqjudy.top/gtbfkiktgk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.316326.xyz/gtalbiocja.html

PHP:  curl_multi_init() 系列
来源：http://hz.aizwys.cn/gtizamhkyo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtulkttvov.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gthtossroi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cashguo.top/gtgcskflme.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aizwys.cn/gtwaifthhf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtoxkglpxm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenjidiqi.icu/gtriekrjeg.html

================================================================================
来源：http://hz.vqdsnc.cn/gthzgaiqim.html

M. 命令行 / 进程 / 环境
来源：http://hz.sufxvd.cn/gtdvshmqua.html

================================================================================
来源：http://hz.chenzaomai.com/gtmjfuxnon.html

[M01] 读取命令行参数
来源：http://hz.xylfe.cn/gtvkelcbgf.html

Py:   sys.argv[1:]
来源：http://hz.zhengqikj.top/gtkvawdyqg.html

PHP:  $argv;  $argc;
来源：http://hz.haohaochexian.top/gtiqqrsljj.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtxdmwrpfq.html

TS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtcojggmjr.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtddvgqvyv.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtsnnhvyco.html

Ruby: ARGV
来源：http://hz.ywan-chungtsiang.top/gtnocqtpdp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gtgsftcoai.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gtisekhqwo.html

Py:   os.environ.get("HOME")
来源：http://hz.smart0.xyz/gtuekgxtuk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sufxvd.cn/gtzxixxyut.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtfepnzdps.html

TS:   process.env.HOME
来源：http://hz.sweek.top/gtzxldrtre.html

Java: System.getenv("HOME")
来源：http://hz.mhx1999.top/gtupttcnxh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yangfankeji.com/gtqdthlazw.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gtajrdssvp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtbactgvkk.html

[M03] 执行外部命令
来源：http://hz.meibo888.top/gtiyzqhbev.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtdnlqbkza.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gtndhpxpxe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtaeoijvqr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtaefejxba.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtwllcwfxf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtytqohuvc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtcmbepxpg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtcvexfkdb.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtlvmbjcfn.html

Py:   os.getcwd()
来源：http://hz.wangshuangyany.cn/gtymutoonk.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gtliueerlf.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtuaqvxvys.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtqfvgbjek.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydzc1.top/gtiwaqcpjh.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtsbmxzgll.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtnhfzvjje.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtptescwix.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtppdkznqn.html

Py:   sys.exit(1)
来源：http://hz.mhx1999.top/gtmbxfdpwg.html

PHP:  exit(1);
来源：http://hz.svipenyu.cn/gttshjjnpw.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtsfdwghxu.html

TS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtibiujygf.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gtcbmfaewv.html

Go:   os.Exit(1)
来源：http://hz.cucudq.cn/gtfgzspmtg.html

Ruby: exit 1
来源：http://hz.jlsjyb.cn/gtqavbulnj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gtptdpjcvw.html

[M06] 向标准错误输出
来源：http://hz.yj20258888.top/gtypvujvlg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gtzqnpzcwz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangtech.top/gtxsirvujc.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtveaxpxsn.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtgolcoktg.html

Java: System.err.println("err")
来源：http://hz.yj20258.top/gtafwxyusi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gthfvpkobd.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtzbcyyvxj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtdzaupvfm.html

[M07] 判断是否为主入口
来源：http://hz.snrcjt.cn/gtnvphgphb.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtajesefnv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nwbrower.top/gtoozejdph.html

JS:   require.main === module
来源：http://hz.316326.xyz/gtmuiyfxhi.html

TS:   require.main === module
来源：http://hz.svipenyu.cn/gtasvkczif.html

Java: public static void main(String[] args)
来源：http://hz.mhx1999.top/gtgrllxsnm.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtlmnacywn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cdnleiting.top/gtxzqudwip.html

C#:   static void Main(string[] args)
来源：http://hz.cheryme.top/gtzlwpsagd.html

[M08] 获取系统与运行时信息
来源：http://hz.hongshengwenyu.top/gtfdegvhsy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangdashe.top/gtzbatsigb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtljpcxoic.html

JS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtsxepmoef.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtjfkimzvt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.mhx1999.top/gtqfuhipwn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gtsxkwpqrv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtxnvyrmeq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zycfv.cn/gtymxhgaai.html

================================================================================
来源：http://hz.gotoacloud.top/gtpimlkbtg.html

N. 数据结构与算法
来源：http://hz.ywan-chungtsiang.top/gtrvhzcdny.html

================================================================================
来源：http://hz.yonumen.top/gtwhcpdagq.html

[N01] 二分查找（有序数组）
来源：http://hz.daria6918.cn/gtpdsorowu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cqqwz.cn/gtcfetfrzp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cashguo.top/gtzeyrkxiw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtccovtkbv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtdoijkeqn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yueranfly.top/gtmradhuvv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtocbgtzpl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtnibdufrz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cucudq.cn/gtrlhmhqgm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgufenzy.top/gtcffarplj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.birdmap.top/gtjssrwcto.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydjk.org.cn/gtvmisfqft.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtipivrfxz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gthpetfpwv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258.top/gtiwuatksg.html

Go:   slices.Sort(arr)
来源：http://hz.zycfv.cn/gtzwvhxrxc.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gthlehcsgr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtvwecgfis.html

[N03] 快速排序（分治示例）
来源：http://hz.gotoacloud.top/gtzysmwyes.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gthieflqfr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtqgnliaaa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtprucgotf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtxqprmlfi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zdqjudy.top/gttdiuboqq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tianlin.xyz/gtpegajlfw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhongyouzk.top/gtabbanawa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258888.top/gtyxqjevtr.html

[N04] 斐波那契数列
来源：http://hz.jqgufenzy.top/gtketwclix.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtmtqwafoc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenzaomai.com/gtsbzsilpz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtltjtwxld.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtkyyumwuq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtpjlyvolt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigfzy.top/gtayzhmrpv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtvwjvrybd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigfzy.top/gthdmktjvk.html

[N05] 最大公约数
来源：http://hz.quarkkingdee.top/gtynlugxar.html

Py:   math.gcd(a, b)
来源：http://hz.jinghuilouyu.cn/gtjtdeyeth.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtojkrqcoz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtehxekcbd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtjfhvybvf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtoohkpsrm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnxiangtu.top/gthubzryfj.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtyojqyfzc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gtkoftrwup.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtkjewxwbm.html

Py:   s == s[::-1]
来源：http://hz.gogol.net.cn/gturhvayrr.html

PHP:  $s === strrev($s);
来源：http://hz.gaohongyu789.top/gtlpbzahce.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtnqhrujzt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtpkeeprcm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pengpengdd.cyou/gtprsalefg.html

Go:   // 双指针从两端比较
来源：http://hz.daria6918.cn/gtkcbyyfzw.html

Ruby: s == s.reverse
来源：http://hz.hysaishi.cn/gtpfavllqe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtbvhsqnwn.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gtvjpegiah.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtsfsnbmsj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinqigufen.top/gtkmujuvoc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.meibo888.top/gtmjvggicb.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gtiwndxqtc.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtwaysywbt.html

Go:   // 手写 map[int]int
来源：http://hz.shuidangran.top/gtvmaopmaf.html

Ruby: // 手写 Hash
来源：http://hz.ppjwa.cn/gtwtioykhn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jyoumei.cn/gthpbtlpxr.html

[N08] 生成全排列
来源：http://hz.yongpay.top/gtmcltnvlc.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangtech.top/gtwqjwizsy.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtkjalltet.html

JS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtoccdteis.html

TS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtvwzgnuwf.html

Java: // 手写回溯递归
来源：http://hz.dianchejie.cn/gtcefdhvlp.html

Go:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gthmtfyhur.html

Ruby: arr.permutation.to_a
来源：http://hz.guannengcc.top/gtqdppyzgt.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtreqeotrx.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtfqqkctwg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigufen.top/gtvnclnjcl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtvauvknpp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.smart0.xyz/gtbuayhifb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ywan-chungtsiang.top/gtuikudgcj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sufxvd.cn/gtjucgdyrj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xingfuxueyuan.xyz/gtwlhdyhmt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gtxrvlxwmi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtanrbjiil.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtdgrfszjp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangdashe.top/gtkywvzaas.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinghuilouyu.cn/gtftumdzpr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gtrvrekzvr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tian-w.cn/gtnssgnecz.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtfphdjepe.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ivvv.top/gtsnltmiir.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangshuangyany.cn/gtlxiloxha.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.haohaochexian.top/gtpemcvubh.html

[N11] 二叉树中序遍历
来源：http://hz.c1oappe.top/gtrzukwory.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jlsjyb.cn/gtjgdxjsxh.html

PHP:  // 手写递归函数
来源：http://hz.mhx1999.top/gtbqolljqq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gtsgolurpj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtipgqiszo.html

Java: // 手写递归
来源：http://hz.316326.xyz/gtsocjtste.html

Go:   // 手写递归
来源：http://hz.jqgufenzy.top/gtjxdcpypl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinghuilouyu.cn/gtargbbred.html

C#:   // 手写递归
来源：http://hz.sweek.top/gtrndcuwte.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dianchejie.cn/gtyoqrhite.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yvedp.cn/gtzatlxkvc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tian-w.cn/gtednktyin.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtmviulddb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtdntykwja.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxuanxn.top/gtpzwwsfqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aibaodan.cn/gtnteyeboc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shzxlz.cn/gtvcvupygc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtpwiejsla.html

================================================================================
来源：http://hz.jiagoushi.top/gtlfaqpdua.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtbkttvlsw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtuiokvzrq.html

[O01] 启动一个线程
来源：http://hz.sxryk.cn/gtunnoozpl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dianchejie.cn/gtlgeteqyd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtzjlbvgfi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gtdtynwqow.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtldnxokvf.html

Java: new Thread(() -> f()).start()
来源：http://hz.yanxiufei.cn/gtonifimmh.html

Go:   go f()
来源：http://hz.cashguo.top/gtkxenxylx.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtrxnfvwsc.html

C#:   Task.Run(() => F());
来源：http://hz.jyoumei.cn/gtjoqfoels.html

[O02] 使用线程池
来源：http://hz.xuetiantiany.cn/gtwbcbcdky.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cdnleiting.top/gtcrvajogn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jiagoushi.top/gtjeywjtid.html

JS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtvmbddjvg.html

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtslnfiobz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daria6918.cn/gtijxqwzfq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jyoumei.cn/gtvjynbzal.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtdueewepv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinghuilouyu.cn/gteahtzbwd.html

[O03] 加锁保护共享数据
来源：http://hz.pengpengdd.cyou/gtrokmdvkn.html

Py:   with lock: shared += 1
来源：http://hz.jinghuilouyu.cn/gtafursftp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuanzhike.top/gthqbxiiuz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtkcfvpcmg.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtxoyftzyh.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtopknavvm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenlongwang.top/gtmxzpivja.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhiwuduotai.top/gtxiwbtyyn.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtachgtici.html

[O04] 定义异步函数并等待
来源：http://hz.hnqzz.top/gtdenkbmch.html

Py:   async def f():⏎    await g()
来源：http://hz.fengsongda.top/gtarnimrhx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhijiandao.cn/gtgwtvxoxu.html

JS:   async function f() { await g(); }
来源：http://hz.havefunace.top/gtjlkazehx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cdnleiting.top/gtxudsivml.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtsazxdycl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydjk.org.cn/gtjmnfmraq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhiwuduotai.top/gttergvwnq.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtpwtadrtv.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gtgbnxeqko.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gotoacloud.top/gtvojyraez.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxuanxn.top/gtkmoaewcz.html

JS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtemfetddp.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtdmwkxnzl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fzhhl.top/gtsmsstkrv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinghuilouyu.cn/gtvwfkifmk.html

Ruby: threads.map(&:join)
来源：http://hz.cucudq.cn/gtmsqhuxrp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydzc1.top/gtyogqcodj.html

[O06] 使用进程池
来源：http://hz.yongpay.top/gtfeuocama.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shuidangran.top/gtlbecpnve.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.haohaochexian.top/gtdittidph.html

JS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtdtkthwaw.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtrwoowbvi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangshuangyany.cn/gtmtaetesn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtndaxzzna.html

Ruby: // fork 块
来源：http://hz.yj202588.top/gtncnnzmdn.html


<!-- 参考信息 -->