代发 wailian999

Go:   encoding/gob
来源：http://hz.chenjidiqi.icu/gtslqtythd.html

Ruby: Marshal.dump(obj)
来源：http://hz.kuanghao11.cn/gtemtundgx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtkdagsupx.html

================================================================================
来源：http://hz.hywenlv.cn/gtuprrhpyl.html

L. 网络请求
来源：http://hz.yangfankeji.com/gtxlwqwwzl.html

================================================================================
来源：http://hz.hnqzz.top/gtdmbwezir.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtrsntwezm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hysaishi.cn/gtqyzecmxd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sweek.top/gtchmayiqs.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtbvgxiiud.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gthbwkkwnu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.smart0.xyz/gtbaxaytrc.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhaomingkeji.xyz/gtqxiqcblj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtzxjeckkv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangdashe.top/gttsqkgzpf.html

[L02] 发送 POST JSON
来源：http://hz.0kj1m.cn/gtuezasnuk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtsyaegkhg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtucfcjgtq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtqamvdkpf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gtcvfvvlcy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aizwys.cn/gthwgxmxhe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtohubvnct.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.kuanghao11.cn/gtxjmshsix.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtvscuvzgg.html

[L03] 设置自定义请求头
来源：http://hz.yvedp.cn/gtgwpuwypg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shuidangran.top/gtwuszilsz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtwfpxcnny.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtimaetltf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgufenzy.top/gtfsbsewqr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.svipenyu.cn/gtatkryjei.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtkyteyuiv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cucudq.cn/gtzdjejlaq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtatajzhkm.html

[L04] 设置超时
来源：http://hz.shanyushiyangkeji.top/gtkbqceynd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenzaomai.com/gtbpppwgak.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hammf.cn/gtjaixpcik.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtbuchduyd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtikmtkjkc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtnkrdgspm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtrgkbhkjp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tianlin.xyz/gtcuuconpc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtlexmxmlc.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258.top/gtyxfcypbt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxuanxn.top/gtcobjhpjo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtbnyyutov.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtvuasxevi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtnmgikbbo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuxming.cn/gtcpllzsdx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hammf.cn/gtzoyjjnrp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydjk.org.cn/gtqcnhzhed.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.9152youxi.cn/gtyfotvhhe.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigufen.top/gteymhawro.html

Py:   resp.json()
来源：http://hz.wangshuangyany.cn/gtorfkyerl.html

PHP:  json_decode($body, true);
来源：http://hz.ywan-chungtsiang.top/gtzdayqvlf.html

JS:   await resp.json()
来源：http://hz.nanxuanxn.top/gtezengtvd.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtjztgmfeh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinghuilouyu.cn/gtvhpmqrmr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gtddloxkzm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtsuwhmgjv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.316326.xyz/gtfimtbbkq.html

[L07] 处理 HTTP 状态码
来源：http://hz.guowangkeji.top/gtyyqihgac.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangdashe.top/gtwlmxepsf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtnwvbycby.html

JS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtsprtuflm.html

TS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtyisqdddu.html

Java: resp.statusCode()
来源：http://hz.jinyuanbaomall.cn/gtrkurqeis.html

Go:   resp.StatusCode
来源：http://hz.sysykeji.top/gtvcddomjl.html

Ruby: resp.code.to_i
来源：http://hz.yangfankeji.com/gtjwuzvibp.html

C#:   (int)resp.StatusCode
来源：http://hz.zhongyouzk.top/gtpnydueoh.html

[L08] 并发请求多个地址
来源：http://hz.zhongyouzk.top/gtseyypars.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtpirutuok.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtfxzncqxe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtaqyocrux.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtairqvpaa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.snrcjt.cn/gtrejqyjhi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtzguppzzy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtjwksxjsy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gtqmxtllri.html

================================================================================
来源：http://hz.bjfxy.top/gtsobkwaog.html

M. 命令行 / 进程 / 环境
来源：http://hz.xylfe.cn/gtctzgwraq.html

================================================================================
来源：http://hz.xylfe.cn/gtvyitfmbb.html

[M01] 读取命令行参数
来源：http://hz.52xcode.cn/gtadljhgec.html

Py:   sys.argv[1:]
来源：http://hz.xingfuxueyuan.xyz/gtkgwsipqg.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtqwqkcoro.html

JS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtitntoqiw.html

TS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gtqbpdqxdt.html

Java: args 数组（main 方法参数）
来源：http://hz.gzhubu.top/gtqrabpngp.html

Go:   os.Args[1:]
来源：http://hz.zhaomingkeji.xyz/gttonxlenl.html

Ruby: ARGV
来源：http://hz.xuanzx.com/gtmxjxamfx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daxiang520.top/gtougczpfc.html

[M02] 读取环境变量
来源：http://hz.yuxming.cn/gtbieljxvm.html

Py:   os.environ.get("HOME")
来源：http://hz.zhoulong.xyz/gtnpjwvytu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.kuanghao11.cn/gtbkjjgego.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtcnuwpgwr.html

TS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtrkkhgeir.html

Java: System.getenv("HOME")
来源：http://hz.cucudq.cn/gtoxxgtxjp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj202588.top/gthbgacnun.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtvyysftfy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gthnjvuqnv.html

[M03] 执行外部命令
来源：http://hz.shuidangran.top/gttaicwxaw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtsdtzknqp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtilfcbgcj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gtwlihyrfv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtriwshbpi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ivvv.top/gtgkvjhkzx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yanxiufei.cn/gtjgeqsulo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtxwbwwlqu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgfzy.top/gtjalbgfyr.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtawfnpqhc.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gtgkgbxhmz.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gtbyalayzw.html

JS:   process.cwd()
来源：http://hz.guowangkeji.top/gtzqcmscdf.html

TS:   process.cwd()
来源：http://hz.chenzaomai.com/gtqbkeniuh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daria6918.cn/gtagzbjzfj.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtmrxndvto.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtrlvsneml.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtjqcxqgjz.html

[M05] 设置退出码
来源：http://hz.sufxvd.cn/gtuxlqhrut.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtztfmfblk.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gtkdiamakh.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtcfniwuza.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtozvkvvfa.html

Java: System.exit(1)
来源：http://hz.jiagoushi.top/gtnivecykk.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtpwpmpvir.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtlzqcuskf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.smart0.xyz/gtflnassxt.html

[M06] 向标准错误输出
来源：http://hz.cheryme.top/gthgstycay.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gttutufzsd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hfpthk.cn/gthdkbaxft.html

JS:   console.error("err")
来源：http://hz.dianchejie.cn/gtixtirjqe.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtejdynmtr.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gthlgcmagh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxuanxn.top/gtgpnxatft.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gtpvlpdezv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenzaomai.com/gtodzjyked.html

[M07] 判断是否为主入口
来源：http://hz.zhixingplan.top/gthsuiaefj.html

Py:   if __name__ == "__main__":
来源：http://hz.yonumen.top/gtcbmqwbwg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtmnxkepaf.html

JS:   require.main === module
来源：http://hz.wangdashe.top/gthstaibec.html

TS:   require.main === module
来源：http://hz.hfpthk.cn/gtjlinrnnc.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtztpwkbck.html

Go:   func main()
来源：http://hz.quarkkingdee.top/gtuzenykgp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.316326.xyz/gtltbjwnpe.html

C#:   static void Main(string[] args)
来源：http://hz.cashguo.top/gtyzsdgkuw.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gthxzdlloj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gtnbanburb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtnvghvaou.html

JS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtvuucpnfp.html

TS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtuqqoyoxk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daria6918.cn/gtpsnrdtwb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtvgwdlotb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fzhhl.top/gtnfyxtokg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ehwqpu.com/gtqriwguyn.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjfhnufgy.html

N. 数据结构与算法
来源：http://hz.ivvv.top/gtajovyvtg.html

================================================================================
来源：http://hz.jqgfzy.top/gtwkfegyhs.html

[N01] 二分查找（有序数组）
来源：http://hz.yuxming.cn/gtiwetpmhk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtefubkdmk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ehwqpu.com/gtibkfgjww.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtkdqieflx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtcifmtvkd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtiwzbooyb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.feifeiyinyue.top/gtpjggoxqf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gtthnawnzx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258888.top/gtvddvdegm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tanke756.top/gtzhrqjorc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtmnlxsonq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zdqjudy.top/gthwlauqpx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtkoumrlev.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtqwiibyhr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jlsjyb.cn/gtzhodatja.html

Go:   slices.Sort(arr)
来源：http://hz.pycfn.com/gtcgdlwfcp.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gtvenloxdr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtbbldhrii.html

[N03] 快速排序（分治示例）
来源：http://hz.haohaochexian.top/gtejcqklea.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigufen.top/gtjfbnspfz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenjidiqi.icu/gtolnnbayi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gteoclwrps.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtdbvvqkrb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.andypj.xyz/gtimmmsdqt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtzylgtznr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.mhx1999.top/gtttulxltk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yvedp.cn/gtrmwlaixm.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gttretyltk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtjwrhlnol.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gotoacloud.top/gtbygyicng.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtxlrtqljg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtfebbpwzt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ydjk.org.cn/gtjfwcxjfn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sysykeji.top/gtsbaxisnp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtdbtsqaah.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yvedp.cn/gtfeozdkmu.html

[N05] 最大公约数
来源：http://hz.iojbl.cn/gtjfysnwuc.html

Py:   math.gcd(a, b)
来源：http://hz.hysaishi.cn/gtcdwkpsjg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtwmdwsjei.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtvqbiuqki.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtokcxymlw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhaomingkeji.xyz/gtatwagtcs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtrivsjogc.html

Ruby: a.gcd(b)
来源：http://hz.fzhhl.top/gtvciosoqv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinghuilouyu.cn/gtxfbmsspa.html

[N06] 判断回文字符串
来源：http://hz.jyoumei.cn/gtvmaplmqa.html

Py:   s == s[::-1]
来源：http://hz.nanxinkj.top/gtzluukbja.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtdnhlmzod.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtsezoqteb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtngfrxkrl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgfzy.top/gtxmbvykbm.html

Go:   // 双指针从两端比较
来源：http://hz.sysykeji.top/gtshuawadb.html

Ruby: s == s.reverse
来源：http://hz.shuidangran.top/gtnwiwyigj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gthoeqtbkq.html

[N07] 两数之和（返回下标）
来源：http://hz.c1oappe.top/gtltopglka.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtdgzhfeys.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yangfankeji.com/gteknrrxrh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtnvicushs.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenjidiqi.icu/gtsrvpsfdj.html

Java: // 手写 HashMap
来源：http://hz.zhijiandao.cn/gtkhsrfdie.html

Go:   // 手写 map[int]int
来源：http://hz.yuanzhike.top/gtvmieerxt.html

Ruby: // 手写 Hash
来源：http://hz.sxryk.cn/gtotarsyfk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gogol.net.cn/gtqvuriaxm.html

[N08] 生成全排列
来源：http://hz.aibaodan.cn/gtrkjfcibb.html

Py:   itertools.permutations(arr)
来源：http://hz.tianlin.xyz/gtnojlghep.html

PHP:  // 手写递归交换
来源：http://hz.chenjidiqi.icu/gtmwpezwiq.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtebxrusku.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtgvotbllm.html

Java: // 手写回溯递归
来源：http://hz.jinqigufen.top/gtgpjadoqp.html

Go:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtrycubtha.html

Ruby: arr.permutation.to_a
来源：http://hz.shzxlz.cn/gtlzmbnnij.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtemfxipls.html

[N09] 栈与队列
来源：http://hz.zhongyouzk.top/gtnunjddck.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gaohongyu789.top/gtyvvrbxgh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhoulong.xyz/gtawjkwntt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aizwys.cn/gttmgjebmn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yonumen.top/gtweemhdfw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtsubznxgq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tianlin.xyz/gtaatrijrv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daria6918.cn/gtutpwnpxl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sysykeji.top/gtlyxfcnlb.html

[N10] 链表节点定义
来源：http://hz.iojbl.cn/gtsncnozfm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtwichlksf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtqaiozbgw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.dianchejie.cn/gtkrorcfty.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yuanzhike.top/gtvhxhzijm.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtzoilytqz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.havefunace.top/gtyckgszji.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sufxvd.cn/gtlltewqqd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.0kj1m.cn/gtbcepdduq.html

[N11] 二叉树中序遍历
来源：http://hz.kuanghao11.cn/gtravlcqjd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gthrrbiodn.html

PHP:  // 手写递归函数
来源：http://hz.mhx1999.top/gtpkuxxvrd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtzeuqybjo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtxppjaoyg.html

Java: // 手写递归
来源：http://hz.smart0.xyz/gtzwjokvpq.html

Go:   // 手写递归
来源：http://hz.gzhubu.top/gtgeizsacw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gtnxnvcthq.html

C#:   // 手写递归
来源：http://hz.guannengcc.top/gtpbbanakj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hammf.cn/gtadavopub.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yvedp.cn/gtbjhpunoo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guannengcc.top/gtezwboorg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtepmabrpg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtxijmcxoq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtrnalycme.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.feifeiyinyue.top/gtevxuiojf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cashguo.top/gtpvgxxxyh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtfzfidqzb.html

================================================================================
来源：http://hz.hfpthk.cn/gtaeoufbzc.html

O. 并发与异步
来源：http://hz.hfpthk.cn/gthweszifw.html

================================================================================
来源：http://hz.yj20258888.top/gtoafnrkip.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtnebzaedt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.9152youxi.cn/gtnblcjftg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jyoumei.cn/gtirudphgo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258888.top/gtzlmqskhn.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtznwszzoc.html

Java: new Thread(() -> f()).start()
来源：http://hz.ehwqpu.com/gtmsvrjgol.html

Go:   go f()
来源：http://hz.pycfn.com/gtgojxdcbv.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtsllgjtlo.html

C#:   Task.Run(() => F());
来源：http://hz.fengsongda.top/gtcotdsliq.html

[O02] 使用线程池
来源：http://hz.xziqi.cn/gtnbghevmo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.kuanghao11.cn/gthuzcimpw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtqbjyshdw.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtfsgpoidh.html

TS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtlodfilsu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shangyingyoupin.top/gtzyyuzfxn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tian-w.cn/gtneuaasvn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenjidiqi.icu/gtqzrdhdga.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxinkj.top/gthntggebv.html

[O03] 加锁保护共享数据
来源：http://hz.zycfv.cn/gtgzfbllhv.html

Py:   with lock: shared += 1
来源：http://hz.andypj.xyz/gtaiyjsvhk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xinyue.icu/gttlkftiuo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yanxiufei.cn/gtbjcvxvuc.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtjcqeviqt.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtmenpjmxi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sufxvd.cn/gtdjzconbb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinyuanbaomall.cn/gticbtlqsh.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxinkj.top/gtxgoglmkm.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtptyemaet.html

Py:   async def f():⏎    await g()
来源：http://hz.snrcjt.cn/gthacoqwlq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258888.top/gtfispklwv.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtyhvyqusx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtgczzsuay.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhongyouzk.top/gtrdikquii.html


<!-- 参考信息 -->