代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnqzz.top/gtfqvskjdr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtqsgkugqh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtncuzshjg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuetiantiany.cn/gteciynpzt.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtgjdyegvg.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258888.top/gtpzjwimgw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtjvrbcfnd.html

================================================================================
来源：http://hz.meibo888.top/gtdduslxsf.html

L. 网络请求
来源：http://hz.hfpthk.cn/gtajvwkmii.html

================================================================================
来源：http://hz.jinqigufen.top/gtdmeuzfiq.html

[L01] 发送 GET 请求
来源：http://hz.zdqjudy.top/gtyqbqdtft.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtoqyxtnsu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shangyingyoupin.top/gteakasdqx.html

JS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtwwpriwrs.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtsgwqqjrz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.bjfxy.top/gtxckqsejt.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtpixksfdo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtncporjyx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hysaishi.cn/gtefggsqjs.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtetpzrttm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cqqwz.cn/gtrscfkjup.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.kuanghao11.cn/gtydlfoxyo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gthvcvqfio.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtvnfnitgt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gtlethfozi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuanzhike.top/gtvpxpygso.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guowangkeji.top/gtamihztgo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtrjydsssd.html

[L03] 设置自定义请求头
来源：http://hz.zhixingplan.top/gtlybuuxwu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xylfe.cn/gtpxvhqlxx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xylfe.cn/gtdttrsrcg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtwjdcvpcz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtsakmtajj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tian-w.cn/gtonvhvbcf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cqqwz.cn/gtltdnsnao.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.0kj1m.cn/gteenrvjrb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.andypj.xyz/gtvuptgqxe.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtuqgqnkwh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtesyieoem.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.svipenyu.cn/gtfazceunz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtpdcwkzfl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtylbioobx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgfzy.top/gtjcmpwdep.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gtqrwmuswk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.iojbl.cn/gtpaydqpxk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.redwolf501.top/gtblzzaibz.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtssvybcfa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jiagoushi.top/gtzpprhtkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtxfypqjgz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gthrlnkbeb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtxcaqcnwg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sxryk.cn/gtrdpbsvmh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtquvlguyo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxinkj.top/gtfeannnnm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tanke756.top/gtdnvkjsyy.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258888.top/gtqkwzfuvz.html

Py:   resp.json()
来源：http://hz.dianchejie.cn/gtgrrakjxu.html

PHP:  json_decode($body, true);
来源：http://hz.birdmap.top/gtylrwzoyb.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtihzimnnl.html

TS:   await resp.json()
来源：http://hz.jiagoushi.top/gtuaqihfdh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jyoumei.cn/gtcpsuzvaz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gtsfkzjxpf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.316326.xyz/gtzfeyjana.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.316326.xyz/gtifnrkdkt.html

[L07] 处理 HTTP 状态码
来源：http://hz.aibaodan.cn/gtbkwcqbfc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtwcayaglo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.feifeiyinyue.top/gteujvkghc.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gttkkncygl.html

TS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtzusaiekb.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gtfotnylsb.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtoihtrlio.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtimogsxka.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gtdppucfom.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtzimsfkie.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtjfmflwsd.html

PHP:  curl_multi_init() 系列
来源：http://hz.shangyingyoupin.top/gtheutvlym.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtnumyxhdr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtrrwdoleo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenlongwang.top/gtarofftia.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xziqi.cn/gtvdebcojm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtmthmwvqi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ehwqpu.com/gtuxluwfaw.html

================================================================================
来源：http://hz.snrcjt.cn/gtnneumakp.html

M. 命令行 / 进程 / 环境
来源：http://hz.ppjwa.cn/gtasgiidpi.html

================================================================================
来源：http://hz.hammf.cn/gtwfwftvdl.html

[M01] 读取命令行参数
来源：http://hz.cqqwz.cn/gtwoxxwnqb.html

Py:   sys.argv[1:]
来源：http://hz.xuanzx.com/gtzorzvosc.html

PHP:  $argv;  $argc;
来源：http://hz.52xcode.cn/gtkrzaarkt.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtgapwdswx.html

TS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtpmjennjc.html

Java: args 数组（main 方法参数）
来源：http://hz.chenlongwang.top/gtxdycseiz.html

Go:   os.Args[1:]
来源：http://hz.gaohongyu789.top/gtisydybnn.html

Ruby: ARGV
来源：http://hz.yongpay.top/gtdrhlfsdf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtvwzsscwg.html

[M02] 读取环境变量
来源：http://hz.gzhubu.top/gtfwsxmzrf.html

Py:   os.environ.get("HOME")
来源：http://hz.guannengcc.top/gtmpnybgxh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.redwolf501.top/gterxyyunn.html

JS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtdkpsfeyo.html

TS:   process.env.HOME
来源：http://hz.zdqjudy.top/gtapohxluu.html

Java: System.getenv("HOME")
来源：http://hz.gotoacloud.top/gtfpwkzmvc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtvrvkcycm.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gtkcefqcwy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dianchejie.cn/gtdzjleqyr.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtkdkspiak.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yangfankeji.com/gtwlxbgaxy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ybcxt.top/gthrenfuqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtdjzcbpey.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtevcsulqi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.snrcjt.cn/gtwfnyzutv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gteypxlhak.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtnpabaevp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtpzeoxlff.html

[M04] 获取当前工作目录
来源：http://hz.jqgfzy.top/gtcycdvdel.html

Py:   os.getcwd()
来源：http://hz.xinyue.icu/gtdztwmakt.html

PHP:  getcwd();
来源：http://hz.shanyushiyangkeji.top/gtrybnsfwv.html

JS:   process.cwd()
来源：http://hz.wangdashe.top/gtyfszrnej.html

TS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtrfwzexeq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gotoacloud.top/gtobahhodq.html

Go:   os.Getwd()
来源：http://hz.yongpay.top/gtifiszqsi.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gttyyiqxnk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gthtntmnxn.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtxzhxecbc.html

Py:   sys.exit(1)
来源：http://hz.fzhhl.top/gtanslvggv.html

PHP:  exit(1);
来源：http://hz.hammf.cn/gtnrefmsgi.html

JS:   process.exit(1)
来源：http://hz.sysykeji.top/gthhsswvac.html

TS:   process.exit(1)
来源：http://hz.0kj1m.cn/gthrsdezbl.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gtjqzbfmbz.html

Go:   os.Exit(1)
来源：http://hz.kuanghao11.cn/gtklshtbek.html

Ruby: exit 1
来源：http://hz.chenzaomai.com/gtcuzjrgad.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gtjnfhspcq.html

[M06] 向标准错误输出
来源：http://hz.cdnleiting.top/gtyycqwayt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtobrsrxey.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nwbrower.top/gtefkifbeu.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gttkravagf.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtshpepijz.html

Java: System.err.println("err")
来源：http://hz.yanxiufei.cn/gtoccgofwg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnxiangtu.top/gtplrwwaqi.html

Ruby: warn "err"
来源：http://hz.tianlin.xyz/gtgxfpwsxd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtunkccgjb.html

[M07] 判断是否为主入口
来源：http://hz.xuetiantiany.cn/gtxnsaxtdt.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtkdjcrkrd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ppjwa.cn/gtbjcznrri.html

JS:   require.main === module
来源：http://hz.hnqzz.top/gtdhbcztpp.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtfprbvzja.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtueikxfst.html

Go:   func main()
来源：http://hz.bjfxy.top/gtfvgeqzwr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.feifeiyinyue.top/gthwznqdbp.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtogsitkil.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gtqnxxqhzj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtdwozccsl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.kuanghao11.cn/gtrhwabzof.html

JS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtflblyjba.html

TS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtzbhdyfce.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigufen.top/gtohxntabk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.snrcjt.cn/gtkhbxdwxz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangshuangyany.cn/gtmyrnezfz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dashuyun.cn/gtbbfryayx.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgbotggns.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtnbakqtjl.html

================================================================================
来源：http://hz.wangdashe.top/gteaifepzg.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtbxnqiscm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtpisgvocc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtygyzesvw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtvjcdsicc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtgqqowatt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtrhcnjini.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtwvwcabek.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sysykeji.top/gtatyrzwxn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinghuilouyu.cn/gtgugqxgas.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gtltpacyox.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtoothriar.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhixingplan.top/gtvpgvxoyj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gthkkjutol.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtqvjxmcjl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxuanxn.top/gtwutraikj.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtncsdqkwt.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtkmjgnddz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtvauawaod.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtawidzqny.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.iojbl.cn/gtjtyhlmgp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgufenzy.top/gtualnuacy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sysykeji.top/gtnbzekbay.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtabijkmyo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtlrncufzk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.iojbl.cn/gtdgdkwncs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtwxrnaeqw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtbddauwzi.html

[N04] 斐波那契数列
来源：http://hz.shuidangran.top/gtdwuyfiue.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtribqzskg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtvpfxvrqx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhengqikj.top/gtxqxulviq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtzglkxjwq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.kuanghao11.cn/gtrnbvsjvx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jianghu66.top/gtjywsfedq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtkwzlhasr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gttbhuhcvh.html

[N05] 最大公约数
来源：http://hz.zhijiandao.cn/gtuqzzuhdw.html

Py:   math.gcd(a, b)
来源：http://hz.yueranfly.top/gtuqzuqsms.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ywan-chungtsiang.top/gtqxhtvyal.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtavyxozoi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtojptteam.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj202588.top/gtpnbcybkf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gtgxlxhuzc.html

Ruby: a.gcd(b)
来源：http://hz.yj20258888.top/gtsqsjuzad.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nwbrower.top/gtrjrlqnlm.html

[N06] 判断回文字符串
来源：http://hz.shzxlz.cn/gtijmmxcai.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtjevcfbub.html

PHP:  $s === strrev($s);
来源：http://hz.ybcxt.top/gtbdvopyfp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtwhaytdvn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtrvrfsrrs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shuidangran.top/gtkcezkbkx.html

Go:   // 双指针从两端比较
来源：http://hz.xuetiantiany.cn/gtofdgynkw.html

Ruby: s == s.reverse
来源：http://hz.sufxvd.cn/gtkwwhfsnk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtemmhdaiw.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtxpdqrynj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.birdmap.top/gtwkgeiecc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxinkj.top/gtzmroqwji.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aibaodan.cn/gtbjxnabmc.html

TS:   // 手写 Map<string, number>
来源：http://hz.yueranfly.top/gtzbtjunqa.html

Java: // 手写 HashMap
来源：http://hz.zhixingplan.top/gtpnceizso.html

Go:   // 手写 map[int]int
来源：http://hz.birdmap.top/gtvxfaiawl.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtdkmnukxz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tian-w.cn/gtjpawrojy.html

[N08] 生成全排列
来源：http://hz.hnqzz.top/gtxxtzzgbi.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtjugexwfq.html

PHP:  // 手写递归交换
来源：http://hz.yj20258.top/gtegverwpw.html

JS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtscoalvad.html

TS:   // 手写回溯递归
来源：http://hz.sweek.top/gtpsmxbwio.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtomaxbmlp.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtjhmgzkkl.html

Ruby: arr.permutation.to_a
来源：http://hz.smart0.xyz/gtplbtrctz.html

C#:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtuvtnblyo.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtrjdaejza.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tianlin.xyz/gtkbtdbhrh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuxming.cn/gtunseigsb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtirsriieb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtkweyopru.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zdqjudy.top/gtdwyspvxb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtjiaajyos.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.andypj.xyz/gtxzoodtth.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sweek.top/gtublefawm.html

[N10] 链表节点定义
来源：http://hz.zhiwuduotai.top/gtrfynwvrp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gaohongyu789.top/gtinbkcgnn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tanke756.top/gtowmqumso.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinghuilouyu.cn/gtxhfryapo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangdashe.top/gtfayvgwxl.html

Java: class Node { int v; Node next; }
来源：http://hz.9152youxi.cn/gtixvbvldh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangkeji.top/gthbrltwxs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.316326.xyz/gtkpcnqmwf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgfzy.top/gtlgnxzfxn.html

[N11] 二叉树中序遍历
来源：http://hz.fzhhl.top/gtgoucyear.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.bjfxy.top/gtipzxvflz.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtgwvnzfgn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtjwrmxmwg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtanmjtjle.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gtlodzigna.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtpeewqcig.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gtnopjsvgz.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gttavktygd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ivvv.top/gtmmmodjen.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtltsbjtyj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.meibo888.top/gtqnqgwozo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtcshbolry.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtvtyhrmwm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtbyeqvsdj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ehwqpu.com/gtvdpmqyxh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtthuhqulc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtsgkzygyc.html

================================================================================
来源：http://hz.smart0.xyz/gttryusxph.html

O. 并发与异步
来源：http://hz.zhaomingkeji.xyz/gtdcjymunt.html

================================================================================
来源：http://hz.xinyue.icu/gtuphlbzas.html

[O01] 启动一个线程
来源：http://hz.52xcode.cn/gthdyqnhmu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtrkmaeiry.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnxiangtu.top/gtafrbjivh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtrvbczdji.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtzlszfamg.html

Java: new Thread(() -> f()).start()
来源：http://hz.iojbl.cn/gtskghxrwt.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtowroyjue.html

Ruby: Thread.new { f }
来源：http://hz.hnxiangtu.top/gtgnleyfqi.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gttdzmuxrt.html

[O02] 使用线程池
来源：http://hz.ydzc1.top/gtozintouh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jlsjyb.cn/gtpvewzoqy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ehwqpu.com/gtuctdrcbk.html

JS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gtvoksrpsm.html

TS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtxdmlpzoh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhoulong.xyz/gtfganjhif.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gtwqpdnken.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtsbzqqvre.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhaomingkeji.xyz/gtnbgbsxsr.html

[O03] 加锁保护共享数据
来源：http://hz.tian-w.cn/gtsbacfmyt.html

Py:   with lock: shared += 1
来源：http://hz.zhengqikj.top/gtcztmdydn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pengpengdd.cyou/gtluyuwqgv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.birdmap.top/gtvajdvvjy.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtttgpjppe.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtfnhyxnnf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ybcxt.top/gtzdhtscom.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.9152youxi.cn/gtfcrxqvnl.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtyrjoxqiu.html

[O04] 定义异步函数并等待
来源：http://hz.smart0.xyz/gtlaijfnba.html

Py:   async def f():⏎    await g()
来源：http://hz.zhongyouzk.top/gtpoijnnda.html


<!-- 参考信息 -->