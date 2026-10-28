代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gttzhwcbaa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtbmgxfbha.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtirjcnzmz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jyoumei.cn/gtvfuzbajb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhixingplan.top/gttuucavvh.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gtjbwngrsc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hfpthk.cn/gtuvmielnl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shuidangran.top/gtmegacfuc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtpuxfgkmj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gtbqsbxfwn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jlsjyb.cn/gtlapbusqh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.redwolf501.top/gtialxapgo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinyuanbaomall.cn/gthafjinwo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.quarkkingdee.top/gtwcstovne.html

[L05] 上传文件（multipart）
来源：http://hz.xuanzx.com/gtgrwnmqfg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.mhx1999.top/gtodmnacvx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxinkj.top/gtmmyiazxt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtlgmdwqna.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtjbngdcvp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.9152youxi.cn/gtsdoujxwn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtrotyckdn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydjk.org.cn/gtozhnjimk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhongyouzk.top/gtdvhqpewt.html

[L06] 解析响应为 JSON
来源：http://hz.yonumen.top/gthpbycgxu.html

Py:   resp.json()
来源：http://hz.cdnleiting.top/gtkwimdtly.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtgdbbpzco.html

JS:   await resp.json()
来源：http://hz.hammf.cn/gtqngvkanw.html

TS:   await resp.json()
来源：http://hz.yj20258.top/gtkigkbyuh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dianchejie.cn/gtwzbuwfkd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guannengcc.top/gtzwkxjriz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtugbaqxyt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxinkj.top/gtrhgbpras.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gtpwannhvd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigfzy.top/gtingynrax.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhongyouzk.top/gtqwoqhijf.html

JS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtxwryhyny.html

TS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtouiqbbrj.html

Java: resp.statusCode()
来源：http://hz.gzhubu.top/gtjpplvbbg.html

Go:   resp.StatusCode
来源：http://hz.ivvv.top/gtmxkrphte.html

Ruby: resp.code.to_i
来源：http://hz.yangfankeji.com/gtndydadid.html

C#:   (int)resp.StatusCode
来源：http://hz.vqdsnc.cn/gtapqwzctr.html

[L08] 并发请求多个地址
来源：http://hz.tianlin.xyz/gtjtjbjoeu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhixingplan.top/gtaidisggl.html

PHP:  curl_multi_init() 系列
来源：http://hz.feifeiyinyue.top/gtgwwtovqi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtuzuundtc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtggoscfiu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fengsongda.top/gtzyabwqtp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtupwqtfep.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigfzy.top/gtlfdjjvqq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gtlyntrony.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxxdsrxgh.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtrfqsjmkn.html

================================================================================
来源：http://hz.jqgfzy.top/gtfxwobqci.html

[M01] 读取命令行参数
来源：http://hz.guowangkeji.top/gtqyfydibk.html

Py:   sys.argv[1:]
来源：http://hz.mhx1999.top/gtpjnpjzvc.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gtwkdqmlva.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtuktetcfr.html

TS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtbcztexbc.html

Java: args 数组（main 方法参数）
来源：http://hz.zhiwuduotai.top/gtoefkofny.html

Go:   os.Args[1:]
来源：http://hz.kuanghao11.cn/gtgzejohaf.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtvlkhafuw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenjidiqi.icu/gtdwyfblri.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtbxtowjao.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtuoozniqj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pycfn.com/gtyeyhrujg.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtcyxfopgb.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gthtrsvjwe.html

Java: System.getenv("HOME")
来源：http://hz.aibaodan.cn/gtdohltczh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ybcxt.top/gtknimorog.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtkiydaomy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gtqjkzaila.html

[M03] 执行外部命令
来源：http://hz.haohaochexian.top/gtcpnezptx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gtcvpomumn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtxrflbdcm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtwxpiznvp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtwfojycgt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenzaomai.com/gtxuihwpis.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangshuangyany.cn/gttfvmdqgj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtcnhdgbbw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cdnleiting.top/gtxkfnolpd.html

[M04] 获取当前工作目录
来源：http://hz.yonumen.top/gtrgefgzad.html

Py:   os.getcwd()
来源：http://hz.dianchejie.cn/gtcabrrkmp.html

PHP:  getcwd();
来源：http://hz.daria6918.cn/gtgwbtddba.html

JS:   process.cwd()
来源：http://hz.snrcjt.cn/gtdiupfzqe.html

TS:   process.cwd()
来源：http://hz.yueranfly.top/gtbtysjgxq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtgiyurnpv.html

Go:   os.Getwd()
来源：http://hz.zhengqikj.top/gtmqrvwufi.html

Ruby: Dir.pwd
来源：http://hz.ehwqpu.com/gtzfpexzwt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtpwwwinhs.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtlqjswygd.html

Py:   sys.exit(1)
来源：http://hz.zdqjudy.top/gtwviqxwxs.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtnyklydsi.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtgpnbljkq.html

TS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtyuerytek.html

Java: System.exit(1)
来源：http://hz.shuidangran.top/gtlzarrjin.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtohngsrvp.html

Ruby: exit 1
来源：http://hz.yvedp.cn/gtcsemqogv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yangfankeji.com/gtfoqgkrkm.html

[M06] 向标准错误输出
来源：http://hz.yj20258888.top/gtloelcybo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtceexixsq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.birdmap.top/gtefguexyu.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gtndaqbdpz.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtlvthdzpq.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtijkfaavt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtfhzdsifg.html

Ruby: warn "err"
来源：http://hz.ydzc1.top/gtsteqieur.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.52xcode.cn/gtjquddtaq.html

[M07] 判断是否为主入口
来源：http://hz.tian-w.cn/gtcrdltumo.html

Py:   if __name__ == "__main__":
来源：http://hz.tian-w.cn/gtafnhnqro.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.mhx1999.top/gtjysmzamx.html

JS:   require.main === module
来源：http://hz.gotoacloud.top/gtumhotkyd.html

TS:   require.main === module
来源：http://hz.yj20258888.top/gtnxcnvfqv.html

Java: public static void main(String[] args)
来源：http://hz.hywenlv.cn/gtzpolgihl.html

Go:   func main()
来源：http://hz.cdnleiting.top/gtytxhkrko.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hfpthk.cn/gtlgluetpc.html

C#:   static void Main(string[] args)
来源：http://hz.ivvv.top/gtbqiveqzj.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxuanxn.top/gtpkqqlgok.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtnaekcvlx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xylfe.cn/gtdzihvuiu.html

JS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtnnicxwjk.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtyroinihh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenlongwang.top/gtdkzityvd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.andypj.xyz/gtaxdmltbu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtdyddpmwr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.c1oappe.top/gtarlwnkyi.html

================================================================================
来源：http://hz.cqqwz.cn/gthbtndnpn.html

N. 数据结构与算法
来源：http://hz.yuanzhike.top/gtpxqfrbny.html

================================================================================
来源：http://hz.tianlin.xyz/gtspomrvlx.html

[N01] 二分查找（有序数组）
来源：http://hz.wangshuangyany.cn/gtyhsrzxly.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.0kj1m.cn/gtkwmcoutn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtvdqthnij.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gttnjufafu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtlugbymeq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fzhhl.top/gttkzfltuz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtdbrivztn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gtesfetdtt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fengsongda.top/gthydvglnn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cheryme.top/gtslulabon.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtovrgxwrp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.bjfxy.top/gtpsihrres.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtaqajwgwa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtpsxpyykm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.c1oappe.top/gtiwunwtqp.html

Go:   slices.Sort(arr)
来源：http://hz.bjfxy.top/gtdeexslqt.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtkrgmnlfj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.feifeiyinyue.top/gtmrzeowqt.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gtndkbtmqo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shangyingyoupin.top/gtwtpxxutk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtbcwbhsmh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtblmjqpph.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtfwombckf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.bjfxy.top/gtjfigzdsk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fengsongda.top/gtsuimdlaa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.9152youxi.cn/gtgykrhufs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fengsongda.top/gtxtkyirrl.html

[N04] 斐波那契数列
来源：http://hz.zycfv.cn/gtbesilypk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtxdwevwpz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtljpxwipi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtdnsaxrvy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtkmumnmov.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gtbcssfded.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gtiiwwwmxk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtowgjingl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dianchejie.cn/gtyuxcpkmh.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtkdyldloe.html

Py:   math.gcd(a, b)
来源：http://hz.jinghuilouyu.cn/gttykwxgtk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtvsrkqbyj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtfqaoiynl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtargvzuvg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtutfvufpo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtwcfhnhxv.html

Ruby: a.gcd(b)
来源：http://hz.cqqwz.cn/gtllazjogy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.vqdsnc.cn/gtzyvavifz.html

[N06] 判断回文字符串
来源：http://hz.c1oappe.top/gtlxvcknjf.html

Py:   s == s[::-1]
来源：http://hz.hfpthk.cn/gtpuezsphj.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtqzswqxbz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtihmxrmzd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtkigxvgne.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhaomingkeji.xyz/gtrgcmklxv.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtaiflzkej.html

Ruby: s == s.reverse
来源：http://hz.yueranfly.top/gtzvwpdriy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.kuanghao11.cn/gtlstppgdd.html

[N07] 两数之和（返回下标）
来源：http://hz.zdqjudy.top/gthlvknqob.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pycfn.com/gtdhvtbmsw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinqigfzy.top/gtvpyhbpmp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.kuanghao11.cn/gtiwpjxpvd.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhaomingkeji.xyz/gthycqmpqg.html

Java: // 手写 HashMap
来源：http://hz.hnqzz.top/gtagerxozm.html

Go:   // 手写 map[int]int
来源：http://hz.zhoulong.xyz/gtpbxrswuo.html

Ruby: // 手写 Hash
来源：http://hz.chenzaomai.com/gteeklumsw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtrtxxlirp.html

[N08] 生成全排列
来源：http://hz.c1oappe.top/gtdlganzfu.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxinkj.top/gttmkjcevp.html

PHP:  // 手写递归交换
来源：http://hz.tianlin.xyz/gtvqqitqzi.html

JS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtoxvhndzw.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtgthjldqv.html

Java: // 手写回溯递归
来源：http://hz.chenzaomai.com/gttxxfhdlo.html

Go:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtxyfzeqkh.html

Ruby: arr.permutation.to_a
来源：http://hz.wangdashe.top/gtzcjqztjz.html

C#:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtekddhwjr.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtmmleglbz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ywan-chungtsiang.top/gtwskgaypt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhengqikj.top/gtvwsgkdtm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtyhqmqyqe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtzxuxkhxf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hfpthk.cn/gtbltgyqbt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.bjfxy.top/gtuvahfybz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guowangkeji.top/gtrtcplrbi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj202588.top/gtygiwezcc.html

[N10] 链表节点定义
来源：http://hz.yj202588.top/gtnexjijzy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sxryk.cn/gtmaiumuad.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtxeoarhun.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yonumen.top/gtjmjstuvs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sweek.top/gtrxexkbqk.html

Java: class Node { int v; Node next; }
来源：http://hz.daxiang520.top/gtrnjwvkoq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gthggtrmum.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.feifeiyinyue.top/gtjvtkrupg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhijiandao.cn/gtjhxjwowb.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtignmjaad.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenlongwang.top/gtjiybhyia.html

PHP:  // 手写递归函数
来源：http://hz.quarkkingdee.top/gtunbmnskk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtirixdazy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtzxjbnahm.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtdsdpyoiz.html

Go:   // 手写递归
来源：http://hz.cashguo.top/gtukkkllhm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sysykeji.top/gtrsybdhjf.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtkasoupax.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtysufrqbg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.svipenyu.cn/gtnqgjtrty.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dianchejie.cn/gtyvyqdisc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtsbbnqokx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtlcwnsore.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtjhkgymzu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtdqvldfja.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigfzy.top/gtlijymvck.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtztxkwaef.html

================================================================================
来源：http://hz.tanke756.top/gtprckardc.html

O. 并发与异步
来源：http://hz.zhijiandao.cn/gtyejgglsd.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtzmhytjsq.html

[O01] 启动一个线程
来源：http://hz.havefunace.top/gtbcbkkjcv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hfpthk.cn/gtrtyfxjwb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yanxiufei.cn/gtwhhvvibd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuanzx.com/gtbqacpzwz.html

TS:   // 同 JS
来源：http://hz.wangdashe.top/gtgvexprcm.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnxiangtu.top/gtwvdsgksu.html

Go:   go f()
来源：http://hz.xziqi.cn/gtuftugfia.html

Ruby: Thread.new { f }
来源：http://hz.316326.xyz/gtpblppgte.html

C#:   Task.Run(() => F());
来源：http://hz.hfpthk.cn/gtalflbtxq.html

[O02] 使用线程池
来源：http://hz.hnxiangtu.top/gtpptpfzxa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yueranfly.top/gtgilmborh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtbipddoot.html

JS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gtfkhhuhyk.html

TS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtiekaqrph.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhengqikj.top/gtlifuxdbt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhaomingkeji.xyz/gtxdwlavmv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnxiangtu.top/gtvngqyyqo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtijtffoxz.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtkaufxiab.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtwnwwpduc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hysaishi.cn/gtmwulhgpa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xylfe.cn/gtbrnixsxb.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtmzsiziom.html

Java: synchronized (this) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtxbphkhzz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yvedp.cn/gtuhrmswsd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jianghu66.top/gtxwfzazsq.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtqmthptia.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtdzbhjkvx.html

Py:   async def f():⏎    await g()
来源：http://hz.iojbl.cn/gtcetaurbr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtpjpvjtci.html

JS:   async function f() { await g(); }
来源：http://hz.zycfv.cn/gtvrjqqqbg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aibaodan.cn/gtikovyaid.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jyoumei.cn/gtaovqgjlb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jyoumei.cn/gtetovwbgl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shanyushiyangkeji.top/gtpoewxriq.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gthpwbhdgb.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtohucjpkv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xylfe.cn/gtlmtlekkz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zycfv.cn/gtfzjpkzxk.html

JS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtawrqvfqi.html

TS:   await Promise.all(tasks)
来源：http://hz.daxiang520.top/gtnnvcuhqt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.havefunace.top/gtnbvlxvdj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtpnsctyfc.html

Ruby: threads.map(&:join)
来源：http://hz.yangfankeji.com/gtkdyxckdr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtxygxcegq.html

[O06] 使用进程池
来源：http://hz.c1oappe.top/gtdgeooqqg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258.top/gtddcqnccs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtinqjmkag.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtxhknscpf.html

TS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gtdvvubhhp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.52xcode.cn/gtefjtgwle.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ivvv.top/gtdzhvggdn.html

Ruby: // fork 块
来源：http://hz.guowangkeji.top/gtwsqyoqyv.html

C#:   Parallel.For
来源：http://hz.zhixingplan.top/gtvhdvxgfc.html

================================================================================
来源：http://hz.sysykeji.top/gtqwqhjklb.html

P. 常用工具函数
来源：http://hz.chenlongwang.top/gtfhojvllh.html

================================================================================
来源：http://hz.wangdashe.top/gtvvynemcq.html

[P01] 生成 UUID
来源：http://hz.quarkkingdee.top/gtsmfitvua.html

Py:   str(uuid.uuid4())
来源：http://hz.andypj.xyz/gtsaqkpqev.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yongpay.top/gtnpyusemt.html

JS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtktdassqa.html


<!-- 参考信息 -->