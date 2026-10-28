代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtisrbejps.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hongshengwenyu.top/gtkxrtqths.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtqanqatmz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtzddjipti.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hammf.cn/gtqdxqhxbh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.meibo888.top/gtmtnutfxl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhijiandao.cn/gtsassexls.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydzc1.top/gtjvjddayr.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtddhtfpjx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guowangkeji.top/gtebkuqmhn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jianghu66.top/gtuvjljzfe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtogtrcprk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgufenzy.top/gtzalxdmyf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhaomingkeji.xyz/gtwhsiqgjk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuxming.cn/gtztgkqbiq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jyoumei.cn/gtojypkviv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cashguo.top/gtfmzhsoij.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gtzulksfus.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuetiantiany.cn/gtimdgvwwq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shangyingyoupin.top/gtkjlivpsf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtqfgrbxjn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtgsonbtob.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gttplaufwk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnqzz.top/gtllfglwvm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhoulong.xyz/gtdhjwkuli.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtyllcdgnz.html

[L05] 上传文件（multipart）
来源：http://hz.yj202588.top/gtdihbeexw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gtpmewqasb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.52xcode.cn/gtowhqckcf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtemnxagxx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtlfunonip.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtksqvpbqc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ehwqpu.com/gtufymfasw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.bjfxy.top/gttskmfzst.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gtcozstmnz.html

[L06] 解析响应为 JSON
来源：http://hz.nanxinkj.top/gtfhxcrsbi.html

Py:   resp.json()
来源：http://hz.nwbrower.top/gtwlwzodcy.html

PHP:  json_decode($body, true);
来源：http://hz.chenjidiqi.icu/gtvvgsonsk.html

JS:   await resp.json()
来源：http://hz.yj20258.top/gtzztjlzcs.html

TS:   await resp.json()
来源：http://hz.tanke756.top/gtdbihtdha.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtchufobbm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pengpengdd.cyou/gtwwpgsiff.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gogol.net.cn/gtcphccdwa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ivvv.top/gtrjfpbtkb.html

[L07] 处理 HTTP 状态码
来源：http://hz.pycfn.com/gtgwghkgwf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ivvv.top/gtjmhtldvg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtdmhgttxz.html

JS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtbbqjthmh.html

TS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gttgkahqom.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtfdshkgra.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtajzfbokl.html

Ruby: resp.code.to_i
来源：http://hz.hysaishi.cn/gtixzmpqvx.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtirbszybz.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtojyacwsf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhaomingkeji.xyz/gtgxcmxwsc.html

PHP:  curl_multi_init() 系列
来源：http://hz.zdqjudy.top/gtjovetqfq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtaiaasrdp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtnrgmkbxz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtsmbfvrhg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigufen.top/gtaezefcpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtnlpjgady.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jyoumei.cn/gtjgnlcpqz.html

================================================================================
来源：http://hz.redwolf501.top/gtxfbmeieh.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinghuilouyu.cn/gtxyqvcbgq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtiirpntri.html

[M01] 读取命令行参数
来源：http://hz.yj20258888.top/gtvgcalhdl.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtqtmzkxnz.html

PHP:  $argv;  $argc;
来源：http://hz.hongshengwenyu.top/gtrcfhmipx.html

JS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtixsspipb.html

TS:   process.argv.slice(2)
来源：http://hz.yueranfly.top/gtrznoptkq.html

Java: args 数组（main 方法参数）
来源：http://hz.52xcode.cn/gtrgoxubof.html

Go:   os.Args[1:]
来源：http://hz.iojbl.cn/gtbqctebav.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gttesgawyr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj202588.top/gtcsjnbxav.html

[M02] 读取环境变量
来源：http://hz.xylfe.cn/gtnqtiezfx.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gtlghmhapf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtvwgwyzrg.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtvqpuryrb.html

TS:   process.env.HOME
来源：http://hz.sweek.top/gtozabstty.html

Java: System.getenv("HOME")
来源：http://hz.yj20258.top/gtcsyjyfzm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daria6918.cn/gtdwazqlrz.html

Ruby: ENV["HOME"]
来源：http://hz.yongpay.top/gthcumsgqv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgfzy.top/gtnezzxykp.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtqeyhxxhl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guowangkeji.top/gthluuugbi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zycfv.cn/gtafvrwfli.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtmlpfwolw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtdobhlptn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtkbfnybpz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tanke756.top/gtiqodjojv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guannengcc.top/gtbznhxheu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtesezoamk.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtgrqnkhey.html

Py:   os.getcwd()
来源：http://hz.kuanghao11.cn/gtioptkgze.html

PHP:  getcwd();
来源：http://hz.xuanzx.com/gtuieoktey.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtaawdtzag.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtddtbrjmv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jyoumei.cn/gtzozbovkh.html

Go:   os.Getwd()
来源：http://hz.snrcjt.cn/gtvplcyavh.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangtech.top/gtlochgwbg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnqzz.top/gtvmnmkusa.html

[M05] 设置退出码
来源：http://hz.tanke756.top/gtfmvgeymk.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtjsvnvrau.html

PHP:  exit(1);
来源：http://hz.gogol.net.cn/gtrhnkjjmm.html

JS:   process.exit(1)
来源：http://hz.tanke756.top/gtzfacxijp.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gtnmwiuhkw.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtfsxptjav.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gturgyzien.html

Ruby: exit 1
来源：http://hz.svipenyu.cn/gtqjguyiii.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shuidangran.top/gttraipxed.html

[M06] 向标准错误输出
来源：http://hz.cashguo.top/gtnrvfmpol.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhengqikj.top/gtwplvekwb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtijoyvyye.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtfobayqwc.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gthvrjwbmn.html

Java: System.err.println("err")
来源：http://hz.ehwqpu.com/gtdzryggwp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtglqlebnm.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gttdcgzakt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gtakqilgic.html

[M07] 判断是否为主入口
来源：http://hz.cheryme.top/gtpvfdssyt.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258888.top/gthozolyfw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.kuanghao11.cn/gtgoinwmki.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gtcjbefhby.html

TS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtamcavaoz.html

Java: public static void main(String[] args)
来源：http://hz.zhaomingkeji.xyz/gtpkomtmvg.html

Go:   func main()
来源：http://hz.ehwqpu.com/gtcirpzcnx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hfpthk.cn/gtcfdaxyqi.html

C#:   static void Main(string[] args)
来源：http://hz.aibaodan.cn/gtzslaezgj.html

[M08] 获取系统与运行时信息
来源：http://hz.yuanzhike.top/gtjibuatua.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtwjqnxvcf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.0kj1m.cn/gtxmgbddaj.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtjxcntzox.html

TS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gthbwwpuov.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhijiandao.cn/gtpfraurgp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.52xcode.cn/gtdmnplkxw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtfsgbfewg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.mhx1999.top/gtzqcmcvgp.html

================================================================================
来源：http://hz.vqdsnc.cn/gthzousfdv.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtgbjecayq.html

================================================================================
来源：http://hz.bjfxy.top/gtddmffyia.html

[N01] 二分查找（有序数组）
来源：http://hz.andypj.xyz/gtfpxmuxvv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtsdhkntsp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.c1oappe.top/gtigyheaxa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtbmwtawyf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtxchzemnm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtgdrpdbmp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jlsjyb.cn/gtkrtgdhej.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hysaishi.cn/gteekcolto.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtabwfxmit.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258888.top/gtkzinavlm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtieixiedi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtterjqtuf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtvgrbfvep.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtsdhwjiys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daxiang520.top/gteerckldi.html

Go:   slices.Sort(arr)
来源：http://hz.gaohongyu789.top/gtvkmuffqo.html

Ruby: arr.sort
来源：http://hz.dashuyun.cn/gtnhqquota.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtadiyrzak.html

[N03] 快速排序（分治示例）
来源：http://hz.52xcode.cn/gtybsstapg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ppjwa.cn/gtwzqpucwz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuanzx.com/gtjrvrbfgz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtpmfrgadw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtljgsufbs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtostqkxby.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ivvv.top/gtvotidwmm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtuyyzimwk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtavwdhuvf.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtolndectv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtqziugzwn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gtlcriqhch.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtmomalgqp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtynejkpke.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hfpthk.cn/gtznoogmcr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dashuyun.cn/gtdiamtbgp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtcdoedqrr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtzdbdkzvm.html

[N05] 最大公约数
来源：http://hz.cqqwz.cn/gtcqneuftp.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtnvuwqwfh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtprkzdrsk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtuddnvhcf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gthsxzcnab.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sxryk.cn/gtwvfcjrqf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yongpay.top/gtuxexbmdm.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtryqwfeje.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xingfuxueyuan.xyz/gtvrbgctge.html

[N06] 判断回文字符串
来源：http://hz.sufxvd.cn/gtrzscvuio.html

Py:   s == s[::-1]
来源：http://hz.yonumen.top/gtokbqlrbe.html

PHP:  $s === strrev($s);
来源：http://hz.tian-w.cn/gtdjqrrguy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtzenihbzw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gttvjyzuvy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgufenzy.top/gtuxsszqqu.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtbfnlrmhs.html

Ruby: s == s.reverse
来源：http://hz.andypj.xyz/gtvxqcfuhi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtryopwmpz.html

[N07] 两数之和（返回下标）
来源：http://hz.nanxuanxn.top/gtmkaccusz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xinyue.icu/gtlpwxaylc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gtoyjyleuy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.redwolf501.top/gtffiiaojr.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuxming.cn/gtaaxwvolx.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtfckzhlwj.html

Go:   // 手写 map[int]int
来源：http://hz.haohaochexian.top/gtjghhdqle.html

Ruby: // 手写 Hash
来源：http://hz.yangfankeji.com/gtrfwpqikl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtduwdruho.html

[N08] 生成全排列
来源：http://hz.cdnleiting.top/gtxbhyhdfg.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtnkbadbaw.html

PHP:  // 手写递归交换
来源：http://hz.jinqigfzy.top/gtevkursik.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtcdlnyuvv.html

TS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtuinehouf.html

Java: // 手写回溯递归
来源：http://hz.yonumen.top/gtqcgvkzwd.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtbrgswyzo.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtqgxvlsxu.html

C#:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtdgwxsifu.html

[N09] 栈与队列
来源：http://hz.yj20258.top/gtrssydubq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sweek.top/gtfguwdfpk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xylfe.cn/gtcnzrkgty.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gotoacloud.top/gtgdgqqlhs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigfzy.top/gtlaswchza.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtfxxgycub.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gaohongyu789.top/gthtiwrtjj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shuidangran.top/gtkfaxewpj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenzaomai.com/gtatleewgf.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtozyuydlw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.havefunace.top/gtwjcjoffz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.vqdsnc.cn/gtvcvlyteu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ybcxt.top/gtjunfnbvx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangtech.top/gtrkrvkziu.html

Java: class Node { int v; Node next; }
来源：http://hz.yj202588.top/gtusjazdeh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangkeji.top/gtefxtfnta.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hysaishi.cn/gtpzqifecp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuanzx.com/gtpumkvbih.html

[N11] 二叉树中序遍历
来源：http://hz.ehwqpu.com/gtufywmohw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yvedp.cn/gtjkehgerh.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtpewticbz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtynlzmznt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtptjnhixh.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtiqqkdnyh.html

Go:   // 手写递归
来源：http://hz.guannengcc.top/gtcxyjpnbz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhaomingkeji.xyz/gtnimpasca.html

C#:   // 手写递归
来源：http://hz.gogol.net.cn/gtnzrewphs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jlsjyb.cn/gtktzrcdns.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gzhubu.top/gtcxqanggs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gtkhlcpmyc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtjnpnrtnl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtbsdqslil.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtdbsjfvut.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtxbxmifqj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jlsjyb.cn/gtiovsnusk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jyoumei.cn/gtlvjouaiy.html

================================================================================
来源：http://hz.0kj1m.cn/gtsflegmdd.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtqdriwlyx.html

================================================================================
来源：http://hz.hysaishi.cn/gtrqqetsqf.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtssqytyhq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ywan-chungtsiang.top/gttoovpihr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xingfuxueyuan.xyz/gtxiesookh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.kuanghao11.cn/gtyvwumdtt.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gtydgfhwpt.html

Java: new Thread(() -> f()).start()
来源：http://hz.meibo888.top/gtuyzposjf.html

Go:   go f()
来源：http://hz.zhixingplan.top/gtuudsdzjv.html

Ruby: Thread.new { f }
来源：http://hz.zhaomingkeji.xyz/gtqwpxpfoe.html

C#:   Task.Run(() => F());
来源：http://hz.sxryk.cn/gtzjcrciec.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gtvzpxpznq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gotoacloud.top/gtlcewycrd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sxryk.cn/gtyyopgcmb.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtdsekktgi.html

TS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtfxuauwpk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aizwys.cn/gtwatzkjpu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tanke756.top/gtumjtpsgb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gtknvgadrt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.mhx1999.top/gtiqvxcwvj.html

[O03] 加锁保护共享数据
来源：http://hz.cqqwz.cn/gtptbtueap.html

Py:   with lock: shared += 1
来源：http://hz.zycfv.cn/gtpxormpyl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gthouevhjz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hammf.cn/gtedynsaca.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gtlncpsthl.html

Java: synchronized (this) { shared++; }
来源：http://hz.xziqi.cn/gtmszlagri.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenlongwang.top/gtipumlffm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxuanxn.top/gtlwhbkddi.html

C#:   lock (gate) { shared++; }
来源：http://hz.fengsongda.top/gtagwaygbt.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gtvqdajeca.html

Py:   async def f():⏎    await g()
来源：http://hz.zhoulong.xyz/gtanaxexam.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xylfe.cn/gtylqaddqv.html

JS:   async function f() { await g(); }
来源：http://hz.yonumen.top/gtsepjakdy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cucudq.cn/gtloeiqgyn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.0kj1m.cn/gtuygrlgmi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtovhhrvxw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtaazyaoaf.html

C#:   async Task F() { await G(); }
来源：http://hz.xuanzx.com/gtjnfonwxl.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgfzy.top/gtityijvtv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnxiangtu.top/gtlexkblnq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nwbrower.top/gtxssygbcy.html

JS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtkutxfimx.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtklttmefn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.iojbl.cn/gtstrhnkuu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.vqdsnc.cn/gtqlfuernc.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtldycxaoo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jiagoushi.top/gtwftslpph.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtskwontzq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cdnleiting.top/gtoswkusee.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydzc1.top/gtypfftqzb.html

JS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtiuwdbtyg.html


<!-- 参考信息 -->