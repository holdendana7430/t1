代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtfschfeak.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.feifeiyinyue.top/gtaxfrspyh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtmgofzecv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtguuaasbx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtasvrrwhm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gzhubu.top/gtdjolqebx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dianchejie.cn/gtwhlczbrn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.kuanghao11.cn/gtxrldcvoy.html

[L03] 设置自定义请求头
来源：http://hz.zhixingplan.top/gtpvkewnup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtivypowin.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nwbrower.top/gtxfyedcxq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtthvkxvxq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtowiepdgm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gogol.net.cn/gtqzertogr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtbwcqbxeo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hammf.cn/gtkkpdrane.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtmgtztitf.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtriywdnlj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sweek.top/gtmjeyndwn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xuetiantiany.cn/gtofsenuyq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtbtwrrude.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtiphkcbxy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtfekhnmfv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhixingplan.top/gtrfpbqcoc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtzrjkdvyl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.9152youxi.cn/gtacwcklwh.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtzidnczlo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhijiandao.cn/gtodrkhqji.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.birdmap.top/gtsrvzlzxd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gturbivbhi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtedllrsqy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtmlhqxugj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gtvwazpvco.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gthvtnknij.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.316326.xyz/gtfupiabmt.html

[L06] 解析响应为 JSON
来源：http://hz.vqdsnc.cn/gtaegfikic.html

Py:   resp.json()
来源：http://hz.daxiang520.top/gtdugsyrgs.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gtbzirzpoh.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtawzoiaid.html

TS:   await resp.json()
来源：http://hz.yvedp.cn/gtyimnkhlx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shzxlz.cn/gtsifwfbuc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ywan-chungtsiang.top/gtejixyrme.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuetiantiany.cn/gtejwqcmfa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nwbrower.top/gtpwkzabfz.html

[L07] 处理 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtigcpwwjy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cucudq.cn/gtyzytmnju.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtowqlonxs.html

JS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gthckahbvi.html

TS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtxoqlkmyo.html

Java: resp.statusCode()
来源：http://hz.shuidangran.top/gtajzyfthp.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtleyvwdag.html

Ruby: resp.code.to_i
来源：http://hz.cashguo.top/gtjoshttxw.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgfzy.top/gtlcqrxqnt.html

[L08] 并发请求多个地址
来源：http://hz.shangyingyoupin.top/gtrnaavkuc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj202588.top/gtpijehnge.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtgsvxqrkf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtzscurgjg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtgwyunkil.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.9152youxi.cn/gtajkhcgjc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangtech.top/gtmmsxyufi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pengpengdd.cyou/gtcbczikay.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtswtmgims.html

================================================================================
来源：http://hz.mhx1999.top/gtfzgraqwt.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtdulksmqo.html

================================================================================
来源：http://hz.sxryk.cn/gtqghrsoli.html

[M01] 读取命令行参数
来源：http://hz.zhengqikj.top/gtcldenurz.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gtinrnsdih.html

PHP:  $argv;  $argc;
来源：http://hz.yueranfly.top/gttvomlxkk.html

JS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtctwdtgaq.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtcukasfoc.html

Java: args 数组（main 方法参数）
来源：http://hz.meibo888.top/gttxjronse.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtvckgxcah.html

Ruby: ARGV
来源：http://hz.ydjk.org.cn/gtiqtlqfos.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtvxuilsht.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtuiqrmopu.html

Py:   os.environ.get("HOME")
来源：http://hz.yongpay.top/gtoezxbyoh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtyfwcpscb.html

JS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtvlcqvbyu.html

TS:   process.env.HOME
来源：http://hz.xinyue.icu/gtqrcjyitk.html

Java: System.getenv("HOME")
来源：http://hz.gzhubu.top/gtlxreybir.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenzaomai.com/gtluqstsdc.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtvdaiucdg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtxggekbls.html

[M03] 执行外部命令
来源：http://hz.yangfankeji.com/gtyyenpevb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhongyouzk.top/gtdufxcnqp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xziqi.cn/gtefbunutr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtctomjwpx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtdsifrkqz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtclqjxcxu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gtbwuocsqu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.iojbl.cn/gtfqlqglla.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gtqdkgyscs.html

[M04] 获取当前工作目录
来源：http://hz.gzhubu.top/gtudvhizzq.html

Py:   os.getcwd()
来源：http://hz.c1oappe.top/gtwschctcs.html

PHP:  getcwd();
来源：http://hz.wangshuangyany.cn/gtuzacrnty.html

JS:   process.cwd()
来源：http://hz.aibaodan.cn/gtbhrfygqj.html

TS:   process.cwd()
来源：http://hz.shzxlz.cn/gtkqwxrkpp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pengpengdd.cyou/gtqhnyatai.html

Go:   os.Getwd()
来源：http://hz.dianchejie.cn/gtfcavanjp.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtrvtzwysr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtbhwuaccy.html

[M05] 设置退出码
来源：http://hz.hfpthk.cn/gtfpuztbsw.html

Py:   sys.exit(1)
来源：http://hz.ydzc1.top/gthubueatz.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gtcmofwrtg.html

JS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtwpwlgejk.html

TS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtqkaekrgn.html

Java: System.exit(1)
来源：http://hz.zhijiandao.cn/gtwvsgplpf.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtfikzvbie.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtygrdaaal.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtrsrluhkh.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtpyvjwhat.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtajcxlkym.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xinyue.icu/gtnjxyiexm.html

JS:   console.error("err")
来源：http://hz.sysykeji.top/gtkbsflyqq.html

TS:   console.error("err")
来源：http://hz.c1oappe.top/gtsgbrjemb.html

Java: System.err.println("err")
来源：http://hz.mhx1999.top/gtlgdwcgav.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuxming.cn/gtmirtsyvn.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gtmvhcjewb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtxejibukh.html

[M07] 判断是否为主入口
来源：http://hz.jqgfzy.top/gtwqndmcbz.html

Py:   if __name__ == "__main__":
来源：http://hz.guowangkeji.top/gtuezqajov.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenzaomai.com/gtkdfljniq.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gtcextekcz.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gthcobrpen.html

Java: public static void main(String[] args)
来源：http://hz.nwbrower.top/gtakorjyes.html

Go:   func main()
来源：http://hz.cucudq.cn/gtvohakdlz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangtech.top/gtnmfhbkio.html

C#:   static void Main(string[] args)
来源：http://hz.daria6918.cn/gtfegmuhsr.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtsfnyfgfo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtagsggrja.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhaomingkeji.xyz/gtujgzziiy.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gttmtbmkfv.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtdxcpisjy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtdoylnlxn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yvedp.cn/gtdrmugkip.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxinkj.top/gtilgdqgks.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sweek.top/gtruzbyvfh.html

================================================================================
来源：http://hz.xinyue.icu/gtytkiyval.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gtnvtbpoat.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvseecjvg.html

[N01] 二分查找（有序数组）
来源：http://hz.aibaodan.cn/gtytbprito.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aibaodan.cn/gtjbollsxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtkedrziys.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtohkunfcm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtmqyvdhbz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuanzx.com/gteedlqgzd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.birdmap.top/gtfcasvnto.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydzc1.top/gtdtwihkrj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtwgzvtpeo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtoogvodul.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtialcivvo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sysykeji.top/gtypfhnges.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtnzoahdwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtiabwjrre.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daria6918.cn/gtjtfkegeg.html

Go:   slices.Sort(arr)
来源：http://hz.gzhubu.top/gtnfoedhgd.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtckznkiuk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtkseukzki.html

[N03] 快速排序（分治示例）
来源：http://hz.redwolf501.top/gtkxtihzmz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.quarkkingdee.top/gtsaribkrk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.quarkkingdee.top/gtqzrmsucy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnxiangtu.top/gthynkrsxz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtmrdiqxbs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yangfankeji.com/gtymyjtyrg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gogol.net.cn/gtozckxxpq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtssroguzv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtsxrhhfnu.html

[N04] 斐波那契数列
来源：http://hz.shangyingyoupin.top/gtnplyaehy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtpgwrtdeg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.snrcjt.cn/gtqhwrvxya.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtujcdqwfe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gttgydxsxm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtekqxxpvg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.guowangkeji.top/gtbizxusam.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtzfnxoxid.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.316326.xyz/gtybppyqyd.html

[N05] 最大公约数
来源：http://hz.sufxvd.cn/gtrllwdych.html

Py:   math.gcd(a, b)
来源：http://hz.ppjwa.cn/gtwrdyuytr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenlongwang.top/gtlcezilym.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtmpngzcsi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtrjhbrjca.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtekhaiecb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigufen.top/gteywnkreb.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtvkbiwlyv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtbbpigwwl.html

[N06] 判断回文字符串
来源：http://hz.yj20258888.top/gtpsozumip.html

Py:   s == s[::-1]
来源：http://hz.hammf.cn/gteqxkxtvt.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtvufiluuy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtzlpzzdcp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtpsgyqjqh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gogol.net.cn/gttcmzdqnp.html

Go:   // 双指针从两端比较
来源：http://hz.wangshuangyany.cn/gtfstfbrcw.html

Ruby: s == s.reverse
来源：http://hz.sufxvd.cn/gtotoiccpy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtzsvaefoq.html

[N07] 两数之和（返回下标）
来源：http://hz.jinghuilouyu.cn/gtjlvwckhw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.9152youxi.cn/gtqdhpywiy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gtuoqzrwbb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtdpowntle.html

TS:   // 手写 Map<string, number>
来源：http://hz.haohaochexian.top/gtqkvsbuzn.html

Java: // 手写 HashMap
来源：http://hz.nanxuanxn.top/gtebrbdyjz.html

Go:   // 手写 map[int]int
来源：http://hz.jinghuilouyu.cn/gtbkbbdorh.html

Ruby: // 手写 Hash
来源：http://hz.gzhubu.top/gtshevsxae.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigufen.top/gtipgoijzc.html

[N08] 生成全排列
来源：http://hz.aizwys.cn/gtejyifvnz.html

Py:   itertools.permutations(arr)
来源：http://hz.gaohongyu789.top/gtmxoobdaf.html

PHP:  // 手写递归交换
来源：http://hz.sxryk.cn/gtooxohbrp.html

JS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtolzvpnoc.html

TS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtlojkwrbd.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gtpaictutw.html

Go:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtmgcmtecn.html

Ruby: arr.permutation.to_a
来源：http://hz.zhoulong.xyz/gtjxallslw.html

C#:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gthkwwlpyz.html

[N09] 栈与队列
来源：http://hz.yanxiufei.cn/gtmxhxomnp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgufenzy.top/gttwnlztjy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gtnjhdsdrb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gtkfannmno.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gthjpcnzcx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuanzx.com/gtijzknxwv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtnhkuejpv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnxiangtu.top/gtmoyowimw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.snrcjt.cn/gtcpoxfbml.html

[N10] 链表节点定义
来源：http://hz.hywenlv.cn/gtvaciqqtf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cashguo.top/gtpsslyeij.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yongpay.top/gtzvzwskvn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.smart0.xyz/gtshfdiuhj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangdashe.top/gtbhhxymqh.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258.top/gtqdlecbnw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xylfe.cn/gtcfstgkiz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xylfe.cn/gtqcaynkxt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fengsongda.top/gtoubjuqre.html

[N11] 二叉树中序遍历
来源：http://hz.shuidangran.top/gtfmgndfqp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.mhx1999.top/gterwlpjlh.html

PHP:  // 手写递归函数
来源：http://hz.aizwys.cn/gtqoxaqcwg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtuxozgdbf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gtqejplkpc.html

Java: // 手写递归
来源：http://hz.bjfxy.top/gtknqgydcs.html

Go:   // 手写递归
来源：http://hz.yvedp.cn/gthhenrjdp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cheryme.top/gtzhgqirzz.html

C#:   // 手写递归
来源：http://hz.nanxinkj.top/gtihdgowaj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gthlezohxn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cheryme.top/gtfyabljdl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgufenzy.top/gtvzjiwdzp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtfictumbj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yueranfly.top/gtcjpqwvnq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtjmfducxc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhijiandao.cn/gtlhgtdooz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xinyue.icu/gtvxxybuyl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtqhwmuhwy.html

================================================================================
来源：http://hz.zhongyouzk.top/gtllktylej.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gttmtfahbq.html

================================================================================
来源：http://hz.guowangkeji.top/gtmbgyaibf.html

[O01] 启动一个线程
来源：http://hz.ppjwa.cn/gtdkjhtpzp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.andypj.xyz/gtosrkigsn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jyoumei.cn/gtvjgpibfe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aibaodan.cn/gtssnmoplj.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtncbfpznv.html

Java: new Thread(() -> f()).start()
来源：http://hz.gzhubu.top/gtwczczhyc.html

Go:   go f()
来源：http://hz.yvedp.cn/gtkcnshxui.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtkzthkkab.html

C#:   Task.Run(() => F());
来源：http://hz.yonumen.top/gtnlielskq.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gtizgkbeap.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhijiandao.cn/gtikguqudk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigfzy.top/gteeuazcsi.html

JS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gthjcbvgsx.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtrdeewasu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hongshengwenyu.top/gtlbrfowgy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gtrcefdtcu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.kuanghao11.cn/gtkxkrdwqc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258888.top/gtwzzbyinw.html

[O03] 加锁保护共享数据
来源：http://hz.ppjwa.cn/gtmwjfsvxp.html

Py:   with lock: shared += 1
来源：http://hz.fengsongda.top/gteslexawd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtczvcttna.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.dashuyun.cn/gtrswxewzx.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtrjzcznjk.html

Java: synchronized (this) { shared++; }
来源：http://hz.birdmap.top/gtyggbbfva.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yongpay.top/gtxaenudzf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shanyushiyangkeji.top/gtrkhcjtkf.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtlwmworsa.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtipjseqco.html

Py:   async def f():⏎    await g()
来源：http://hz.hnqzz.top/gtvxoyeara.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gthfeevdyk.html

JS:   async function f() { await g(); }
来源：http://hz.zhongyouzk.top/gtgytqpyvt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtffghckec.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtnaybhyqi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.9152youxi.cn/gtcppxzizi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cqqwz.cn/gtwpngbcmu.html

C#:   async Task F() { await G(); }
来源：http://hz.jlsjyb.cn/gtufszxbzr.html

[O05] 并发执行并等待全部完成
来源：http://hz.shzxlz.cn/gtkuwxywyj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.birdmap.top/gtihzuesph.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhengqikj.top/gtzaroymvy.html

JS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gtwjxtlsww.html

TS:   await Promise.all(tasks)
来源：http://hz.tanke756.top/gttoudoedy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jlsjyb.cn/gtqicfngjt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sysykeji.top/gtklhqttkk.html

Ruby: threads.map(&:join)
来源：http://hz.tian-w.cn/gtcpisuluv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daria6918.cn/gtohpiftke.html

[O06] 使用进程池
来源：http://hz.yj202588.top/gtqpnrbrci.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinghuilouyu.cn/gttldokpzx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xingfuxueyuan.xyz/gtzfcijqjd.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtxmimxgxf.html


<!-- 参考信息 -->