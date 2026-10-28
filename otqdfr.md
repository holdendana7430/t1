代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtondizrvi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gtaswzceqc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jianghu66.top/gtcbrvlowa.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtehertlmw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xziqi.cn/gtyriowfow.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shuidangran.top/gtncrrakcj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtslhnebwk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtuxobqgfn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daxiang520.top/gtzfgkhmgk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gzhubu.top/gteckkwekj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhaomingkeji.xyz/gtkalgnycx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fengsongda.top/gtekhbovmi.html

[L03] 设置自定义请求头
来源：http://hz.gaohongyu789.top/gtppbmxnjj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtlzcrswhi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ppjwa.cn/gtlzsqwoht.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtatarkqnd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtasozprbc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dashuyun.cn/gttsxwrvgq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtfdjznqpb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fzhhl.top/gtqvczozbk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydjk.org.cn/gtcnxyslek.html

[L04] 设置超时
来源：http://hz.guowangkeji.top/gtkbeeiylm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhoulong.xyz/gtwsbzuogb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgfzy.top/gtzmbwfodn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtzisbihha.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtwbryirdq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtmocywmnz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtlszmfbmm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daxiang520.top/gtyagzajpi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangdashe.top/gtdfwdafps.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258.top/gtlszwdqvw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtodjzdghc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.iojbl.cn/gtkepkrygw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtelxnusft.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtpeqnnanx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hywenlv.cn/gtmmtuurqz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.bjfxy.top/gtpshsdwkr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aibaodan.cn/gtwzqvnxxz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtcgjhxbwj.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtinrxsnlz.html

Py:   resp.json()
来源：http://hz.jlsjyb.cn/gtgjvyykmt.html

PHP:  json_decode($body, true);
来源：http://hz.shzxlz.cn/gtojuaqkmo.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtkjiqqffv.html

TS:   await resp.json()
来源：http://hz.hfpthk.cn/gtxkvbehvr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.c1oappe.top/gtjpzbrcdu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnxiangtu.top/gtigkcfypb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xziqi.cn/gtrtxkrgld.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sweek.top/gtzipehwsj.html

[L07] 处理 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtuhsxxjcj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgfzy.top/gtdbckcjhd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ppjwa.cn/gtublxqrxv.html

JS:   resp.ok;  resp.status
来源：http://hz.52xcode.cn/gtbfnkylun.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtqzyrlvnm.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gtdleoayfs.html

Go:   resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtlszyscel.html

Ruby: resp.code.to_i
来源：http://hz.andypj.xyz/gtjxpcgykn.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gtakodalcg.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtuzfkxnaw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtpzlmslue.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtbvoiwmwv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtjhyxgrtd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtfmbhcxvw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gtusnahgal.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangdashe.top/gtcuyxkocl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtzhaugbgr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtkxvvjzzy.html

================================================================================
来源：http://hz.cheryme.top/gtpejnnqhe.html

M. 命令行 / 进程 / 环境
来源：http://hz.svipenyu.cn/gtgconfdwp.html

================================================================================
来源：http://hz.xuanzx.com/gtciezmogn.html

[M01] 读取命令行参数
来源：http://hz.ydjk.org.cn/gtzpkoszqy.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangtech.top/gtsprhaaih.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangkeji.top/gtfuyrladd.html

JS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gthicqlvuu.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtqqbxtqox.html

Java: args 数组（main 方法参数）
来源：http://hz.ydjk.org.cn/gtfmkgsgys.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtopswyryr.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtrvrxhhha.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xylfe.cn/gtabataibv.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtpamyncer.html

Py:   os.environ.get("HOME")
来源：http://hz.hysaishi.cn/gttkzgffdt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ivvv.top/gtucczlcba.html

JS:   process.env.HOME
来源：http://hz.iojbl.cn/gtjnixidom.html

TS:   process.env.HOME
来源：http://hz.yj20258888.top/gtaplqaluv.html

Java: System.getenv("HOME")
来源：http://hz.ydjk.org.cn/gtjlppibja.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigfzy.top/gtobvmrjyu.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtspzbwnqu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gaohongyu789.top/gtmczilszo.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gtuaamwskt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinyuanbaomall.cn/gtervyhjff.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gtnfchcxgv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtswgjiyqi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtwwpeciyr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258.top/gtzkwfflzk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yueranfly.top/gthojkwdao.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ehwqpu.com/gtccginoyh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtxrnfnnju.html

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gtrpmldbya.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtcfswtgez.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtefwogabi.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gtdwjsurzw.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtdzyjdail.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtrdfuotun.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtvftarnid.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtlwngcsif.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.snrcjt.cn/gtqvqskzqs.html

[M05] 设置退出码
来源：http://hz.redwolf501.top/gtefsocflm.html

Py:   sys.exit(1)
来源：http://hz.nwbrower.top/gtizlmzvin.html

PHP:  exit(1);
来源：http://hz.aizwys.cn/gtafnlkgni.html

JS:   process.exit(1)
来源：http://hz.iojbl.cn/gtuqpnddia.html

TS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtfxafjyov.html

Java: System.exit(1)
来源：http://hz.daria6918.cn/gtsmppjrbx.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtvobonnle.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtfmhwrwrb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinghuilouyu.cn/gtittxgtps.html

[M06] 向标准错误输出
来源：http://hz.birdmap.top/gtsntecpue.html

Py:   print("err", file=sys.stderr)
来源：http://hz.snrcjt.cn/gtydrfdgqs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hammf.cn/gtgamwsbrn.html

JS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtqfiydmae.html

TS:   console.error("err")
来源：http://hz.ydzc1.top/gtxchmdqtj.html

Java: System.err.println("err")
来源：http://hz.jianghu66.top/gtkczlmkns.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gtuvygesze.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtqildnpmx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgufenzy.top/gtgnawebfq.html

[M07] 判断是否为主入口
来源：http://hz.shuidangran.top/gtdedgykqh.html

Py:   if __name__ == "__main__":
来源：http://hz.dashuyun.cn/gtnrkrwiaw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtdlbjifma.html

JS:   require.main === module
来源：http://hz.shzxlz.cn/gtkfqgtltm.html

TS:   require.main === module
来源：http://hz.tianlin.xyz/gtrgnwyjkl.html

Java: public static void main(String[] args)
来源：http://hz.zhijiandao.cn/gtetxwmfpl.html

Go:   func main()
来源：http://hz.hammf.cn/gtdqgjtjzh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.0kj1m.cn/gtyaufeghh.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtpxuffqha.html

[M08] 获取系统与运行时信息
来源：http://hz.chenzaomai.com/gtresyfgtw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.vqdsnc.cn/gtzpddyfhj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xylfe.cn/gtuwwtwvce.html

JS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtkoojxomb.html

TS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtisvrmlkw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangtech.top/gtqqkdoawx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtbxexankh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtsfiuitqf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gotoacloud.top/gtrysdpeau.html

================================================================================
来源：http://hz.nanxinkj.top/gtuyukorst.html

N. 数据结构与算法
来源：http://hz.yj20258888.top/gtrhvrkduw.html

================================================================================
来源：http://hz.aizwys.cn/gtzequesik.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtrfyszwyq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigfzy.top/gthujiirwb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtgrytfpsg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtiacrqzgk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtdxvwbaoo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gthbwqdgdh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cucudq.cn/gtxgowyfjt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.52xcode.cn/gtcubaxrzh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hysaishi.cn/gtqncqrytm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.birdmap.top/gttyawemkg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtvwmivnsx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtcrrhykgk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtpwqrfuvy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtyoszhsvy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cdnleiting.top/gteewackrv.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtiimynveo.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtakukhbxo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gtzppdqooi.html

[N03] 快速排序（分治示例）
来源：http://hz.xuetiantiany.cn/gtdtgidooz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ehwqpu.com/gtyvvahgfp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.redwolf501.top/gtwfqctara.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtlwezqhuh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtodxsbchi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.havefunace.top/gtwridmysz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nwbrower.top/gtpyieallq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtunlxnkzh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenjidiqi.icu/gtsyfevzos.html

[N04] 斐波那契数列
来源：http://hz.birdmap.top/gttmrhbbca.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtcgpuadgk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtqbkdpico.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtxlzwpocg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtupyjffoa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xylfe.cn/gtirgjwcra.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinghuilouyu.cn/gteumgrpwr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtkvauxoyt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gotoacloud.top/gtznezurgy.html

[N05] 最大公约数
来源：http://hz.yj202588.top/gtrwvtnjju.html

Py:   math.gcd(a, b)
来源：http://hz.andypj.xyz/gtyxieueiu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aibaodan.cn/gtouhuyymh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtlgzkptdt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtknxrzpuw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.haohaochexian.top/gtcctdxbjn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtkfcqduxg.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtzitftqyq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtjsfzooyj.html

[N06] 判断回文字符串
来源：http://hz.hongshengwenyu.top/gteebphxwk.html

Py:   s == s[::-1]
来源：http://hz.yvedp.cn/gtplrczcee.html

PHP:  $s === strrev($s);
来源：http://hz.yj202588.top/gtpiukeeyu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtvnbnwhkw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtfhnfdnvz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtxilxljjt.html

Go:   // 双指针从两端比较
来源：http://hz.xingfuxueyuan.xyz/gtcyayndof.html

Ruby: s == s.reverse
来源：http://hz.jlsjyb.cn/gtejmjmbio.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gtketfleat.html

[N07] 两数之和（返回下标）
来源：http://hz.hnxiangtu.top/gtbytagjro.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.feifeiyinyue.top/gtlhlannkj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinyuanbaomall.cn/gtrsbbktqb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.quarkkingdee.top/gtespgaeyu.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gtmnkehfyq.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtlgwvlwmh.html

Go:   // 手写 map[int]int
来源：http://hz.zhengqikj.top/gtsgewmsmf.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gttuobypis.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cheryme.top/gtjwzydjkq.html

[N08] 生成全排列
来源：http://hz.jiagoushi.top/gtenbijwxx.html

Py:   itertools.permutations(arr)
来源：http://hz.yueranfly.top/gtwqudspkt.html

PHP:  // 手写递归交换
来源：http://hz.zhoulong.xyz/gtfompxfvl.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtbjetbxdd.html

TS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gteewolavs.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtdaozqhxq.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtyfbechsj.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtmomrryql.html

C#:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtqygfsrpn.html

[N09] 栈与队列
来源：http://hz.yuanzhike.top/gtjjwqtpbf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtnkzdmmbr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zdqjudy.top/gtwljaytuv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258888.top/gtelbmrfyz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtwjbjbtdw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hongshengwenyu.top/gtnaldcijd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yangfankeji.com/gtzlpdklqj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenzaomai.com/gtwqcjevjl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ywan-chungtsiang.top/gtxphagesw.html

[N10] 链表节点定义
来源：http://hz.sxryk.cn/gtjumpgpio.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daxiang520.top/gtkwomwmly.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydzc1.top/gtbwrnyxos.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jyoumei.cn/gteibjqofc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jiagoushi.top/gtjevducil.html

Java: class Node { int v; Node next; }
来源：http://hz.ehwqpu.com/gtnewmqjcv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aibaodan.cn/gtfbrwvrxm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangtech.top/gtlxksaqos.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gternljfbn.html

[N11] 二叉树中序遍历
来源：http://hz.chenzaomai.com/gtbezjjgvu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ehwqpu.com/gtsxkqnwil.html

PHP:  // 手写递归函数
来源：http://hz.zdqjudy.top/gtslsngglz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xziqi.cn/gtuiidhdfs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtxsotuzcl.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtudgqmznd.html

Go:   // 手写递归
来源：http://hz.yuanzhike.top/gtpomhfnjk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guannengcc.top/gtpfgnhswq.html

C#:   // 手写递归
来源：http://hz.sysykeji.top/gtgpgiiynl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtlphkexox.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ppjwa.cn/gtshmafhiu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guannengcc.top/gtskmothpw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gtkxdwvooo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtzipmbcuu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtldlmjwpj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daxiang520.top/gtxcgjakwg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenlongwang.top/gtgmlfjdyb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtvmrlbqia.html

================================================================================
来源：http://hz.pycfn.com/gtmeshqhvb.html

O. 并发与异步
来源：http://hz.yangfankeji.com/gtlekpfrgi.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkgspmfwd.html

[O01] 启动一个线程
来源：http://hz.dianchejie.cn/gtfekcclrx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yonumen.top/gtnlmnznln.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gtkeuoeyau.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yueranfly.top/gtbbgyplfu.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtuwxtymrf.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gttoaywjgg.html

Go:   go f()
来源：http://hz.xinyue.icu/gtzrfaskdx.html

Ruby: Thread.new { f }
来源：http://hz.hammf.cn/gttjothbmn.html

C#:   Task.Run(() => F());
来源：http://hz.haohaochexian.top/gtugaanark.html

[O02] 使用线程池
来源：http://hz.dashuyun.cn/gtfobgyjyi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gtxurqlrkl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gtthiyloct.html

JS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtkmijinkt.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtmfcflqec.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtimzacpnq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnxiangtu.top/gtkrdskaqk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jlsjyb.cn/gtxvtdqknn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jqgfzy.top/gtutdvxwku.html

[O03] 加锁保护共享数据
来源：http://hz.yanxiufei.cn/gtzgugthbz.html

Py:   with lock: shared += 1
来源：http://hz.zhoulong.xyz/gtkfkzjqzs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.bjfxy.top/gtispvsjgw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cqqwz.cn/gtpoboiqsc.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gttdmpqkuu.html

Java: synchronized (this) { shared++; }
来源：http://hz.c1oappe.top/gtynamctum.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.vqdsnc.cn/gtczfhbpzp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtshskquac.html

C#:   lock (gate) { shared++; }
来源：http://hz.yvedp.cn/gtomqbgbhc.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gtharmkygf.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtahhcgrmp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxuanxn.top/gtfuxnzhzb.html

JS:   async function f() { await g(); }
来源：http://hz.chenjidiqi.icu/gtmtehghfl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pycfn.com/gtqurrcdzx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shangyingyoupin.top/gtobllwbqf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258888.top/gthxqitrtm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.316326.xyz/gtivllkdcz.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtkcalicfv.html

[O05] 并发执行并等待全部完成
来源：http://hz.xziqi.cn/gtvtqkpeit.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhengqikj.top/gtkjiwuhgq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gtiraoxecc.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtfavhbgfl.html

TS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gttdsiggwb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yangfankeji.com/gtchfvvumr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cheryme.top/gtoxdadeij.html

Ruby: threads.map(&:join)
来源：http://hz.jqgufenzy.top/gtpwqisxom.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgfzy.top/gtjsnawoke.html


<!-- 参考信息 -->