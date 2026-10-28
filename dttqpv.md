代发 wailian999

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtdowwbrhx.html

Ruby: Marshal.dump(obj)
来源：http://hz.xingfuxueyuan.xyz/gtdhzddthh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gttklqflii.html

================================================================================
来源：http://hz.ydzc1.top/gtjdkeopul.html

L. 网络请求
来源：http://hz.guowangkeji.top/gtsakeiaba.html

================================================================================
来源：http://hz.xinyue.icu/gtcdxzodvz.html

[L01] 发送 GET 请求
来源：http://hz.hysaishi.cn/gtodqhnwho.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtrifppfvs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtiqsxcwac.html

JS:   await fetch(url)
来源：http://hz.cashguo.top/gtbuphmtyn.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtyjiybodu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtohryjhlr.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigfzy.top/gtplgmsnfu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shangyingyoupin.top/gtzwjckilz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhijiandao.cn/gtqcgkmriw.html

[L02] 发送 POST JSON
来源：http://hz.birdmap.top/gtmulfmykh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xuetiantiany.cn/gtevnwhndj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gtjtauekzv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtupadmijb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xziqi.cn/gtergnlegv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gtomqiqfed.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yvedp.cn/gtgqmqooey.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.vqdsnc.cn/gtnsbbyptk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jianghu66.top/gtmdoozhpo.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gthcqmwpmy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.vqdsnc.cn/gtsdhjknpu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.iojbl.cn/gtuuwcmvsz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtaoetmnnf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtgdpuaxtj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtsvmkeaes.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtypcdyqtd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtzlgetfif.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtsktddzux.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtmdxecuse.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gotoacloud.top/gtwabjngby.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zdqjudy.top/gtridqcuyl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtzykdulsb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtxydhrtip.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pycfn.com/gtfoabsezu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sysykeji.top/gtzcsyvqlz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtfodcjdoj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dashuyun.cn/gtttsmifiw.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gthkmfiucp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtocahhwcp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtinpoowny.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtidkigati.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtwtmihyxt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhixingplan.top/gtkbupqqoq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pycfn.com/gtqawasplo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtgphtkmhd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.bjfxy.top/gtttdunsko.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtqyvhfsrc.html

Py:   resp.json()
来源：http://hz.birdmap.top/gtsiuqsbev.html

PHP:  json_decode($body, true);
来源：http://hz.daxiang520.top/gtjdhvesqa.html

JS:   await resp.json()
来源：http://hz.ehwqpu.com/gtjjnrqkqn.html

TS:   await resp.json()
来源：http://hz.fzhhl.top/gtgxsqvnav.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hfpthk.cn/gtklhbqjgc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.quarkkingdee.top/gtomxgxmwx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hongshengwenyu.top/gtkfixbymq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuxming.cn/gtghtcmudf.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtrajcyfab.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cucudq.cn/gtlfzufgma.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtnusxbhdh.html

JS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtefcwqbdt.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtgsrecpbi.html

Java: resp.statusCode()
来源：http://hz.xingfuxueyuan.xyz/gtfzjxvjru.html

Go:   resp.StatusCode
来源：http://hz.meibo888.top/gtcgdkaylu.html

Ruby: resp.code.to_i
来源：http://hz.ehwqpu.com/gtqnjsqpyl.html

C#:   (int)resp.StatusCode
来源：http://hz.yongpay.top/gtpwxpuxwr.html

[L08] 并发请求多个地址
来源：http://hz.hammf.cn/gttzaxlpza.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnxiangtu.top/gtaqkyzqqy.html

PHP:  curl_multi_init() 系列
来源：http://hz.meibo888.top/gtqmksctbz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtlcohdbya.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtrgokjnvp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhongyouzk.top/gtcwyqynoa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtseoyoyyw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangkeji.top/gtmvnvceom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtzftmekrr.html

================================================================================
来源：http://hz.yonumen.top/gtfeeyvkyd.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhixingplan.top/gthhwzwrle.html

================================================================================
来源：http://hz.jianghu66.top/gtixzfgwzd.html

[M01] 读取命令行参数
来源：http://hz.yj20258888.top/gtfxtdwjbs.html

Py:   sys.argv[1:]
来源：http://hz.zhongyouzk.top/gtchwbpmbp.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gtkgtthwfc.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtpvwelcal.html

TS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtvqeaeeeb.html

Java: args 数组（main 方法参数）
来源：http://hz.snrcjt.cn/gtoldiseqx.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gtcdiorqvd.html

Ruby: ARGV
来源：http://hz.cashguo.top/gtoofapxvi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnxiangtu.top/gtwqdsgfmg.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gthvgbmiwq.html

Py:   os.environ.get("HOME")
来源：http://hz.zhijiandao.cn/gtsnrtyknw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtvfufqyzu.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtosbqxyfq.html

TS:   process.env.HOME
来源：http://hz.guannengcc.top/gtmutbhelt.html

Java: System.getenv("HOME")
来源：http://hz.kuanghao11.cn/gtgdpymarl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gtaervnhbq.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtkpnpdman.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtcyrmdccd.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtlyxmfkcr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xingfuxueyuan.xyz/gtuwzrhtej.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.meibo888.top/gtebulhqtz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtribinyyr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.birdmap.top/gthdkwnova.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zdqjudy.top/gtumsqohid.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gtyblsnqzi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydzc1.top/gtcatfyhhj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtnkxlnlps.html

[M04] 获取当前工作目录
来源：http://hz.iojbl.cn/gttcsabaxf.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtnazhgvec.html

PHP:  getcwd();
来源：http://hz.ydjk.org.cn/gtfyapbiut.html

JS:   process.cwd()
来源：http://hz.fengsongda.top/gtjgqvbclq.html

TS:   process.cwd()
来源：http://hz.gogol.net.cn/gtqrwglqux.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtqygghhvb.html

Go:   os.Getwd()
来源：http://hz.ydjk.org.cn/gtvjrogegg.html

Ruby: Dir.pwd
来源：http://hz.fzhhl.top/gtfrmeamfv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.52xcode.cn/gthpshtueo.html

[M05] 设置退出码
来源：http://hz.zhongyouzk.top/gthgrdyexx.html

Py:   sys.exit(1)
来源：http://hz.tian-w.cn/gtjbtgpguy.html

PHP:  exit(1);
来源：http://hz.quarkkingdee.top/gthmlhhwlg.html

JS:   process.exit(1)
来源：http://hz.shuidangran.top/gtxhoizrvr.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gtnitzkkdv.html

Java: System.exit(1)
来源：http://hz.jiagoushi.top/gtloupjnfk.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangtech.top/gttbdrfbow.html

Ruby: exit 1
来源：http://hz.guowangkeji.top/gtcrwxgytx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gogol.net.cn/gtmrbheelm.html

[M06] 向标准错误输出
来源：http://hz.nanxuanxn.top/gtazgwjsmo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtcichalqa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258.top/gtcuyjpfgg.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtapjnmmnx.html

TS:   console.error("err")
来源：http://hz.smart0.xyz/gtwxrdwsbs.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gtufykkmeu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nwbrower.top/gtpufqdzll.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gtrtealefv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.meibo888.top/gtxtdasrzk.html

[M07] 判断是否为主入口
来源：http://hz.yueranfly.top/gtbasqhbtm.html

Py:   if __name__ == "__main__":
来源：http://hz.gogol.net.cn/gtoydaunds.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangkeji.top/gtvpvuqwmz.html

JS:   require.main === module
来源：http://hz.ehwqpu.com/gtmenaczjz.html

TS:   require.main === module
来源：http://hz.xziqi.cn/gtjrgejjow.html

Java: public static void main(String[] args)
来源：http://hz.jinqigufen.top/gteicfynic.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gtwxyhbrqn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.52xcode.cn/gtgobxzmol.html

C#:   static void Main(string[] args)
来源：http://hz.yvedp.cn/gtkowjbmeb.html

[M08] 获取系统与运行时信息
来源：http://hz.xuetiantiany.cn/gtkhrjbsas.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtkgrkdjoo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aizwys.cn/gtqejhalfu.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtvfwvdlik.html

TS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtgkpreule.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gtdzjeyfcc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gtfjlykfoj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxinkj.top/gtrqshuvvy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtmbdbmere.html

================================================================================
来源：http://hz.gogol.net.cn/gtjownisns.html

N. 数据结构与算法
来源：http://hz.sxryk.cn/gtxgzmizmo.html

================================================================================
来源：http://hz.xinyue.icu/gtjnelniyw.html

[N01] 二分查找（有序数组）
来源：http://hz.zhiwuduotai.top/gtpqaxqarg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtejdigzoe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinghuilouyu.cn/gtzbluargx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shangyingyoupin.top/gtjbgepbna.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtbfzutrrz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.smart0.xyz/gtezxjpyky.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cashguo.top/gtavbuouhu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cashguo.top/gtmrxkkfaq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtggkzfdtg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xziqi.cn/gtjzsleyns.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtrmjducbl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgufenzy.top/gtqhuyxjpl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtkjttszlt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtgckgvebf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.redwolf501.top/gtbvuuqljz.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtkrjeecbz.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtznxezkxc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxuanxn.top/gtasrllylr.html

[N03] 快速排序（分治示例）
来源：http://hz.ehwqpu.com/gtsowypaow.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuetiantiany.cn/gtflqemodl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ybcxt.top/gtmlvdidtd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtmmvxruna.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtribjgxzp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gtfhvqfnro.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.andypj.xyz/gtbdcxufzh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hywenlv.cn/gtkreohrfo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtlyrjrqjm.html

[N04] 斐波那契数列
来源：http://hz.tian-w.cn/gtoqnwhxam.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtoxttvkzz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gtuefiauur.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtalohxghq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gttglveoqd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangshuangyany.cn/gtctweifrr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtwtiiwlgw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtlgpylcgr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtzjavexlw.html

[N05] 最大公约数
来源：http://hz.havefunace.top/gtrmtlmukf.html

Py:   math.gcd(a, b)
来源：http://hz.cheryme.top/gtjgusrfoq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.vqdsnc.cn/gtolijmlzp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtunhqibpd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtgxezwrit.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhijiandao.cn/gtdvdolhls.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gtreuuktha.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtnabspavd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sxryk.cn/gtokldhwyo.html

[N06] 判断回文字符串
来源：http://hz.9152youxi.cn/gtcswgqmdh.html

Py:   s == s[::-1]
来源：http://hz.yanxiufei.cn/gtfytohfnu.html

PHP:  $s === strrev($s);
来源：http://hz.jqgfzy.top/gtbbkiorpz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtqeswazsr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gteeboqmqm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtbwqynwtg.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gtqorhobkl.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtwuoabeef.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gthcmqnqgy.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigufen.top/gttejtotrt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.feifeiyinyue.top/gtbnxrnlac.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cashguo.top/gtxvhgemrt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.dianchejie.cn/gtuvbkxqrx.html

TS:   // 手写 Map<string, number>
来源：http://hz.gotoacloud.top/gtfddnofap.html

Java: // 手写 HashMap
来源：http://hz.jinghuilouyu.cn/gtybjnvdod.html

Go:   // 手写 map[int]int
来源：http://hz.gogol.net.cn/gtgadqxlyn.html

Ruby: // 手写 Hash
来源：http://hz.zhiwuduotai.top/gtimagqekh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhijiandao.cn/gtculuzswo.html

[N08] 生成全排列
来源：http://hz.ybcxt.top/gtmhtfknvu.html

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gtvalrkgfd.html

PHP:  // 手写递归交换
来源：http://hz.chenjidiqi.icu/gtqmyvcwuq.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtlyfiqfml.html

TS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtsggsmaln.html

Java: // 手写回溯递归
来源：http://hz.jyoumei.cn/gtsbmuddnm.html

Go:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtvvjobubv.html

Ruby: arr.permutation.to_a
来源：http://hz.ivvv.top/gtmoomtbsa.html

C#:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtcvvvaaiq.html

[N09] 栈与队列
来源：http://hz.yj20258.top/gtdxgvcbqy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gtchxpgfhv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tian-w.cn/gtxmknwknr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ydjk.org.cn/gtwtatksvh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.snrcjt.cn/gtjhpgmfpc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gtqyutqbwh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenlongwang.top/gtfhwlvdpd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gtkjzarssg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jqgfzy.top/gtezzumypx.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangkeji.top/gtsbkrgvox.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtrhrzexvs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgfzy.top/gteygitgbt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtrmjzmnnm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhijiandao.cn/gtqqmeevng.html

Java: class Node { int v; Node next; }
来源：http://hz.yongpay.top/gtxfekwbvq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgfzy.top/gthnntbjxr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.mhx1999.top/gtizmbltdt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ivvv.top/gtwoketanp.html

[N11] 二叉树中序遍历
来源：http://hz.hnxiangtu.top/gtwujhfqdj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.c1oappe.top/gtmjglqlrk.html

PHP:  // 手写递归函数
来源：http://hz.cucudq.cn/gtupteuvqg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtuhhiozjv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtskffqlrp.html

Java: // 手写递归
来源：http://hz.fengsongda.top/gteoazzdjl.html

Go:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtytwnaisy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhongyouzk.top/gtmothqbcy.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtwpigedbs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tianlin.xyz/gtbbuzuuuu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgufenzy.top/gttcchwcua.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.birdmap.top/gtsulwbooc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnqzz.top/gtxedwebwv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnqzz.top/gtkpjqsegl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtsrkbifxp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gtbwkkbjul.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtmrqhpsok.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtbufapoeh.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtigkyawqq.html

O. 并发与异步
来源：http://hz.zhoulong.xyz/gtsqktkext.html

================================================================================
来源：http://hz.havefunace.top/gtnmctkxbn.html

[O01] 启动一个线程
来源：http://hz.chenjidiqi.icu/gttzsvvahl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.316326.xyz/gtrfmvgpre.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtavadeddw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinyuanbaomall.cn/gtueymzsfg.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtsmotexeg.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gtoqqfwvoe.html

Go:   go f()
来源：http://hz.zdqjudy.top/gtbetibgxn.html

Ruby: Thread.new { f }
来源：http://hz.yueranfly.top/gttjrajouc.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtszkqgshy.html

[O02] 使用线程池
来源：http://hz.hfpthk.cn/gtgiydzxek.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtfcvlrbam.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gzhubu.top/gtktkrttjb.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtxyoqgips.html

TS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtpjllmlbp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gtvogyvskh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ybcxt.top/gthxmnetpf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtmnxalcog.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangshuangyany.cn/gtlqrpotgs.html

[O03] 加锁保护共享数据
来源：http://hz.gzhubu.top/gtkgupvawd.html

Py:   with lock: shared += 1
来源：http://hz.yj20258888.top/gtxskxetlt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gtdttinjhp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinghuilouyu.cn/gtzbijtpzx.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtthyzozbm.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gtltefwucf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gtbjzvqcpu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.316326.xyz/gtmcbngigg.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtjgkcdtox.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtwtfqhaqa.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtygzszhha.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhijiandao.cn/gtmotrdarm.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtcgbsvnkq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtephumwft.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gzhubu.top/gtqmjrmjrj.html


<!-- 参考信息 -->