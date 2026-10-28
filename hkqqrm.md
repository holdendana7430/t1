代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtodemgarp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aizwys.cn/gtpwdhhgfs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangkeji.top/gtvvmfvhrz.html

[L02] 发送 POST JSON
来源：http://hz.mhx1999.top/gthicfjtrk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xziqi.cn/gtvxdekvgg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtzxezmaxt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtvucachnh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xziqi.cn/gttmxnutos.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hammf.cn/gtjjgyaxtk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtjciusfwi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtxehzuzgk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gtwvfknpwm.html

[L03] 设置自定义请求头
来源：http://hz.havefunace.top/gtdfwlheva.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtvkskwlbp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yonumen.top/gtpqykkctp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtoughqdrs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtbchqxngh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhengqikj.top/gtywpbqxjo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtmtmgnswl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtyhrfpdrj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtqzhqjhzl.html

[L04] 设置超时
来源：http://hz.sysykeji.top/gtpetqpwwm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtzhgzshhq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gtyxgmyeei.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gtuogcmknd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtllvqamqg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtxchthsav.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shangyingyoupin.top/gtobnruvkr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yangfankeji.com/gtsbqpxkrt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shanyushiyangtech.top/gttwjsrgpc.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gtfzqwxuax.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnxiangtu.top/gtocdvrqbw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhengqikj.top/gtbwdjuyie.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtglvisree.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtvvzeirqw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zdqjudy.top/gtynxpxnyp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.feifeiyinyue.top/gtrecywftn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gtgldzafot.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtgbikrgta.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtrhgnkidn.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gtuuogpdvy.html

PHP:  json_decode($body, true);
来源：http://hz.svipenyu.cn/gtkxezpxtw.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtoovqcacb.html

TS:   await resp.json()
来源：http://hz.hywenlv.cn/gtmhynduan.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenjidiqi.icu/gtlwwstqae.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gtqdwtpgqy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gtomnodlzz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gotoacloud.top/gtmwbssbau.html

[L07] 处理 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtbadkuwwp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jyoumei.cn/gtfhezikzp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jiagoushi.top/gtimuxwknt.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtpuliqmur.html

TS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtuazdnyec.html

Java: resp.statusCode()
来源：http://hz.xylfe.cn/gttomcinte.html

Go:   resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtocjorlxo.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gtlbhsnnnm.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtinptedbz.html

[L08] 并发请求多个地址
来源：http://hz.guannengcc.top/gtbwejxaae.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj202588.top/gtkgirxsmu.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtiirzklgw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtwqwgfjts.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtpfrkwnyp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xinyue.icu/gthzxhqxhy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pengpengdd.cyou/gtzhnugyhl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hongshengwenyu.top/gtklpeqjtt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jyoumei.cn/gttdknixin.html

================================================================================
来源：http://hz.yongpay.top/gtsjcqxdin.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinghuilouyu.cn/gtbzzwhnoh.html

================================================================================
来源：http://hz.ivvv.top/gtscjakepm.html

[M01] 读取命令行参数
来源：http://hz.yongpay.top/gtczgtnkli.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtvatnnpgw.html

PHP:  $argv;  $argc;
来源：http://hz.sysykeji.top/gtfqvyneft.html

JS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gttjrokdon.html

TS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtprajikcr.html

Java: args 数组（main 方法参数）
来源：http://hz.ydzc1.top/gtaxzbzcqj.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtjwhgtmys.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gtjzxkftfl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gaohongyu789.top/gtduprgirf.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtokplywwd.html

Py:   os.environ.get("HOME")
来源：http://hz.hnqzz.top/gtwawgeart.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cdnleiting.top/gtnxjzqfpe.html

JS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtrcjpgwib.html

TS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtzrlueaoh.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtuvtaegrz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ivvv.top/gtxhmypojy.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtwywxepke.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtmqbkkood.html

[M03] 执行外部命令
来源：http://hz.jinqigufen.top/gtpqtdrgnk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtdktshtdm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.bjfxy.top/gtfzbfzojh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtlfowkmbr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtaikdrsyn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gzhubu.top/gtopypotrd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtlzjardtl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.snrcjt.cn/gtssblyjom.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhengqikj.top/gtfodvybba.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtqteiotfy.html

Py:   os.getcwd()
来源：http://hz.cheryme.top/gtcpjdxadu.html

PHP:  getcwd();
来源：http://hz.ywan-chungtsiang.top/gtnvebmfme.html

JS:   process.cwd()
来源：http://hz.aibaodan.cn/gtofesjoan.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtzsuuxezk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnxiangtu.top/gtvffjeswo.html

Go:   os.Getwd()
来源：http://hz.svipenyu.cn/gtwwkykupm.html

Ruby: Dir.pwd
来源：http://hz.daria6918.cn/gtquwuaoey.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtzwofrljy.html

[M05] 设置退出码
来源：http://hz.yj20258888.top/gtjyhnjivd.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtolltokij.html

PHP:  exit(1);
来源：http://hz.hysaishi.cn/gtsokioqgz.html

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gtclhhgdvr.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gtjzhusxba.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtlrlquzej.html

Go:   os.Exit(1)
来源：http://hz.jiagoushi.top/gtxuglyzvu.html

Ruby: exit 1
来源：http://hz.jinqigfzy.top/gtqgyndalr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yangfankeji.com/gtuqqscasl.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtpuiusgwh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtewmgonnw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgufenzy.top/gtdqxvvrbn.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtlvtpcdun.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gthpftltzh.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtolofaomm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtmatiexnr.html

Ruby: warn "err"
来源：http://hz.gotoacloud.top/gtwfvvvuot.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ehwqpu.com/gtftzbbuzj.html

[M07] 判断是否为主入口
来源：http://hz.ywan-chungtsiang.top/gtxxttknqh.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigfzy.top/gtgbtnwcib.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xziqi.cn/gtjwyfgxda.html

JS:   require.main === module
来源：http://hz.ydzc1.top/gtklybavtf.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtchaxpxnc.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtfcuipzuh.html

Go:   func main()
来源：http://hz.cucudq.cn/gtzsrfvtse.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.vqdsnc.cn/gtgxbsfueo.html

C#:   static void Main(string[] args)
来源：http://hz.zdqjudy.top/gtzmlotrqd.html

[M08] 获取系统与运行时信息
来源：http://hz.jyoumei.cn/gtkyvlwipv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtphakhlah.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.birdmap.top/gtbkxblydb.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtrpqjpidx.html

TS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtdvnwicui.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangkeji.top/gtmdnomiye.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenjidiqi.icu/gtxxtckfuo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cdnleiting.top/gtukvbilji.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.iojbl.cn/gtwzdbbtag.html

================================================================================
来源：http://hz.yj202588.top/gtjudlxvoe.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gttqnhdqra.html

================================================================================
来源：http://hz.iojbl.cn/gtlxgmgedm.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtntmzwola.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daria6918.cn/gtxiyrynff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xinyue.icu/gtiqaxpuga.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtkivgnvfd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtinckppsf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtfkzfyjtv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ybcxt.top/gthgnpynhc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pengpengdd.cyou/gtisrfquet.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtzwedifpl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhongyouzk.top/gtzyavrfwh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtynqzqzkl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zdqjudy.top/gtlnycfwnn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtkdkqictr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtgzbyqrvh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtxdzdelaq.html

Go:   slices.Sort(arr)
来源：http://hz.ivvv.top/gtxsvahkve.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtouzqgtaa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aibaodan.cn/gtfmmolgqa.html

[N03] 快速排序（分治示例）
来源：http://hz.tanke756.top/gtpaymgqpw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ehwqpu.com/gtnxcbueee.html

PHP:  // 递归实现，或用 usort
来源：http://hz.316326.xyz/gtixygejxw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtbeutidrw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtrnbmxpwa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hfpthk.cn/gtmeebdnnf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtdcxzymdj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhoulong.xyz/gtyqcisydf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtwlhhhswh.html

[N04] 斐波那契数列
来源：http://hz.zhengqikj.top/gtkjquekrc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtkrsfmysc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtqojixwua.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtaanokgyl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtzsbolruv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gtwhzoazbz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xylfe.cn/gtfbxsmegf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtfkgixjhh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtjaxpddso.html

[N05] 最大公约数
来源：http://hz.haohaochexian.top/gtotalmeyf.html

Py:   math.gcd(a, b)
来源：http://hz.ehwqpu.com/gtinsorxpo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hysaishi.cn/gtzyopymcv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtvkrbjjwj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtsmfmiaxh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gthhnudgac.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgfzy.top/gtxetbmgmi.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtfhypourc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ybcxt.top/gtmlbhhbbs.html

[N06] 判断回文字符串
来源：http://hz.yanxiufei.cn/gthaeleaha.html

Py:   s == s[::-1]
来源：http://hz.hysaishi.cn/gtnkhpvrhr.html

PHP:  $s === strrev($s);
来源：http://hz.bjfxy.top/gtcbyymxbn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtockbycbk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtxxuhmprf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tian-w.cn/gtfmdepcts.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gttpyjmlad.html

Ruby: s == s.reverse
来源：http://hz.316326.xyz/gtzymxndrc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.quarkkingdee.top/gtiecrswts.html

[N07] 两数之和（返回下标）
来源：http://hz.zhengqikj.top/gteufirmgf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gaohongyu789.top/gtxkvcoswn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gtbaytooar.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xingfuxueyuan.xyz/gtcsvialfd.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtwpjsvsto.html

Java: // 手写 HashMap
来源：http://hz.chenzaomai.com/gtjtsubltd.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gtapcayyxm.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtjtkjfjmq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtjdvoqbnu.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gtbrtmlhpt.html

Py:   itertools.permutations(arr)
来源：http://hz.52xcode.cn/gtinvhpqzo.html

PHP:  // 手写递归交换
来源：http://hz.ivvv.top/gtpgiuhblg.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtuhtcczeq.html

TS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtswhoaups.html

Java: // 手写回溯递归
来源：http://hz.snrcjt.cn/gtjbhaceba.html

Go:   // 手写回溯递归
来源：http://hz.ivvv.top/gtxsrucnjm.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtyojqfhkx.html

C#:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtbcolhmtp.html

[N09] 栈与队列
来源：http://hz.xuanzx.com/gtbakodqoi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtkmlvijpd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gzhubu.top/gtqmgkkuhk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjfxy.top/gthqzmuwhi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fzhhl.top/gtlldfnebm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gtfcrhnbys.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hysaishi.cn/gtrtyxyzwu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj202588.top/gtdlfyqsvo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydjk.org.cn/gtchlosohv.html

[N10] 链表节点定义
来源：http://hz.shzxlz.cn/gtjvsplknn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxuanxn.top/gttrfedcml.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.pycfn.com/gtlitgkeqv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hongshengwenyu.top/gttzwelwhp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ehwqpu.com/gtfdumlkkh.html

Java: class Node { int v; Node next; }
来源：http://hz.cqqwz.cn/gtbqrwevep.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.snrcjt.cn/gtzipxdnep.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.iojbl.cn/gtatinnift.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenlongwang.top/gtmogivsdj.html

[N11] 二叉树中序遍历
来源：http://hz.yangfankeji.com/gtsntgnskm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.smart0.xyz/gtpgwuubxa.html

PHP:  // 手写递归函数
来源：http://hz.gaohongyu789.top/gtjonwurur.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtgcnthmzy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtummnbrtk.html

Java: // 手写递归
来源：http://hz.sufxvd.cn/gtddscnsjy.html

Go:   // 手写递归
来源：http://hz.yvedp.cn/gtaflftizz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtlmpalhtr.html

C#:   // 手写递归
来源：http://hz.hysaishi.cn/gtsnzmecke.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenlongwang.top/gtqmgdvdmy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fzhhl.top/gtqhsdysct.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shangyingyoupin.top/gtbdlppgdx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daria6918.cn/gttpkacsyc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gtqzvwxexn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtnrmxqwmp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ehwqpu.com/gtpxfroyqe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tian-w.cn/gthpbaafnk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxuanxn.top/gtyhisplbe.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgynsshxu.html

O. 并发与异步
来源：http://hz.vqdsnc.cn/gtgpwcacem.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtppdcxzsl.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtvujnyodn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258888.top/gtldyluudf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtshaapbyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gthwvpfjpn.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtogrjdmex.html

Java: new Thread(() -> f()).start()
来源：http://hz.ywan-chungtsiang.top/gtmmipwpld.html

Go:   go f()
来源：http://hz.smart0.xyz/gtxssruwnj.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gtczvknvwb.html

C#:   Task.Run(() => F());
来源：http://hz.sxryk.cn/gthjjqfoiw.html

[O02] 使用线程池
来源：http://hz.kuanghao11.cn/gtacpucmei.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cdnleiting.top/gtwcjcoynt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pengpengdd.cyou/gtsrrgjhwv.html

JS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtbraudxuh.html

TS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtcdaylyau.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shuidangran.top/gtcqurygnd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtushzvimm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258.top/gtxtefrcga.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fengsongda.top/gtoqpdcwix.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtxjzqkzzw.html

Py:   with lock: shared += 1
来源：http://hz.smart0.xyz/gticebcefx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xziqi.cn/gtzmuqyddy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ywan-chungtsiang.top/gteptofved.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtskgesubw.html

Java: synchronized (this) { shared++; }
来源：http://hz.daxiang520.top/gtvmhixmms.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.bjfxy.top/gthupibzzn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sxryk.cn/gtyrqlpgdb.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtwkoeaiwd.html

[O04] 定义异步函数并等待
来源：http://hz.guannengcc.top/gtxzcvvzws.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtaaijvgoj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gotoacloud.top/gtkpuuolfu.html

JS:   async function f() { await g(); }
来源：http://hz.yonumen.top/gtemuhfbzi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aibaodan.cn/gtzsdwwydb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.svipenyu.cn/gtvaneekja.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtnpxddbjj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.c1oappe.top/gttlkeugpg.html

C#:   async Task F() { await G(); }
来源：http://hz.zhijiandao.cn/gtbujqldfy.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gtzfelbrib.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtpwhwiixx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.iojbl.cn/gtwyyygvoz.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtdhwuojjh.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtoypgptqv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangtech.top/gtlkrofava.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pengpengdd.cyou/gtrusvhlob.html

Ruby: threads.map(&:join)
来源：http://hz.jlsjyb.cn/gtpmrridzg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xingfuxueyuan.xyz/gtvbrekddi.html


<!-- 参考信息 -->