代发 wailian999

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtarcghifa.html

Ruby: Marshal.dump(obj)
来源：http://hz.cucudq.cn/gtnxfifdqd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.snrcjt.cn/gtzoypodrq.html

================================================================================
来源：http://hz.ivvv.top/gttcjqtmmd.html

L. 网络请求
来源：http://hz.xinyue.icu/gttukryfjh.html

================================================================================
来源：http://hz.xinyue.icu/gtkogvbufy.html

[L01] 发送 GET 请求
来源：http://hz.wangdashe.top/gtckwemzmt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fengsongda.top/gtdrsceovq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtdzfyemnl.html

JS:   await fetch(url)
来源：http://hz.nwbrower.top/gtvsznbnlu.html

TS:   await fetch(url)
来源：http://hz.zdqjudy.top/gtkgqhyzjv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtrtumclgi.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinghuilouyu.cn/gtnafuqyhd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gtcddiejbe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hongshengwenyu.top/gtvvvqzltc.html

[L02] 发送 POST JSON
来源：http://hz.yuanzhike.top/gtggfousjb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtsknhxdmb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhongyouzk.top/gtwofusfmh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtxfhszeds.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gttpwlwhds.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtgtfqbtij.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cucudq.cn/gtfyectkvv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yanxiufei.cn/gtmdgegkmd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuxming.cn/gtdlbqrgda.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtiumdkddl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtqoivlbzj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gtmkfkajrd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtmlvrtocb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtpfahuhvz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtnozoglzp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258.top/gtmssgfcfl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigufen.top/gtovipdtkg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtjvtqwavo.html

[L04] 设置超时
来源：http://hz.tanke756.top/gtrzezsvoa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxinkj.top/gtoblectvv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.feifeiyinyue.top/gtjinjrvjq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtajbavlui.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtiunphdml.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigfzy.top/gtdznnrsbf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tianlin.xyz/gtkmnkukrv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hywenlv.cn/gtftdtmfbe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fzhhl.top/gtujytecng.html

[L05] 上传文件（multipart）
来源：http://hz.yuxming.cn/gtpxxihsmp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtmznktwbo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtckkttbcs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.52xcode.cn/gtfhcoqlou.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtgusragfh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gteqdperor.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.feifeiyinyue.top/gtexapxpwy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtsvbeanlo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinyuanbaomall.cn/gtzoclqgzp.html

[L06] 解析响应为 JSON
来源：http://hz.chenjidiqi.icu/gttbthmurs.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtywqjpidt.html

PHP:  json_decode($body, true);
来源：http://hz.ppjwa.cn/gtwiyrsxnk.html

JS:   await resp.json()
来源：http://hz.ybcxt.top/gtcewpvpgf.html

TS:   await resp.json()
来源：http://hz.hywenlv.cn/gtryqqkqgx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenzaomai.com/gtddncktvx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.quarkkingdee.top/gtlmhejbdt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jianghu66.top/gtkngqbmsr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtqucqujpk.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtudjxiydz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtzozrqjmw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guannengcc.top/gteovhrvie.html

JS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtanyundpw.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtjcxqrjjq.html

Java: resp.statusCode()
来源：http://hz.zhengqikj.top/gttulvglvf.html

Go:   resp.StatusCode
来源：http://hz.pycfn.com/gtceihokqm.html

Ruby: resp.code.to_i
来源：http://hz.cqqwz.cn/gthwisywpw.html

C#:   (int)resp.StatusCode
来源：http://hz.c1oappe.top/gtrnwkubgf.html

[L08] 并发请求多个地址
来源：http://hz.hfpthk.cn/gtmfvuruqr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258888.top/gtcpcbgvqw.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtopfkwchz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtcediijcd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtaugdfbzs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtglswhofg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aizwys.cn/gttrzlbgcg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtyuffnscg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtbvqoqnjz.html

================================================================================
来源：http://hz.svipenyu.cn/gtayfaafad.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtdlbqndzk.html

================================================================================
来源：http://hz.smart0.xyz/gtbiphdhpw.html

[M01] 读取命令行参数
来源：http://hz.yongpay.top/gtlcnhlnhx.html

Py:   sys.argv[1:]
来源：http://hz.52xcode.cn/gtiluubzxy.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtyhgafecx.html

JS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gttlbrjjsd.html

TS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtobdovpgv.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gttkanwarq.html

Go:   os.Args[1:]
来源：http://hz.9152youxi.cn/gtmltburvx.html

Ruby: ARGV
来源：http://hz.shangyingyoupin.top/gtpzhokhcx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sweek.top/gtpsssqrjz.html

[M02] 读取环境变量
来源：http://hz.hnqzz.top/gtdhfggtms.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtocsshdwk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtoiazuubg.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gthkliabyl.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtrklwipys.html

Java: System.getenv("HOME")
来源：http://hz.feifeiyinyue.top/gtumefghes.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtwfowwckh.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtzoisajjn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtkjlacxgq.html

[M03] 执行外部命令
来源：http://hz.birdmap.top/gtmhprsjbj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhongyouzk.top/gtocnpyaai.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sysykeji.top/gtmrervqcv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtdjfmqwon.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtxbgegquk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtveauiijn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gtsviynrhl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yonumen.top/gttrysytip.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ivvv.top/gtyfzkbtmb.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtzxlniuku.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangkeji.top/gtzqcrypkj.html

PHP:  getcwd();
来源：http://hz.xuanzx.com/gtvocbckgc.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtyjyhpyzm.html

TS:   process.cwd()
来源：http://hz.nanxuanxn.top/gtiqlsqymy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtohreicvy.html

Go:   os.Getwd()
来源：http://hz.yj202588.top/gtopdfgnxw.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtnlmesddt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtcsgvecmi.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtbbdmhhtq.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gttjxsdgzn.html

PHP:  exit(1);
来源：http://hz.daxiang520.top/gtnkzkhlxa.html

JS:   process.exit(1)
来源：http://hz.tanke756.top/gtqgrpqqpw.html

TS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtlxksxexq.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gtnmtzhrzy.html

Go:   os.Exit(1)
来源：http://hz.jiagoushi.top/gtoqeakaut.html

Ruby: exit 1
来源：http://hz.xinyue.icu/gtiknkyalf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ivvv.top/gtbmypwlcg.html

[M06] 向标准错误输出
来源：http://hz.shzxlz.cn/gtpbbdbatw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.52xcode.cn/gtmybtqimf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigfzy.top/gtfyifsszk.html

JS:   console.error("err")
来源：http://hz.hywenlv.cn/gtmksnciah.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtifilhpjm.html

Java: System.err.println("err")
来源：http://hz.hammf.cn/gtmgwceujo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yanxiufei.cn/gtdezncrsd.html

Ruby: warn "err"
来源：http://hz.yuxming.cn/gtvpktastg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ehwqpu.com/gtbtdbngji.html

[M07] 判断是否为主入口
来源：http://hz.yongpay.top/gtalusyfrb.html

Py:   if __name__ == "__main__":
来源：http://hz.tian-w.cn/gthsaikgpz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtoyrjfwuf.html

JS:   require.main === module
来源：http://hz.jianghu66.top/gtmqkllqlr.html

TS:   require.main === module
来源：http://hz.zdqjudy.top/gtqkjzssty.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtobujowch.html

Go:   func main()
来源：http://hz.cheryme.top/gtzjipiaqg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtwgnqswmi.html

C#:   static void Main(string[] args)
来源：http://hz.jlsjyb.cn/gtudiomaxz.html

[M08] 获取系统与运行时信息
来源：http://hz.hfpthk.cn/gtbhpspzia.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtvrgfcuej.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtpkdgkpov.html

JS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtzrcgbxlu.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtxspcdoru.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtglsokjug.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sufxvd.cn/gtvhqrfxqd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.andypj.xyz/gtgdgzrweb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jqgufenzy.top/gtudxoepus.html

================================================================================
来源：http://hz.zycfv.cn/gtzjfbtqjs.html

N. 数据结构与算法
来源：http://hz.zdqjudy.top/gtflgbnsct.html

================================================================================
来源：http://hz.yj20258.top/gtwmfpntfx.html

[N01] 二分查找（有序数组）
来源：http://hz.tanke756.top/gtinqjmezj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guannengcc.top/gtebmbslmr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cheryme.top/gtavpcaolp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gtapqjpqoc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtkapclpdz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtjmpekfgb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shzxlz.cn/gttqximggw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zycfv.cn/gtnkgionvj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtvhrzvauq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dianchejie.cn/gtqrgbjeel.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtzpmxcgzo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.haohaochexian.top/gtgpztztni.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtuiscopyv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtmpgslvjc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gtsrcxztmc.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtubfozgke.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtowcaucju.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj202588.top/gtaobovnfd.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtembzejss.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.dashuyun.cn/gthfinkjtg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtoeemxmnj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtkevwoecz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtvmlpydxv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtprsxpkzv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnqzz.top/gtlsjiabmd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtivlrluqv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.havefunace.top/gtpbpvjdhf.html

[N04] 斐波那契数列
来源：http://hz.mhx1999.top/gtfzjvclbn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtodwkitnj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yangfankeji.com/gtdxwlxjgh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.andypj.xyz/gthjuzqnna.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtnmvxtfvd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangtech.top/gtjzylvpqm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangkeji.top/gttusbmzgl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtgodfxtfd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtxzsjzohb.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gtytbqnwuv.html

Py:   math.gcd(a, b)
来源：http://hz.jyoumei.cn/gthbgbnbko.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daria6918.cn/gtliksrwxb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtmmhixrqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtdsycipwj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuetiantiany.cn/gtrhyomhky.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yvedp.cn/gthboqprkz.html

Ruby: a.gcd(b)
来源：http://hz.jinyuanbaomall.cn/gtermlttfk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shangyingyoupin.top/gtoavyzyla.html

[N06] 判断回文字符串
来源：http://hz.gotoacloud.top/gtslfohtrq.html

Py:   s == s[::-1]
来源：http://hz.nanxinkj.top/gtddzlyqwa.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258.top/gtmdtystwv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtxktzdrok.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtydkcfsji.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gthdudykva.html

Go:   // 双指针从两端比较
来源：http://hz.snrcjt.cn/gtnvdhcnxq.html

Ruby: s == s.reverse
来源：http://hz.jinghuilouyu.cn/gtilookkwi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtufscshie.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gtuljctngo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.andypj.xyz/gtdzkcmsqv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cheryme.top/gtpqodrnlc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtevatshtu.html

TS:   // 手写 Map<string, number>
来源：http://hz.xingfuxueyuan.xyz/gtfcmwetkc.html

Java: // 手写 HashMap
来源：http://hz.chenzaomai.com/gtlgmhkqab.html

Go:   // 手写 map[int]int
来源：http://hz.zhengqikj.top/gticseeezb.html

Ruby: // 手写 Hash
来源：http://hz.jiagoushi.top/gtmdhsvaiu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tianlin.xyz/gttxoqopxc.html

[N08] 生成全排列
来源：http://hz.hongshengwenyu.top/gtjqonjzcc.html

Py:   itertools.permutations(arr)
来源：http://hz.tianlin.xyz/gtuelrwdqh.html

PHP:  // 手写递归交换
来源：http://hz.yangfankeji.com/gtitoptvhm.html

JS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtlgepdvfx.html

TS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtellmlpca.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtannrkles.html

Go:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtkuoyigtm.html

Ruby: arr.permutation.to_a
来源：http://hz.ydzc1.top/gtsztlgcjg.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gtvfvrbapw.html

[N09] 栈与队列
来源：http://hz.sweek.top/gtocydiuzy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtgzgawszs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hongshengwenyu.top/gtvxljmsgn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gttugyinfb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtxhucqyjv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtoiyixlpw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hywenlv.cn/gtlqcvfoyg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ydzc1.top/gtzrivnfru.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuanzhike.top/gtzxfzqixi.html

[N10] 链表节点定义
来源：http://hz.wangshuangyany.cn/gtjdrrehie.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nwbrower.top/gtajvmvnxr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jiagoushi.top/gtqvppleij.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.0kj1m.cn/gtvndosjoj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtfalafwxu.html

Java: class Node { int v; Node next; }
来源：http://hz.ehwqpu.com/gtbofaovls.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nwbrower.top/gtkiozupkx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.quarkkingdee.top/gttycezwek.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hywenlv.cn/gtzeyedzng.html

[N11] 二叉树中序遍历
来源：http://hz.andypj.xyz/gtkrwmwkew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gtkjfbhjma.html

PHP:  // 手写递归函数
来源：http://hz.0kj1m.cn/gtnzqvmncb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtubmsmjhs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gthjaacvwd.html

Java: // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtfkyyukpy.html

Go:   // 手写递归
来源：http://hz.gogol.net.cn/gtmfztksmo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xylfe.cn/gtnbfddjuy.html

C#:   // 手写递归
来源：http://hz.aizwys.cn/gtuedtimhs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hongshengwenyu.top/gtquutkaky.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ehwqpu.com/gtxijtiwsd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258.top/gttgzffmjf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gttduufodu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gttukkfkdk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gttzvbrutq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gaohongyu789.top/gtyjeaahwp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhoulong.xyz/gtbrlcuciu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtyspyxpme.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtaxgdqkyv.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtuetzgmdx.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjgdmnjnc.html

[O01] 启动一个线程
来源：http://hz.9152youxi.cn/gtedbfyuei.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gthxioorwb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258.top/gtvqtqagsy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xylfe.cn/gtcwiaopfp.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gteqagktnb.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gtabhsjofz.html

Go:   go f()
来源：http://hz.yueranfly.top/gtczfexkkh.html

Ruby: Thread.new { f }
来源：http://hz.ydjk.org.cn/gtjlxzlyyk.html

C#:   Task.Run(() => F());
来源：http://hz.iojbl.cn/gtrczfudef.html

[O02] 使用线程池
来源：http://hz.ywan-chungtsiang.top/gtshqjxeqx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258888.top/gtmbekkfzn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinqigufen.top/gtwyjnuked.html

JS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtgxyxfjlm.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtxemvnfft.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guannengcc.top/gtennduire.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhiwuduotai.top/gtkntnznqx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yanxiufei.cn/gtnikxuert.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtvxrwmban.html

[O03] 加锁保护共享数据
来源：http://hz.smart0.xyz/gtixoblanu.html

Py:   with lock: shared += 1
来源：http://hz.9152youxi.cn/gtyrwfkddy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jyoumei.cn/gtwbzjwlot.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sysykeji.top/gtaxalrmfv.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtglbosukb.html

Java: synchronized (this) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtzblbyojf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.snrcjt.cn/gtivomiuin.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgfzy.top/gtlfmjzxjf.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gtytjngxbu.html

[O04] 定义异步函数并等待
来源：http://hz.yuanzhike.top/gtwlevapml.html

Py:   async def f():⏎    await g()
来源：http://hz.hnqzz.top/gtulelifwp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtoksaugsy.html

JS:   async function f() { await g(); }
来源：http://hz.wangdashe.top/gtaadmekid.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gttskqwaon.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.mhx1999.top/gtnlqeuzuw.html


<!-- 参考信息 -->