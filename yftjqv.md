代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtkvjhnvfx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.0kj1m.cn/gtspdsurva.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtkuychwlm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtmztgavwr.html

[L03] 设置自定义请求头
来源：http://hz.quarkkingdee.top/gtlrlesuaj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.snrcjt.cn/gtkopignqh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258888.top/gteqqwgmol.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtzbtdrptv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gttrmnzkxn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.svipenyu.cn/gtwudwgour.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtadkiyqib.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jlsjyb.cn/gtzvgxbfcp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtluqldphq.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtuyvtbnug.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gtaibhmlqe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cucudq.cn/gtykpxwzvc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtfxlmazsm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gthytipxms.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gtcqqljsjt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtfjabmful.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenlongwang.top/gtyuyfbtpa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtwzojnnse.html

[L05] 上传文件（multipart）
来源：http://hz.cheryme.top/gtyerubtui.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtinrhaexi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jlsjyb.cn/gtfgmnvseq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtppyoemnr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtbunxhtif.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gzhubu.top/gtwzbolnnc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtghdvengw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daxiang520.top/gtvepravmx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jlsjyb.cn/gtrceecpuh.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtyauktewl.html

Py:   resp.json()
来源：http://hz.cucudq.cn/gtnnbxrqxz.html

PHP:  json_decode($body, true);
来源：http://hz.gzhubu.top/gtwdgkhouc.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtoblhzcgh.html

TS:   await resp.json()
来源：http://hz.0kj1m.cn/gtqdzwmdmt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnxiangtu.top/gtkemzrqej.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hammf.cn/gtccdvrdfq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gthnczhlfp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtghpyyvyw.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtqkqurlkk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtbhjzuqcp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtqcfeejlm.html

JS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gteucwhlqu.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gthbgtgpbs.html

Java: resp.statusCode()
来源：http://hz.tian-w.cn/gtbfeltspa.html

Go:   resp.StatusCode
来源：http://hz.jianghu66.top/gtmxjcjesk.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtdcrnvfda.html

C#:   (int)resp.StatusCode
来源：http://hz.nwbrower.top/gtkttvexux.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangtech.top/gtqsaubyrh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gogol.net.cn/gtvmqccwqj.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtwzagxkzu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtwfwiqado.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtojfxowpq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.kuanghao11.cn/gtbkavdsqr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jyoumei.cn/gtebcmazab.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtxymdhkki.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtuklqyjvj.html

================================================================================
来源：http://hz.yongpay.top/gtlbczrtor.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnqzz.top/gtinmbrrzk.html

================================================================================
来源：http://hz.ivvv.top/gtpcpqvxyn.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gttqkpzdeu.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtzmzsvxua.html

PHP:  $argv;  $argc;
来源：http://hz.feifeiyinyue.top/gtobhnztvj.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtxcmtfcla.html

TS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtlpcdnqld.html

Java: args 数组（main 方法参数）
来源：http://hz.aizwys.cn/gtipzludmf.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangkeji.top/gtmltrwtev.html

Ruby: ARGV
来源：http://hz.pengpengdd.cyou/gtbnnpqgsp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gtzspzotmt.html

[M02] 读取环境变量
来源：http://hz.ydjk.org.cn/gtsefrikss.html

Py:   os.environ.get("HOME")
来源：http://hz.yj202588.top/gtpkyjsqoo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gtkpintxue.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtjnzfvfum.html

TS:   process.env.HOME
来源：http://hz.andypj.xyz/gtvxqprkxv.html

Java: System.getenv("HOME")
来源：http://hz.hongshengwenyu.top/gtgyiecdpu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtuhzlhlgr.html

Ruby: ENV["HOME"]
来源：http://hz.quarkkingdee.top/gtsnexuwqh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtetjcjnpi.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtzotwwzvs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangkeji.top/gtdzicuwrw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.mhx1999.top/gtiysbvrpj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtjomsrsgy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtnztifetm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxinkj.top/gtsjmhhxtw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtkdxxlgyz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yonumen.top/gtyzvdbkea.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtpndwtxoo.html

[M04] 获取当前工作目录
来源：http://hz.haohaochexian.top/gthovuyjck.html

Py:   os.getcwd()
来源：http://hz.zhijiandao.cn/gtwkfgchxv.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtfjbtebjt.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtkqrnoruk.html

TS:   process.cwd()
来源：http://hz.tanke756.top/gttuqsefcb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgufenzy.top/gtqizlyike.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gtsnqeypbr.html

Ruby: Dir.pwd
来源：http://hz.guowangkeji.top/gthwiisadq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gtwccuaunv.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtmzbnyjqx.html

Py:   sys.exit(1)
来源：http://hz.xuanzx.com/gtmrwubmet.html

PHP:  exit(1);
来源：http://hz.feifeiyinyue.top/gtskdjdkrw.html

JS:   process.exit(1)
来源：http://hz.bjfxy.top/gtqywyrktt.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtxksyvvfw.html

Java: System.exit(1)
来源：http://hz.dashuyun.cn/gtmzihoagb.html

Go:   os.Exit(1)
来源：http://hz.dashuyun.cn/gtjhixeyem.html

Ruby: exit 1
来源：http://hz.sxryk.cn/gtnkexokao.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtfalonyuh.html

[M06] 向标准错误输出
来源：http://hz.sxryk.cn/gtpevyxfvz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtxnmrwttf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtlrvvdmpo.html

JS:   console.error("err")
来源：http://hz.meibo888.top/gtfoaduvsi.html

TS:   console.error("err")
来源：http://hz.sweek.top/gtyiuzrdwf.html

Java: System.err.println("err")
来源：http://hz.hammf.cn/gtnyginvri.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cashguo.top/gtrsmmvhab.html

Ruby: warn "err"
来源：http://hz.feifeiyinyue.top/gtciqzpctb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jyoumei.cn/gtgcgchekm.html

[M07] 判断是否为主入口
来源：http://hz.ydzc1.top/gtfburztxx.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gtkdqijsuz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtcumfqbrp.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtterrgwco.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtiigxueww.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtmhgdvnmg.html

Go:   func main()
来源：http://hz.haohaochexian.top/gtvxnpjmob.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cucudq.cn/gtsfnoffjv.html

C#:   static void Main(string[] args)
来源：http://hz.ywan-chungtsiang.top/gtgnalicex.html

[M08] 获取系统与运行时信息
来源：http://hz.shzxlz.cn/gtceurzuuu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daxiang520.top/gtdygcriqc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.kuanghao11.cn/gtrphbxdfl.html

JS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtqobptvtf.html

TS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gttggzbgyl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangtech.top/gtwueibdte.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtnkvxhtab.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtcunpzlfl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtjleulqhn.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttzhufwne.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtojhcfyxc.html

================================================================================
来源：http://hz.gaohongyu789.top/gthleoexjp.html

[N01] 二分查找（有序数组）
来源：http://hz.yuanzhike.top/gtoqpnrfhf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.bjfxy.top/gthjjvidpj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cucudq.cn/gtdhkviczl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtalnfetye.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtwpaarhwc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtzszvokmw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xuanzx.com/gtiaizxcyr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtriwqckfo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtatvelqbv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydzc1.top/gtqsfagekf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtpahyzqtv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgfzy.top/gtcovcphof.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtgdlwdmmv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtrpgvplrn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenjidiqi.icu/gtqxycpeyt.html

Go:   slices.Sort(arr)
来源：http://hz.andypj.xyz/gthxlrypda.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtkklfijoo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.52xcode.cn/gtnlkwpfzv.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtnvpyeisr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigfzy.top/gttbkwqmht.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtjuwkkvgr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtpfoxhixt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtpcvswfqy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.9152youxi.cn/gtjmprxnpb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtttgdleok.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gtazyevycg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.52xcode.cn/gttipfdynf.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtpohyccoc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtwglhaiur.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.haohaochexian.top/gtdbqvjaaf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtyontikyj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtrzwmdlgl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuanzhike.top/gteslseiyh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.meibo888.top/gtrtfcwcsv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtbwjtmjpy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtsjaxkzzr.html

[N05] 最大公约数
来源：http://hz.yonumen.top/gtxpdkycng.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gthivlmrdw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtefiardys.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtvlqaqaqe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtzuanwkwb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.snrcjt.cn/gtmrahvimp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtdxtdskdp.html

Ruby: a.gcd(b)
来源：http://hz.hongshengwenyu.top/gtzhsfnjxf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jiagoushi.top/gtdenzvczd.html

[N06] 判断回文字符串
来源：http://hz.jinqigfzy.top/gtvzsmyrix.html

Py:   s == s[::-1]
来源：http://hz.zhiwuduotai.top/gtjclagiqp.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtrxwcheni.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtiuoypxdw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtexckchyc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jianghu66.top/gtgjnixgrx.html

Go:   // 双指针从两端比较
来源：http://hz.yangfankeji.com/gtrojibnqg.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtptlxyggh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtywoxklbf.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtsevvcsvv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gthcfmjmop.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydzc1.top/gtmblxklvp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtpxaivouv.html

TS:   // 手写 Map<string, number>
来源：http://hz.quarkkingdee.top/gtwqrerjyx.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtjxnmpafs.html

Go:   // 手写 map[int]int
来源：http://hz.nanxuanxn.top/gtngfylzge.html

Ruby: // 手写 Hash
来源：http://hz.tanke756.top/gtulsxwhmh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gtnsdoqsma.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtxvqnxhma.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtegynitws.html

PHP:  // 手写递归交换
来源：http://hz.zdqjudy.top/gtoucnedzx.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtsofxnqfx.html

TS:   // 手写回溯递归
来源：http://hz.meibo888.top/gthffibknh.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gtsarvxmnl.html

Go:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtikquunpv.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtwdstoyzv.html

C#:   // 手写回溯递归
来源：http://hz.hammf.cn/gtlablznkm.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gtjtfnzixe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtzsjgzwjh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtedijwyut.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gtumiqbrpk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhoulong.xyz/gtrxmwuniw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sweek.top/gtahlxhmbz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yanxiufei.cn/gtmbhipbny.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yongpay.top/gtpmibgohg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tanke756.top/gtaoupwjgu.html

[N10] 链表节点定义
来源：http://hz.cdnleiting.top/gtgkqvstpf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtvqtbmnkz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgufenzy.top/gtjnwvyaig.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hysaishi.cn/gtgkpqvuhp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnqzz.top/gtdaumuevf.html

Java: class Node { int v; Node next; }
来源：http://hz.fzhhl.top/gtetlqobmj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.meibo888.top/gtxuaxqqja.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangtech.top/gtieygvatg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtcrdzqaal.html

[N11] 二叉树中序遍历
来源：http://hz.sxryk.cn/gtztckoulc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aizwys.cn/gtvjrbwcnd.html

PHP:  // 手写递归函数
来源：http://hz.yj20258.top/gtpqirtgql.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtzywqsbxe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.iojbl.cn/gtbsiljzru.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtjtmihiye.html

Go:   // 手写递归
来源：http://hz.jiagoushi.top/gthcmkbuef.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.c1oappe.top/gtvriyvusk.html

C#:   // 手写递归
来源：http://hz.tianlin.xyz/gthgclmcwb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinghuilouyu.cn/gtlhzkohnl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.iojbl.cn/gtirvcfjvz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fengsongda.top/gtjftvfesp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtrqnbpnhx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnxiangtu.top/gtgaoufejg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtumpzntkj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtbnzwztoe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gtipsjklzb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtnqjwtweq.html

================================================================================
来源：http://hz.andypj.xyz/gtewnxywil.html

O. 并发与异步
来源：http://hz.c1oappe.top/gtgtzskeql.html

================================================================================
来源：http://hz.wangdashe.top/gtlfhmjijj.html

[O01] 启动一个线程
来源：http://hz.cdnleiting.top/gtqgupyenw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dianchejie.cn/gtrjlyoevi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtdgfrrfuk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhijiandao.cn/gtsvbzjzzw.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtbfzslcsi.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gtdshwxndr.html

Go:   go f()
来源：http://hz.yuanzhike.top/gtqyluzhhr.html

Ruby: Thread.new { f }
来源：http://hz.sxryk.cn/gtkpxbiekv.html

C#:   Task.Run(() => F());
来源：http://hz.yongpay.top/gtvyflrhmd.html

[O02] 使用线程池
来源：http://hz.gogol.net.cn/gtilebpyoj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.9152youxi.cn/gtpgexpcdg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtliutxrhs.html

JS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtmxdbecln.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtmdldbqvq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.c1oappe.top/gtlkxhhapu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtolomsbrt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtlnrwismf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gogol.net.cn/gteaxgpwxv.html

[O03] 加锁保护共享数据
来源：http://hz.aibaodan.cn/gtductjpqh.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gtxdzttxnq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gttwibyfod.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daria6918.cn/gtswbqlunr.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtykbhogmz.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxinkj.top/gtmrhnbttl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jyoumei.cn/gtwhqodhso.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ywan-chungtsiang.top/gtgcgmvhpw.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtuaejydgz.html

[O04] 定义异步函数并等待
来源：http://hz.hysaishi.cn/gtruudpkdi.html

Py:   async def f():⏎    await g()
来源：http://hz.hfpthk.cn/gtfvdxabnx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangshuangyany.cn/gtidxhgmzj.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gttimvwhjj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gaohongyu789.top/gtengroygc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xinyue.icu/gtjiaelywt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.smart0.xyz/gteczgbnuj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guowangkeji.top/gtawkhshwc.html

C#:   async Task F() { await G(); }
来源：http://hz.cheryme.top/gtieafgxcx.html

[O05] 并发执行并等待全部完成
来源：http://hz.jiagoushi.top/gtpwcwrxux.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gaohongyu789.top/gtfhhhtnnm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gthfvmlleh.html

JS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtsihmzivv.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtuvzirdoz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.smart0.xyz/gtygrvfiky.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guannengcc.top/gthsydifwh.html

Ruby: threads.map(&:join)
来源：http://hz.zhiwuduotai.top/gtwtcrlcns.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yvedp.cn/gtajeazhfi.html

[O06] 使用进程池
来源：http://hz.guannengcc.top/gtpjffmwii.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guowangkeji.top/gtfbhypglc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuanzhike.top/gttkiwodui.html

JS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gteunefolg.html

TS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtzobjewwj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dashuyun.cn/gtoiqbcndh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sysykeji.top/gtmgouylaj.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtalcvoyrt.html


<!-- 参考信息 -->