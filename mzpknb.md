代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sweek.top/gtmobcwdva.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenjidiqi.icu/gtdjxroyqc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtkxlotmjg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtamyqelds.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtlreaxwxg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtdrqlaext.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gtfpccmrtr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhengqikj.top/gtsggjcdvo.html

[L03] 设置自定义请求头
来源：http://hz.zhoulong.xyz/gtztcuwrvs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gtzybwlxgo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtxxzeqlhi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtvwnkcktt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtmutyuytn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xingfuxueyuan.xyz/gtqbwzmcds.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtjregnlcj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenlongwang.top/gtzeiyjnrj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtikrwpvlm.html

[L04] 设置超时
来源：http://hz.chenlongwang.top/gtvscvhzfu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jiagoushi.top/gtiudfcyns.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtdkwwrywx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtgydynudo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtrbfortpm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtmtdsukxq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtwethnpuv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hysaishi.cn/gtvgzpngva.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hysaishi.cn/gtskxcidxm.html

[L05] 上传文件（multipart）
来源：http://hz.bjfxy.top/gtdkrkjngd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangshuangyany.cn/gtrxasxqum.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtfcryuayb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtzjtgsdxx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtjblrdedq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.mhx1999.top/gteovlkblf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtzlxcqrcj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtrhblgnik.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtaibbpvlw.html

[L06] 解析响应为 JSON
来源：http://hz.sxryk.cn/gtecklhkvj.html

Py:   resp.json()
来源：http://hz.zhiwuduotai.top/gtphdawsnf.html

PHP:  json_decode($body, true);
来源：http://hz.zhengqikj.top/gtqfytzsgj.html

JS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtnqbxckug.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtouzovwcs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cashguo.top/gtcbliuekk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhongyouzk.top/gthvtitzon.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigfzy.top/gtgsboigpc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guowangkeji.top/gtydfpvhiv.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtykwgzqqe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.mhx1999.top/gtsjdrjhzk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtdxoimtpy.html

JS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtqxigbncz.html

TS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtpygokeuy.html

Java: resp.statusCode()
来源：http://hz.c1oappe.top/gtbqtpllej.html

Go:   resp.StatusCode
来源：http://hz.shanyushiyangkeji.top/gtzsfugvum.html

Ruby: resp.code.to_i
来源：http://hz.bjfxy.top/gtsgjiuzak.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtkixhdfpo.html

[L08] 并发请求多个地址
来源：http://hz.yj20258.top/gtmaontzhx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtiqxnqhvm.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhoulong.xyz/gtnqbohips.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtdhblzwry.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtfxrmmqhe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtzgcepjua.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hongshengwenyu.top/gtakcoavrp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hywenlv.cn/gtdmsbzpke.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtncmguoxq.html

================================================================================
来源：http://hz.fzhhl.top/gtevhrbied.html

M. 命令行 / 进程 / 环境
来源：http://hz.tianlin.xyz/gtduupnuef.html

================================================================================
来源：http://hz.yuanzhike.top/gtdfzevghm.html

[M01] 读取命令行参数
来源：http://hz.snrcjt.cn/gtstichfws.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtderhthtm.html

PHP:  $argv;  $argc;
来源：http://hz.quarkkingdee.top/gtyddnxcvb.html

JS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtjvwzwflj.html

TS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtriwambsz.html

Java: args 数组（main 方法参数）
来源：http://hz.sxryk.cn/gtuioytrsg.html

Go:   os.Args[1:]
来源：http://hz.smart0.xyz/gtdveikqis.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtjirnuwhp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtjygyinbz.html

[M02] 读取环境变量
来源：http://hz.yanxiufei.cn/gtwqnkaxsw.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtnmzbihsb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhoulong.xyz/gtxukcpuco.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gthvpatxsx.html

TS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtzhhnjxnv.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtinucqito.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtcttjddvl.html

Ruby: ENV["HOME"]
来源：http://hz.sysykeji.top/gtesnzehgd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gtjnagkeis.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gteznlpzcy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtvqzuhyax.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jiagoushi.top/gtyjvcwshq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtqqxilywt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtgdfbjoqn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtvqegwvlu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.9152youxi.cn/gtrvqfsxff.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.birdmap.top/gtupkyvonh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dashuyun.cn/gtewtrmydg.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtkscbovcp.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtuonzglby.html

PHP:  getcwd();
来源：http://hz.cashguo.top/gtixtfimiw.html

JS:   process.cwd()
来源：http://hz.yj202588.top/gtuwilbgzn.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtrewooqbo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yueranfly.top/gtdjbicbvh.html

Go:   os.Getwd()
来源：http://hz.aibaodan.cn/gtxbtjishz.html

Ruby: Dir.pwd
来源：http://hz.hongshengwenyu.top/gtpbrbjhzc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtghhxjcee.html

[M05] 设置退出码
来源：http://hz.cheryme.top/gtmwocyvlm.html

Py:   sys.exit(1)
来源：http://hz.jlsjyb.cn/gtqrwjjain.html

PHP:  exit(1);
来源：http://hz.zdqjudy.top/gtoyniuchn.html

JS:   process.exit(1)
来源：http://hz.zycfv.cn/gtdcemafdw.html

TS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtvqjculyf.html

Java: System.exit(1)
来源：http://hz.ivvv.top/gtmrkrlgwk.html

Go:   os.Exit(1)
来源：http://hz.svipenyu.cn/gtnszkvlno.html

Ruby: exit 1
来源：http://hz.xingfuxueyuan.xyz/gtuequzbqz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtpxlewmfa.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtugycivpd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtcwadelai.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yongpay.top/gtmwpdmmox.html

JS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtzokyutdd.html

TS:   console.error("err")
来源：http://hz.ybcxt.top/gtvoicignm.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtwrsyxltz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.52xcode.cn/gtlazmkihz.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtlrkxepez.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yueranfly.top/gtolugupks.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtwfgjejkl.html

Py:   if __name__ == "__main__":
来源：http://hz.yuanzhike.top/gtaasswhll.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gthtbykrka.html

JS:   require.main === module
来源：http://hz.xuanzx.com/gtsfehklao.html

TS:   require.main === module
来源：http://hz.mhx1999.top/gtbjnmnjqs.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gtvalbugpf.html

Go:   func main()
来源：http://hz.zhixingplan.top/gtatsqlzuy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtaljusuyk.html

C#:   static void Main(string[] args)
来源：http://hz.zhixingplan.top/gtevnnuuyk.html

[M08] 获取系统与运行时信息
来源：http://hz.ydzc1.top/gtjpelrfzo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yvedp.cn/gtpxulbpsz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ehwqpu.com/gtvndbrvkd.html

JS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtomafrryx.html

TS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gttqpczdcz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtgjjcnimh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.snrcjt.cn/gtcoccpdsf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtmyifblra.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guowangkeji.top/gtcmdxsgtk.html

================================================================================
来源：http://hz.iojbl.cn/gthhneszpx.html

N. 数据结构与算法
来源：http://hz.sweek.top/gtyjdnuvbn.html

================================================================================
来源：http://hz.xziqi.cn/gttzqrkawu.html

[N01] 二分查找（有序数组）
来源：http://hz.dashuyun.cn/gtmbbnaqdx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tanke756.top/gtzlgenbnj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgfzy.top/gtzogetugr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtnfrxiklf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtzcmpdjtq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtbfxaonwr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangtech.top/gtqibrrxqq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hammf.cn/gtbuaphmxq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtawrykhdr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tian-w.cn/gtidvbwnid.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtcuebozoh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hongshengwenyu.top/gtfcygxsvn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtzftqwnll.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtxiwiswfk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtlubnlgbu.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtxnpcvowg.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtxqnjrnht.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtwanapngo.html

[N03] 快速排序（分治示例）
来源：http://hz.jinghuilouyu.cn/gtnnroyyhg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ehwqpu.com/gtbyryador.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gtpimcxepo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtnaolrzen.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtyamplqya.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtawikmqjz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.iojbl.cn/gtmofuaduk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuanzhike.top/gtkjdswcxo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sysykeji.top/gteqxxpesx.html

[N04] 斐波那契数列
来源：http://hz.andypj.xyz/gtysupkrzk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtwxwlffeq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gzhubu.top/gtbwdlvvui.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtpldlepiv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtnhwcnvzb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yueranfly.top/gtikgszkuh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gtqeykiqix.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtmfmmglpn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.meibo888.top/gtezfnxupb.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtruypinuz.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtkhtkqqyf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daria6918.cn/gtcdekteac.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuanzhike.top/gtbmiebcxk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtatjaodye.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxinkj.top/gtsyiwiwde.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gtrhtgsdza.html

Ruby: a.gcd(b)
来源：http://hz.iojbl.cn/gtbypfbngw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pycfn.com/gtlglrxbxf.html

[N06] 判断回文字符串
来源：http://hz.redwolf501.top/gtotwnpdae.html

Py:   s == s[::-1]
来源：http://hz.yj20258.top/gtmqgzhcyn.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtpverklme.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtgfzakzzw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtffehsbam.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yuanzhike.top/gtfevqvzyv.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigfzy.top/gtoccamnuq.html

Ruby: s == s.reverse
来源：http://hz.aibaodan.cn/gtfhfpqkul.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtrwdooejz.html

[N07] 两数之和（返回下标）
来源：http://hz.cqqwz.cn/gttlacunig.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gteecmbrqg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangshuangyany.cn/gtwjlhtpch.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.kuanghao11.cn/gtmurdzsyr.html

TS:   // 手写 Map<string, number>
来源：http://hz.snrcjt.cn/gtbtfmofwj.html

Java: // 手写 HashMap
来源：http://hz.yanxiufei.cn/gtncilubbj.html

Go:   // 手写 map[int]int
来源：http://hz.nanxuanxn.top/gtkxapxruh.html

Ruby: // 手写 Hash
来源：http://hz.shanyushiyangtech.top/gtomisgxbh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gteumwtpds.html

[N08] 生成全排列
来源：http://hz.gogol.net.cn/gtqiwlzweh.html

Py:   itertools.permutations(arr)
来源：http://hz.shzxlz.cn/gtzwojhiie.html

PHP:  // 手写递归交换
来源：http://hz.vqdsnc.cn/gtmmvbstgh.html

JS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtstxrqrnq.html

TS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtgdiokkde.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtdodznpqu.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtddavponw.html

Ruby: arr.permutation.to_a
来源：http://hz.shzxlz.cn/gtvfduiyns.html

C#:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtztsngeue.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gttremgvpx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zycfv.cn/gtnpfdaafg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtvvcmmqno.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtcjgohign.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yangfankeji.com/gtttpychnq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shuidangran.top/gtjrwhxaoe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hongshengwenyu.top/gthulwwavv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gotoacloud.top/gtzdddranj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.vqdsnc.cn/gtswxbfijv.html

[N10] 链表节点定义
来源：http://hz.gaohongyu789.top/gtpmeqbzwr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgfzy.top/gtrahydxjs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fzhhl.top/gtxogzpakm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zdqjudy.top/gtxdisbdpw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hfpthk.cn/gtlnlzvios.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gtlkcgqlmb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dianchejie.cn/gtyqperlpk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gaohongyu789.top/gtekpisend.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuxming.cn/gtzqkhzetb.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gthjditjwm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxuanxn.top/gtxounazmu.html

PHP:  // 手写递归函数
来源：http://hz.52xcode.cn/gtwbwhgxjq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtfzciojtp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtbqnyxxwg.html

Java: // 手写递归
来源：http://hz.jinghuilouyu.cn/gtoimofixu.html

Go:   // 手写递归
来源：http://hz.yj202588.top/gtvpefckts.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuxming.cn/gtkoileuzr.html

C#:   // 手写递归
来源：http://hz.sysykeji.top/gtervvfvqu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtnrxfmfgf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhiwuduotai.top/gtjwbfwnsz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxinkj.top/gtjvxfbtdm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtlplcnzlt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtrjovclla.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gttdbfdtsf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.feifeiyinyue.top/gtiopkulmg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sysykeji.top/gtgzfxfjgw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtsgtrmcvx.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtarezkbxg.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtehcnlrew.html

================================================================================
来源：http://hz.jinqigfzy.top/gtulxmbklt.html

[O01] 启动一个线程
来源：http://hz.wangshuangyany.cn/gtqtsuysgi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.svipenyu.cn/gtughcoqbn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtlhwymsmy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yonumen.top/gtuuzgdwia.html

TS:   // 同 JS
来源：http://hz.52xcode.cn/gtfpkfbfae.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtgbylehyl.html

Go:   go f()
来源：http://hz.svipenyu.cn/gtgfqdzsyq.html

Ruby: Thread.new { f }
来源：http://hz.yj202588.top/gtzaqpqech.html

C#:   Task.Run(() => F());
来源：http://hz.pycfn.com/gtqmadswhg.html

[O02] 使用线程池
来源：http://hz.hfpthk.cn/gtjrssmsbn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shuidangran.top/gtrnvwkstn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shzxlz.cn/gtvfspfnhl.html

JS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtweamgwym.html

TS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtolmwbmyv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuanzhike.top/gtxisogsfp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tian-w.cn/gttxdfgzjh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aibaodan.cn/gtjexfznwu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuxming.cn/gtbmuunpvi.html

[O03] 加锁保护共享数据
来源：http://hz.hfpthk.cn/gthffrwzwt.html

Py:   with lock: shared += 1
来源：http://hz.ydjk.org.cn/gtulxhjopf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cashguo.top/gtuhmlnzet.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dashuyun.cn/gtoangzvhp.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gthcfygxnq.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gtkroysfty.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtolhxtjvn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.snrcjt.cn/gttgqkerih.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhoulong.xyz/gtbjusomdf.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gtxyfaxaxc.html

Py:   async def f():⏎    await g()
来源：http://hz.aibaodan.cn/gtgisyoblv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258888.top/gtdjxpeoag.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtlidllhok.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnqzz.top/gtiyoytfat.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.316326.xyz/gtgosgyzwr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shzxlz.cn/gtxynwiwna.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gzhubu.top/gtrjkhicds.html

C#:   async Task F() { await G(); }
来源：http://hz.52xcode.cn/gttghyfoxg.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenzaomai.com/gtgkmcvqih.html

Py:   asyncio.gather(*tasks)
来源：http://hz.52xcode.cn/gtncvaihqy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtzpjxbgqt.html

JS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtewwvfrnb.html

TS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtuengifjy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hammf.cn/gtkishzylj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.fzhhl.top/gtdlosdcdw.html

Ruby: threads.map(&:join)
来源：http://hz.ehwqpu.com/gthokvhice.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xziqi.cn/gtmfjohhlz.html

[O06] 使用进程池
来源：http://hz.ywan-chungtsiang.top/gtaxvkldqx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtmefiuskx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cucudq.cn/gtdjrbggsd.html

JS:   // child_process / cluster 模块
来源：http://hz.bjfxy.top/gtrbktnges.html


<!-- 参考信息 -->