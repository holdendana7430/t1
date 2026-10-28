代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gtdbpebpjy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gtjgykquqz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ybcxt.top/gtlgbvijaj.html

[L02] 发送 POST JSON
来源：http://hz.ppjwa.cn/gttlsqgivr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhijiandao.cn/gtnisnemld.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hammf.cn/gtrhbvyrju.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtzcjcmbmr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtqrfatpjq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gtepboewok.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtybsjgtst.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtmduasxns.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtlwbrkirw.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtpqamhfhv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tianlin.xyz/gtgsyzhydb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtdmctupsq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gttvvkcqnm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtqpwazrcs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxuanxn.top/gtxejrzxui.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtogknjjix.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtoidbrulz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtjurwhxfr.html

[L04] 设置超时
来源：http://hz.yueranfly.top/gtuohmfhuz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtywbwdonb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daxiang520.top/gtraqcoyrt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtzuklhgox.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtcfpoorrp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtjcxqnmzv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.vqdsnc.cn/gtcovyynhf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gtytmtvwmk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ybcxt.top/gtobvsonom.html

[L05] 上传文件（multipart）
来源：http://hz.cdnleiting.top/gtbocafmce.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cheryme.top/gtllndkfvs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtdghibykt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gzhubu.top/gtbfugidea.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigufen.top/gtfjtbaqop.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sweek.top/gtqelfnbvl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hongshengwenyu.top/gtajedigte.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.feifeiyinyue.top/gtzxyqydnd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shuidangran.top/gttseugrry.html

[L06] 解析响应为 JSON
来源：http://hz.smart0.xyz/gtplyrfkqa.html

Py:   resp.json()
来源：http://hz.cashguo.top/gtnrpmbrjs.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gthalfiruh.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtxwecpifl.html

TS:   await resp.json()
来源：http://hz.daxiang520.top/gtnhuzutex.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenlongwang.top/gtfunzcqcb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zdqjudy.top/gthjsgdnxz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pycfn.com/gtrtmvbdgs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fzhhl.top/gtllttrlqd.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtukxuwxkn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dashuyun.cn/gtituasghz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jyoumei.cn/gtqgqvsrkw.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtdjinbmyh.html

TS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtimgdxuwu.html

Java: resp.statusCode()
来源：http://hz.iojbl.cn/gtcnqvkslt.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtzucxntmf.html

Ruby: resp.code.to_i
来源：http://hz.jiagoushi.top/gtpwantzdq.html

C#:   (int)resp.StatusCode
来源：http://hz.smart0.xyz/gtkmhbubto.html

[L08] 并发请求多个地址
来源：http://hz.hnxiangtu.top/gtmfskwzam.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenlongwang.top/gtwhnpjrwl.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtbynspqxb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtwifymdjy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtstssznoq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gzhubu.top/gthyrugnfl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.havefunace.top/gtxjupfcpe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ppjwa.cn/gtyswhjaia.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gtkyoppund.html

================================================================================
来源：http://hz.jyoumei.cn/gtqtalzetn.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtmhocbfyj.html

================================================================================
来源：http://hz.xziqi.cn/gtpvzprafb.html

[M01] 读取命令行参数
来源：http://hz.cdnleiting.top/gtecvmfvyy.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gtbhdkcuvv.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtyxxcbaph.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtgidtxwsc.html

TS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtzcvozyeo.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtdqrpmfen.html

Go:   os.Args[1:]
来源：http://hz.cdnleiting.top/gtahhodvec.html

Ruby: ARGV
来源：http://hz.shanyushiyangkeji.top/gtftdyflcy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gthlfvnnmc.html

[M02] 读取环境变量
来源：http://hz.zhongyouzk.top/gtxzuvvyxj.html

Py:   os.environ.get("HOME")
来源：http://hz.xziqi.cn/gttedexvec.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gtrnhvhfqd.html

JS:   process.env.HOME
来源：http://hz.cqqwz.cn/gtwylsxbxq.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtjjfjloim.html

Java: System.getenv("HOME")
来源：http://hz.fengsongda.top/gtedokhhjr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cheryme.top/gtvefdqfrb.html

Ruby: ENV["HOME"]
来源：http://hz.fengsongda.top/gtbiwmrbos.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guannengcc.top/gtypyfoorx.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gtveiweyfp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shuidangran.top/gtojelisbk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtkbbdlkhg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtyfrpvhqu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtugtzrapf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtmayfjyzq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shzxlz.cn/gtjqetfhjm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtuuxjgorc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ivvv.top/gtdioxyfzq.html

[M04] 获取当前工作目录
来源：http://hz.jinyuanbaomall.cn/gthcbglyjz.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gtfeenljww.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gttfojszpx.html

JS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtzgoqjmsn.html

TS:   process.cwd()
来源：http://hz.gogol.net.cn/gtygynjagn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigufen.top/gtfiyewjpl.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtahgqyyaf.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gtxofzkzse.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxuanxn.top/gtyjimfxvy.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtyucfdcxw.html

Py:   sys.exit(1)
来源：http://hz.cucudq.cn/gtgmfusxia.html

PHP:  exit(1);
来源：http://hz.shuidangran.top/gtscvwbdvg.html

JS:   process.exit(1)
来源：http://hz.xziqi.cn/gthwchtvxv.html

TS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtdvawjnns.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gtyhuqdhdo.html

Go:   os.Exit(1)
来源：http://hz.zdqjudy.top/gtkyapjqej.html

Ruby: exit 1
来源：http://hz.havefunace.top/gtsuztqwiz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hysaishi.cn/gtysfztwsi.html

[M06] 向标准错误输出
来源：http://hz.pycfn.com/gtcipnhasp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtsjjpmlxy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ehwqpu.com/gtzlhbosos.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtehzlnytx.html

TS:   console.error("err")
来源：http://hz.wangdashe.top/gtjtwzrmix.html

Java: System.err.println("err")
来源：http://hz.jinghuilouyu.cn/gtawffkdna.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtnunchzan.html

Ruby: warn "err"
来源：http://hz.jlsjyb.cn/gtdnyfgkvc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daria6918.cn/gthxsbpkbm.html

[M07] 判断是否为主入口
来源：http://hz.fengsongda.top/gtsuuuyiuu.html

Py:   if __name__ == "__main__":
来源：http://hz.yuxming.cn/gtejcuxeal.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.0kj1m.cn/gtjtxdeecd.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtrwosboto.html

TS:   require.main === module
来源：http://hz.meibo888.top/gtxfuhfkdp.html

Java: public static void main(String[] args)
来源：http://hz.ydzc1.top/gthzyaliyx.html

Go:   func main()
来源：http://hz.smart0.xyz/gtzsgzdueh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cucudq.cn/gtthqprmiu.html

C#:   static void Main(string[] args)
来源：http://hz.quarkkingdee.top/gtxgckfglr.html

[M08] 获取系统与运行时信息
来源：http://hz.yueranfly.top/gtjbsitykz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aizwys.cn/gtssmeclxg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sufxvd.cn/gtvfmkmdqm.html

JS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtkqxeaimv.html

TS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtwvqkmgse.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.0kj1m.cn/gtkryukelw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gtgyylgpch.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtbfsuxhen.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtilumalco.html

================================================================================
来源：http://hz.c1oappe.top/gtmrjaycdh.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtbwytqhno.html

================================================================================
来源：http://hz.jianghu66.top/gtnhuswzyb.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtlrfopnib.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yongpay.top/gtzyzgcxpy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.vqdsnc.cn/gthkbtklak.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtjxfcxitm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtgipmgftl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gthkzqeeco.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gtncxjiytr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtlzyoqoiz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtiikqgeca.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258888.top/gtumjbdswm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtukzkzyfo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.iojbl.cn/gtrktczowe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtwehiidcj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtncwyhhed.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aibaodan.cn/gtyqhwqhwy.html

Go:   slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gteiqstflm.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtrfimghdw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zycfv.cn/gtftuikvpn.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gtbxsjlqhg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.52xcode.cn/gtbxazvzuw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtdpprzisg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtkaenagfx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtsefwykce.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtqzdhjgxs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuetiantiany.cn/gtogpxkhkf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zycfv.cn/gtbvhquazk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtieolhakm.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtagfeximt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtniqzyfiq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangtech.top/gtqqxhrtca.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtpxjkfhuw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtietehykr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtkhmjgvzt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xziqi.cn/gtallqjflr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtjigwgqgy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tianlin.xyz/gtzyewumwk.html

[N05] 最大公约数
来源：http://hz.guannengcc.top/gtomwbrgmv.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gtilbogxmc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtpotskwtq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtqmxtqdoh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtasplvhtz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sysykeji.top/gtbumkjuhb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxinkj.top/gtmmyjwmht.html

Ruby: a.gcd(b)
来源：http://hz.xinyue.icu/gtdkeajwer.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtbbextwwn.html

[N06] 判断回文字符串
来源：http://hz.jqgfzy.top/gtecqskcyu.html

Py:   s == s[::-1]
来源：http://hz.yonumen.top/gthcgioqri.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtqcutoxeb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gttuhbkehv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtgwstjpor.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigufen.top/gtfpybykwp.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtrszwemfr.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtjqedyohi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtseywpvlh.html

[N07] 两数之和（返回下标）
来源：http://hz.yvedp.cn/gtglnuzeyi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangdashe.top/gtainotsji.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.snrcjt.cn/gtsmfasdvk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtfkppqyvg.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtwuazfdqe.html

Java: // 手写 HashMap
来源：http://hz.redwolf501.top/gtoleilfrv.html

Go:   // 手写 map[int]int
来源：http://hz.ybcxt.top/gtbpsfmjsw.html

Ruby: // 手写 Hash
来源：http://hz.gogol.net.cn/gtfrnlrmum.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gtnwbfzknd.html

[N08] 生成全排列
来源：http://hz.zhiwuduotai.top/gtpkbsdywp.html

Py:   itertools.permutations(arr)
来源：http://hz.zhengqikj.top/gtrpmkzxtl.html

PHP:  // 手写递归交换
来源：http://hz.9152youxi.cn/gtcpeeltsg.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gthaozqqho.html

TS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gttqmruygh.html

Java: // 手写回溯递归
来源：http://hz.sysykeji.top/gthwtqtsal.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtmipoyyzl.html

Ruby: arr.permutation.to_a
来源：http://hz.hnxiangtu.top/gtxdkjbyig.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gthyuccdkl.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gtziupydew.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.52xcode.cn/gtpbnktsho.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yanxiufei.cn/gtswakbqhu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gtknqqditu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pengpengdd.cyou/gtazpehzau.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.vqdsnc.cn/gtnxcwpoyq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hongshengwenyu.top/gtyrcqxsfw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtwisukdfv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tianlin.xyz/gtbhlbgnje.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtnjymrlhs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gotoacloud.top/gtultgtpzf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.feifeiyinyue.top/gtrdjjwzlh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hywenlv.cn/gtpubcfkuc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ywan-chungtsiang.top/gtflfbhxbm.html

Java: class Node { int v; Node next; }
来源：http://hz.zhoulong.xyz/gtajpluuah.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.svipenyu.cn/gthvqazfsu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xingfuxueyuan.xyz/gtcauivbvv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhixingplan.top/gtvmzozajy.html

[N11] 二叉树中序遍历
来源：http://hz.hnqzz.top/gtndvdchly.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydzc1.top/gtupgfiqcb.html

PHP:  // 手写递归函数
来源：http://hz.52xcode.cn/gtjmucskoa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtmazqftpp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtdoocslhn.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtncxwdglj.html

Go:   // 手写递归
来源：http://hz.yongpay.top/gtyobcxhyl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.vqdsnc.cn/gtrpcjuoif.html

C#:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtytdtxegp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenjidiqi.icu/gtcdmitaaw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gthbubwqxv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gtcwqugyaz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtzqobtfbi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gtaiyhepjh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtabmymqqj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtdzksnznm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangkeji.top/gtmgxinnyp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jyoumei.cn/gtmelilsfw.html

================================================================================
来源：http://hz.meibo888.top/gtarasunky.html

O. 并发与异步
来源：http://hz.zhaomingkeji.xyz/gtswtdkinq.html

================================================================================
来源：http://hz.zhongyouzk.top/gtzrvagtty.html

[O01] 启动一个线程
来源：http://hz.hnxiangtu.top/gtsetypxrr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.redwolf501.top/gtasldjbxg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydzc1.top/gtzxtkcirg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtdbsreweb.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtkijiwhop.html

Java: new Thread(() -> f()).start()
来源：http://hz.tian-w.cn/gtsfrtvdmg.html

Go:   go f()
来源：http://hz.nanxinkj.top/gtyoabbakt.html

Ruby: Thread.new { f }
来源：http://hz.shangyingyoupin.top/gtxxxnqglk.html

C#:   Task.Run(() => F());
来源：http://hz.yanxiufei.cn/gtqyrupyvs.html

[O02] 使用线程池
来源：http://hz.hfpthk.cn/gtvdarnmkc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.fzhhl.top/gtcqgisjvb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yongpay.top/gttrcfukus.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtgxcqliog.html

TS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtwhzvyyoq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gzhubu.top/gtgjaqytrw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ehwqpu.com/gtrbkrhmzd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258.top/gtvfxkfsfe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.feifeiyinyue.top/gtzggehwhj.html

[O03] 加锁保护共享数据
来源：http://hz.guannengcc.top/gtomatzhia.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gtvkxierlx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tanke756.top/gtenttpgkn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.0kj1m.cn/gtvbemsxxd.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtmmxdoxbu.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtowjaokny.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangkeji.top/gtnkufawva.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtnnxcpcql.html

C#:   lock (gate) { shared++; }
来源：http://hz.hysaishi.cn/gttbyzzafc.html

[O04] 定义异步函数并等待
来源：http://hz.hnxiangtu.top/gtkxmsyrhx.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigufen.top/gtwnytchcq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aizwys.cn/gtfxfphoyy.html

JS:   async function f() { await g(); }
来源：http://hz.nwbrower.top/gtxhekwvug.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenlongwang.top/gtdwzchvat.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.fengsongda.top/gtlqzajvil.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jianghu66.top/gtorkzcoaq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jlsjyb.cn/gtderconcv.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtxovgicxk.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtphtvhyri.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigufen.top/gtdfvgbspu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtvrtfwjbi.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtqskwnaeo.html

TS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtamjteumh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtsdympndi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhengqikj.top/gtborbvtuo.html

Ruby: threads.map(&:join)
来源：http://hz.52xcode.cn/gtsvsbmahe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtlgeccntg.html


<!-- 参考信息 -->