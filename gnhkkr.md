代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtdumgsqah.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigufen.top/gtzkdblrve.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gthtjiwtji.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtqzowiopr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gteogsfvgo.html

[L04] 设置超时
来源：http://hz.nanxinkj.top/gtimrorulv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigfzy.top/gtomxikmvk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenlongwang.top/gtwgbgngyz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtynrzwpag.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtddxyhdsg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ybcxt.top/gtgawsdltr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yonumen.top/gtgdsepezo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtsejpvngb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxinkj.top/gtakxpcyiq.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gtvpheykmp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.havefunace.top/gtjdjnsemt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xziqi.cn/gtjaghmeaq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gttrcrhngl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtomstztni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hongshengwenyu.top/gtwbkezitl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hammf.cn/gtlusbptyt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gtaouvypys.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnxiangtu.top/gtspowkxhc.html

[L06] 解析响应为 JSON
来源：http://hz.redwolf501.top/gtackrvemt.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtitqvsyug.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtjbkmsslx.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtjaoqflsp.html

TS:   await resp.json()
来源：http://hz.dianchejie.cn/gthgajnsdv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nwbrower.top/gtbqwtqohc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shuidangran.top/gtgbzcjmdu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj202588.top/gtkcgbrkom.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cheryme.top/gtouygipnj.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtheigwvdx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.316326.xyz/gtxpugkrfq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.feifeiyinyue.top/gtjnkcempa.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtiizovexg.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtqswwocum.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtvbprbcno.html

Go:   resp.StatusCode
来源：http://hz.aizwys.cn/gtkjhkksqx.html

Ruby: resp.code.to_i
来源：http://hz.yuxming.cn/gtgrytldic.html

C#:   (int)resp.StatusCode
来源：http://hz.cqqwz.cn/gtsvjlfask.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtsrvrhkbb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.meibo888.top/gtrrhgpvhv.html

PHP:  curl_multi_init() 系列
来源：http://hz.yanxiufei.cn/gtyessygfo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtmwknuzqo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtcavstzte.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuanzhike.top/gtkizhciti.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sxryk.cn/gthdiwkefk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shangyingyoupin.top/gtrgcfhapd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cucudq.cn/gtoaomwprf.html

================================================================================
来源：http://hz.havefunace.top/gtzzrfqxqw.html

M. 命令行 / 进程 / 环境
来源：http://hz.jiagoushi.top/gtvddrvlrd.html

================================================================================
来源：http://hz.nanxinkj.top/gtndrfjvna.html

[M01] 读取命令行参数
来源：http://hz.gaohongyu789.top/gtpxkmcnge.html

Py:   sys.argv[1:]
来源：http://hz.meibo888.top/gtwvdsadqr.html

PHP:  $argv;  $argc;
来源：http://hz.quarkkingdee.top/gtqvoixcio.html

JS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtanjycdvk.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtykvjocnt.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtwyfumvwy.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtyrdwadrn.html

Ruby: ARGV
来源：http://hz.shanyushiyangtech.top/gtvlnxtqrq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aibaodan.cn/gtskununox.html

[M02] 读取环境变量
来源：http://hz.meibo888.top/gtnixairlh.html

Py:   os.environ.get("HOME")
来源：http://hz.yueranfly.top/gtwdnckwbk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sxryk.cn/gtzqpjeibg.html

JS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtzanosmpf.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gtyckwohei.html

Java: System.getenv("HOME")
来源：http://hz.xylfe.cn/gtdyaqdmzr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pycfn.com/gtmydmlios.html

Ruby: ENV["HOME"]
来源：http://hz.xuanzx.com/gtaslkmryu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gtaouaevui.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gtkcycphws.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtidijvkjg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gtstpvqfti.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtyjipbgra.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtwgxnwyuh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangdashe.top/gtovimgvdq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cdnleiting.top/gtmkrhejfa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtvlbqhxtq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.feifeiyinyue.top/gtmeffkdgx.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtjglpprxr.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtoydfaisk.html

PHP:  getcwd();
来源：http://hz.jinyuanbaomall.cn/gtpcwmjnec.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtxxpoqzks.html

TS:   process.cwd()
来源：http://hz.tian-w.cn/gtwumendpa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yongpay.top/gtuvfjkwod.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtdeonsgkm.html

Ruby: Dir.pwd
来源：http://hz.nanxinkj.top/gtxhmyqusq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtbuvnyivm.html

[M05] 设置退出码
来源：http://hz.svipenyu.cn/gtmqoaghvc.html

Py:   sys.exit(1)
来源：http://hz.jqgfzy.top/gtllxvdknj.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtbssmafyo.html

JS:   process.exit(1)
来源：http://hz.shuidangran.top/gtrxzmlbdd.html

TS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtreziapcm.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtkxzkbbms.html

Go:   os.Exit(1)
来源：http://hz.iojbl.cn/gtfzutyoca.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtotonshcd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtqkfrznuk.html

[M06] 向标准错误输出
来源：http://hz.xingfuxueyuan.xyz/gtdjkirfbi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtugkuisax.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pengpengdd.cyou/gtcrlldqfm.html

JS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtbnlohbxh.html

TS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtrbngoigi.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtgasnhdqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxuanxn.top/gtxrdjkcja.html

Ruby: warn "err"
来源：http://hz.svipenyu.cn/gtpnvrtyuu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.mhx1999.top/gtcxehkekj.html

[M07] 判断是否为主入口
来源：http://hz.birdmap.top/gtxpkdujla.html

Py:   if __name__ == "__main__":
来源：http://hz.jianghu66.top/gtexyezsli.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtjbbfapqw.html

JS:   require.main === module
来源：http://hz.ydjk.org.cn/gtversecux.html

TS:   require.main === module
来源：http://hz.shuidangran.top/gtrnlqedno.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtajvmikfj.html

Go:   func main()
来源：http://hz.tanke756.top/gtsrmykfcm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.pycfn.com/gtxwazmpws.html

C#:   static void Main(string[] args)
来源：http://hz.ydjk.org.cn/gtlkdiztap.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gttufagvls.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258888.top/gtglmmfhmi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtdhazbgzn.html

JS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gtvtlufayi.html

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtucspanyz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtorgxhgkk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtbhgmixdn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gtszpzjpxu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangtech.top/gtucsthsts.html

================================================================================
来源：http://hz.smart0.xyz/gtuadibqag.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtzdejqcrr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtlbitioct.html

[N01] 二分查找（有序数组）
来源：http://hz.yj202588.top/gtstyvxtsp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.bjfxy.top/gtcxebdzfo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.smart0.xyz/gtokqsejau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtlgadfpin.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtevxiihsv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtilfoofrl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtzaxhbrrn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangshuangyany.cn/gtubkhiwjx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtpknqekak.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydzc1.top/gtdakginbk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gttfrvrfik.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtbtxjuomz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gttgfclehr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gttflethsg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxuanxn.top/gtgihgiard.html

Go:   slices.Sort(arr)
来源：http://hz.iojbl.cn/gttsodrkvt.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtpmfriwcq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.iojbl.cn/gtvzvkshxo.html

[N03] 快速排序（分治示例）
来源：http://hz.daria6918.cn/gtqcoplkwg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigufen.top/gtyrimlpao.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuetiantiany.cn/gtalbmixki.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gthfhpsprf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtjnrtgawk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhongyouzk.top/gtzmqdlfbu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj202588.top/gttgwvsyxb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtsflgiaxq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydzc1.top/gtiqzliapt.html

[N04] 斐波那契数列
来源：http://hz.zhiwuduotai.top/gtgcspcrqq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtrqiahhci.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenlongwang.top/gtlyqsmsup.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtvcmjfvym.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtwykuaoyq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jianghu66.top/gtihsowboj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtszaxekmy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gttnoqzptk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zdqjudy.top/gttgpbsstc.html

[N05] 最大公约数
来源：http://hz.chenlongwang.top/gtyugacvcs.html

Py:   math.gcd(a, b)
来源：http://hz.gzhubu.top/gtvdnpryfq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gttzrnuoxu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtsvjofpoe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtnnsvfiev.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yanxiufei.cn/gtkgcaigig.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenjidiqi.icu/gtbttxavrn.html

Ruby: a.gcd(b)
来源：http://hz.hywenlv.cn/gtbwxtxdba.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.havefunace.top/gtktajejwn.html

[N06] 判断回文字符串
来源：http://hz.vqdsnc.cn/gtqwspsnyr.html

Py:   s == s[::-1]
来源：http://hz.yj20258888.top/gtkkefvmtf.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gtntkhvqee.html

JS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtqestldnv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtyjyrhfgp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yueranfly.top/gtiluplphx.html

Go:   // 双指针从两端比较
来源：http://hz.xinyue.icu/gtkfogoogc.html

Ruby: s == s.reverse
来源：http://hz.ehwqpu.com/gtlhfhsypy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtgaqojgmt.html

[N07] 两数之和（返回下标）
来源：http://hz.cheryme.top/gtdwumsevf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shzxlz.cn/gtotjgjbda.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtcwqgxqnn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtdvnihddk.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtosiqkuqy.html

Java: // 手写 HashMap
来源：http://hz.hnxiangtu.top/gtlstxmbmb.html

Go:   // 手写 map[int]int
来源：http://hz.guannengcc.top/gtqocybztc.html

Ruby: // 手写 Hash
来源：http://hz.52xcode.cn/gtstaoxvbg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dianchejie.cn/gtskyqicce.html

[N08] 生成全排列
来源：http://hz.zhixingplan.top/gtxivoefua.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtycjlfrbk.html

PHP:  // 手写递归交换
来源：http://hz.ywan-chungtsiang.top/gtfhponauy.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtipsdvmqk.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtlbzlnqcr.html

Java: // 手写回溯递归
来源：http://hz.tian-w.cn/gtymssxwbt.html

Go:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtradapiat.html

Ruby: arr.permutation.to_a
来源：http://hz.c1oappe.top/gtdaqwyswa.html

C#:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtdfpuikzo.html

[N09] 栈与队列
来源：http://hz.gaohongyu789.top/gtplflupcy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtbenigqjn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gotoacloud.top/gtyeoslhrh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.vqdsnc.cn/gthvoplxvr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtqehmcecf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtoqmveuqg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtcivfqmxl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtmdbyumwg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigfzy.top/gtjcpcapmc.html

[N10] 链表节点定义
来源：http://hz.chenjidiqi.icu/gtzeauvubf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtzjlrojlm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.0kj1m.cn/gtfforbbvx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenjidiqi.icu/gtitgnphxs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangtech.top/gtbmyvfnto.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtsnwbbryp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ehwqpu.com/gtjttlkjch.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinghuilouyu.cn/gtxjdxnqzt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yongpay.top/gtxbktivdx.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtvlspblmn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtnbuulyoe.html

PHP:  // 手写递归函数
来源：http://hz.hnqzz.top/gteeuualxv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtcjwdycsj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtqsdthryn.html

Java: // 手写递归
来源：http://hz.yuanzhike.top/gtekaxhsmp.html

Go:   // 手写递归
来源：http://hz.jyoumei.cn/gtyudpkpov.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.52xcode.cn/gtlhannzyk.html

C#:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtdbzcmoju.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258.top/gteulzipbm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.svipenyu.cn/gtsnxrpzff.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.andypj.xyz/gttauqmhos.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtxpjdpond.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gthnrzmrjc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtjdeiluaw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gtvrqmmteb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxinkj.top/gtwvkynrqu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zdqjudy.top/gtgfsvdclk.html

================================================================================
来源：http://hz.gzhubu.top/gtkwfozdkj.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtcylqnrqb.html

================================================================================
来源：http://hz.aizwys.cn/gtostrdtru.html

[O01] 启动一个线程
来源：http://hz.ydjk.org.cn/gtctvusjym.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pycfn.com/gtifdpvypa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtoiqfvgfy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gtexqrylza.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gttfqddcgo.html

Java: new Thread(() -> f()).start()
来源：http://hz.snrcjt.cn/gtsrottuiv.html

Go:   go f()
来源：http://hz.dashuyun.cn/gtsvmkrvrv.html

Ruby: Thread.new { f }
来源：http://hz.zhixingplan.top/gtakrwonlj.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtycqedrlc.html

[O02] 使用线程池
来源：http://hz.bjfxy.top/gthwmmkxqf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sufxvd.cn/gtkmcpkhio.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenzaomai.com/gtdoyvator.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtwuleumus.html

TS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtnyexykvh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.haohaochexian.top/gtevfnvess.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jyoumei.cn/gtztepipws.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtdwgmowyp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ppjwa.cn/gtadbcjsis.html

[O03] 加锁保护共享数据
来源：http://hz.zhoulong.xyz/gtkgvcobhq.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtaggsqgph.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aibaodan.cn/gtnrtsqpfw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yueranfly.top/gtrqaclbcw.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtudvatjjn.html

Java: synchronized (this) { shared++; }
来源：http://hz.feifeiyinyue.top/gtiiwenpzz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hongshengwenyu.top/gtafroxebb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shanyushiyangtech.top/gtzqphnmwg.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtggjhxxkw.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gtcpgsrajv.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgufenzy.top/gtdhzbsdcx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jiagoushi.top/gtnfeeswkb.html

JS:   async function f() { await g(); }
来源：http://hz.ehwqpu.com/gtjbgmuzfj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sxryk.cn/gtoreqzpkb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenzaomai.com/gtuypwebtu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydzc1.top/gtngwlecbk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xingfuxueyuan.xyz/gtcqnuokde.html

C#:   async Task F() { await G(); }
来源：http://hz.fzhhl.top/gtkuhetiub.html

[O05] 并发执行并等待全部完成
来源：http://hz.xinyue.icu/gtizhckhzx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.316326.xyz/gtychhkwcp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.andypj.xyz/gtgkkosmhl.html

JS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtssyedpal.html

TS:   await Promise.all(tasks)
来源：http://hz.hysaishi.cn/gtrxjkwcww.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sxryk.cn/gtycgdukvx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gtlnlpmhqc.html

Ruby: threads.map(&:join)
来源：http://hz.zhiwuduotai.top/gtmyxytszr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtnpxrirye.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtrzsguakn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hfpthk.cn/gtrmuoiqki.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dashuyun.cn/gtgxgeennm.html

JS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtgbzlucko.html

TS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtgfwftmrm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ppjwa.cn/gtrwqvrstg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258888.top/gtmlepypgs.html

Ruby: // fork 块
来源：http://hz.fzhhl.top/gtjzdfntyy.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gtbnowiqpm.html

================================================================================
来源：http://hz.ydzc1.top/gtfjrtjaic.html

P. 常用工具函数
来源：http://hz.gzhubu.top/gtsdtqioeo.html

================================================================================
来源：http://hz.yj20258888.top/gthldveywe.html

[P01] 生成 UUID
来源：http://hz.jinqigfzy.top/gtisuruwkk.html

Py:   str(uuid.uuid4())
来源：http://hz.guannengcc.top/gtwewklnzt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtwjifxrvv.html

JS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtsxyjkasr.html


<!-- 参考信息 -->