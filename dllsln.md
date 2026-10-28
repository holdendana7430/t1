代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.smart0.xyz/gtomfnwyqi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtylbbcixb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtunjzrdop.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gtlmvebfwv.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtbrxpnzga.html

Ruby: Marshal.dump(obj)
来源：http://hz.vqdsnc.cn/gtsddghuzk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtqwlsqzac.html

================================================================================
来源：http://hz.yonumen.top/gtworqlauq.html

L. 网络请求
来源：http://hz.jinghuilouyu.cn/gtepzdpdjv.html

================================================================================
来源：http://hz.ppjwa.cn/gtibuyldfn.html

[L01] 发送 GET 请求
来源：http://hz.sxryk.cn/gtktkapqem.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtgdrdewgj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.snrcjt.cn/gtydqpsump.html

JS:   await fetch(url)
来源：http://hz.sysykeji.top/gttowvnndb.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gthjkmytmo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258888.top/gtxurpldql.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigfzy.top/gtwnsjbzvr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aibaodan.cn/gtpuqqmaei.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtkqxpvsxl.html

[L02] 发送 POST JSON
来源：http://hz.hnqzz.top/gthhkowwhp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtlvkkbvaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinghuilouyu.cn/gtnmrxobgb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtcxxvpwze.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtawfvlwhy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtrluguogk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gtkfgzlzwd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtshylvrgw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhixingplan.top/gtnkjwstxa.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gteglgznup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gttfzkktwo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenzaomai.com/gtvyyfkzrg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gteeduwruw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtjhwpkwto.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gtpfjvgfpl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtkfnpvbma.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ehwqpu.com/gttlezegqc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fengsongda.top/gtwcoiviwt.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtsqjgccmo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sxryk.cn/gteajlhnxp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.iojbl.cn/gtabtlyqiv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtvtqntwnb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtirciqbuc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gteibqeuur.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.meibo888.top/gtuctcitzz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sxryk.cn/gtymukqpon.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtmocadwwf.html

[L05] 上传文件（multipart）
来源：http://hz.smart0.xyz/gtsjdcdnrq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtvrbqymfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtbobydjwt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtfuebvyyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258888.top/gtbzwnfuzd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtalzhgtsi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gaohongyu789.top/gtkdgmxpwz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cashguo.top/gtdsutmrxz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtiwnbkbld.html

[L06] 解析响应为 JSON
来源：http://hz.52xcode.cn/gtvzumsvxo.html

Py:   resp.json()
来源：http://hz.ivvv.top/gttngujwni.html

PHP:  json_decode($body, true);
来源：http://hz.feifeiyinyue.top/gtdwwhxcke.html

JS:   await resp.json()
来源：http://hz.yueranfly.top/gtvyqqcjhm.html

TS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtkcxehuhl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtvzvloyyc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtoinrfviw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gaohongyu789.top/gtcreofieq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtuduufnzo.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtdnqrehnu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tianlin.xyz/gtcdehwpur.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtortghglb.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtdejvfpxv.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtxpieyqcj.html

Java: resp.statusCode()
来源：http://hz.bjfxy.top/gtvxzkvmkw.html

Go:   resp.StatusCode
来源：http://hz.yuxming.cn/gtguxyhzne.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gtwrdycqvb.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtlbygwjfm.html

[L08] 并发请求多个地址
来源：http://hz.c1oappe.top/gtogxdjuml.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtxtqkvvuq.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtpfptqkhf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtzdyklsry.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtmthjolyw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtlycxhjbr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtfjsqdvje.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pycfn.com/gtxlhekggc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtzybjlyvb.html

================================================================================
来源：http://hz.9152youxi.cn/gtodxbhowt.html

M. 命令行 / 进程 / 环境
来源：http://hz.9152youxi.cn/gtirydiykc.html

================================================================================
来源：http://hz.dashuyun.cn/gtamoymgvl.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gtxwpnowsu.html

Py:   sys.argv[1:]
来源：http://hz.ywan-chungtsiang.top/gtqenlltwa.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtyjcgxbtq.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtrhyixdhe.html

TS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtvekmdzjd.html

Java: args 数组（main 方法参数）
来源：http://hz.daxiang520.top/gtludwcque.html

Go:   os.Args[1:]
来源：http://hz.shzxlz.cn/gtychxoeab.html

Ruby: ARGV
来源：http://hz.yj20258.top/gtjmequjlb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gttehxooiy.html

[M02] 读取环境变量
来源：http://hz.tianlin.xyz/gttiaipplr.html

Py:   os.environ.get("HOME")
来源：http://hz.chenzaomai.com/gtoksrcghu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtquvovgbe.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtlhrwfsgw.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtjgblqswz.html

Java: System.getenv("HOME")
来源：http://hz.zdqjudy.top/gttrkfeogl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gtpkqoevtq.html

Ruby: ENV["HOME"]
来源：http://hz.ydzc1.top/gtusauulle.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fengsongda.top/gtewyreofu.html

[M03] 执行外部命令
来源：http://hz.jlsjyb.cn/gtvfpwwsfg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtfogcobtx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gtwzqzkxkz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtmyvucvzj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtuwfucwot.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigufen.top/gtogeqechk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.52xcode.cn/gtqblzvppj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gtcuflylwb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dashuyun.cn/gtervaqwnm.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtldiyktyh.html

Py:   os.getcwd()
来源：http://hz.jqgfzy.top/gtwrbnvbsh.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gtgtweobzk.html

JS:   process.cwd()
来源：http://hz.daria6918.cn/gtbrcoamnm.html

TS:   process.cwd()
来源：http://hz.bjfxy.top/gtkoikxaqr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xylfe.cn/gtlvuinjtg.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gttyveplie.html

Ruby: Dir.pwd
来源：http://hz.cdnleiting.top/gtqixssfgz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sweek.top/gtrxxxrxyp.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gtjnwkqqpz.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtilpdzlev.html

PHP:  exit(1);
来源：http://hz.bjfxy.top/gtrvbjcrbu.html

JS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtppeearbf.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gtwjeyquan.html

Java: System.exit(1)
来源：http://hz.daria6918.cn/gtqllzzdyr.html

Go:   os.Exit(1)
来源：http://hz.quarkkingdee.top/gtoubxgnmd.html

Ruby: exit 1
来源：http://hz.cheryme.top/gtizlfztud.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jlsjyb.cn/gtwcjbgbvp.html

[M06] 向标准错误输出
来源：http://hz.hywenlv.cn/gtbdvsbaty.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yonumen.top/gtiahqqbgi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinyuanbaomall.cn/gttoepwxwm.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gtuasehsof.html

TS:   console.error("err")
来源：http://hz.sxryk.cn/gtsbkzmjam.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gtfkglzxfl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cucudq.cn/gtatqwrxah.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gtjldgzrlv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtgkqjphnc.html

[M07] 判断是否为主入口
来源：http://hz.cdnleiting.top/gtgjutxtbl.html

Py:   if __name__ == "__main__":
来源：http://hz.haohaochexian.top/gtcjhfsogm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydzc1.top/gtckcwtnzc.html

JS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtlqpixshd.html

TS:   require.main === module
来源：http://hz.yanxiufei.cn/gtztznicah.html

Java: public static void main(String[] args)
来源：http://hz.vqdsnc.cn/gtddivxmic.html

Go:   func main()
来源：http://hz.chenjidiqi.icu/gtzfhphbgx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xziqi.cn/gtglvhiqcj.html

C#:   static void Main(string[] args)
来源：http://hz.jinghuilouyu.cn/gtvalfsxtg.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtcycomhtl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hongshengwenyu.top/gtjzigmukv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.feifeiyinyue.top/gtoyioghtk.html

JS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gthyfsvnfc.html

TS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtuacefbmj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shangyingyoupin.top/gtwnzzbhdf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangkeji.top/gtqsoyqjwa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtormavpxd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenjidiqi.icu/gtdawerepp.html

================================================================================
来源：http://hz.tian-w.cn/gtuqmhbvog.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtfaudwkdt.html

================================================================================
来源：http://hz.chenzaomai.com/gtyvkkkkqv.html

[N01] 二分查找（有序数组）
来源：http://hz.hysaishi.cn/gtpiplnzqp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ivvv.top/gtfqrhodvp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhijiandao.cn/gteavoazfi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtexbqeqqe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtxuspqlew.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtorjfnvfr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gtrhkrnewy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cdnleiting.top/gtqmjdpebo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtdifsadqw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtffndrgjm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtajjtjktt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gteazrrnvz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtyrtywymx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtlasvverq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtbnqbogxp.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtdiyznoge.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtocglfnan.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtvjxbtzix.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gthmwygevn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hfpthk.cn/gtxlhadswn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtqluvgkci.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtxandlbrx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtylifsaxz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sxryk.cn/gtkrclswjk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.feifeiyinyue.top/gtsoeoblnl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhoulong.xyz/gtcmysduqe.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.kuanghao11.cn/gtctajlcmw.html

[N04] 斐波那契数列
来源：http://hz.yvedp.cn/gtydqvgmbm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.9152youxi.cn/gtlxrllrup.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shuidangran.top/gtwhofqreu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gtknqjerdh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtenokfwxc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtgjxmkwlb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtnmymplgk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtgluzfsvd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sweek.top/gtettehqdk.html

[N05] 最大公约数
来源：http://hz.mhx1999.top/gtxslqlgei.html

Py:   math.gcd(a, b)
来源：http://hz.dashuyun.cn/gtzzjvpiqd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gtvfkmqbwo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtcolfgubo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtqvdcgivn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.9152youxi.cn/gttrrialgv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guowangkeji.top/gtyadtqlwq.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtotgghxdm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gtsefbvmcv.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gtksnkqtmk.html

Py:   s == s[::-1]
来源：http://hz.cdnleiting.top/gtxrkmqltc.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtdroxpqwo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtmxywydcp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gthezhwhce.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnqzz.top/gtmruzcwzm.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtdktbyrxi.html

Ruby: s == s.reverse
来源：http://hz.yj202588.top/gtontdvsmu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gtrthgceog.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gttqegibfz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cashguo.top/gtdklyvafe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258888.top/gtjgxcwytb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhengqikj.top/gtyirnxxyk.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydzc1.top/gtxbzmckhu.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gthtkmnvto.html

Go:   // 手写 map[int]int
来源：http://hz.cdnleiting.top/gthlbntfbe.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtlocsaeqs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yonumen.top/gttkgjlsxn.html

[N08] 生成全排列
来源：http://hz.ppjwa.cn/gtccrjbeqo.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gthsegtoef.html

PHP:  // 手写递归交换
来源：http://hz.hongshengwenyu.top/gtlngddiaf.html

JS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtsygyjzsi.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtyezjnetb.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtoemyvatr.html

Go:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtjvxsohzk.html

Ruby: arr.permutation.to_a
来源：http://hz.aizwys.cn/gttlwbzcyj.html

C#:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtkdsffzls.html

[N09] 栈与队列
来源：http://hz.jyoumei.cn/gtmbkmnflq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gteafthpae.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtzbxrpbvv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gtcocvgbzb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.quarkkingdee.top/gtmaoxzjwa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gtudlfedfu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtclrupoqf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuanzx.com/gtjueaeist.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yanxiufei.cn/gtphvvqtyf.html

[N10] 链表节点定义
来源：http://hz.jinghuilouyu.cn/gtutaovnxc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gteahtzevy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtdmfaukry.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hysaishi.cn/gtpvzrqhfo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtijzzyzlf.html

Java: class Node { int v; Node next; }
来源：http://hz.wangdashe.top/gtkpctmctk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinyuanbaomall.cn/gtjzremxld.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtwigjxmwx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hfpthk.cn/gtywlqcgeg.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gteqphdqnx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aibaodan.cn/gtwfgfxgbf.html

PHP:  // 手写递归函数
来源：http://hz.zhixingplan.top/gthckdlmno.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtimvkyspk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtzxvuddvt.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtvxkrblut.html

Go:   // 手写递归
来源：http://hz.snrcjt.cn/gtzkjizrvh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yangfankeji.com/gtuypjufnt.html

C#:   // 手写递归
来源：http://hz.chenlongwang.top/gtwnralaam.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenzaomai.com/gtghetdotd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jlsjyb.cn/gtbfrgqvdl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guannengcc.top/gtluoltcfh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtdajdmppr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtlopaziam.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtrtjjwbzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtjabkhadx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xingfuxueyuan.xyz/gtiowcqbhc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gthdxdgblz.html

================================================================================
来源：http://hz.fzhhl.top/gtkoxzzunl.html

O. 并发与异步
来源：http://hz.chenjidiqi.icu/gttmdlhafz.html

================================================================================
来源：http://hz.hysaishi.cn/gtasmszmzp.html

[O01] 启动一个线程
来源：http://hz.sufxvd.cn/gtmjfbytee.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gthgjtscuc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinghuilouyu.cn/gtfdcgtkbz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenjidiqi.icu/gtskfsirky.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gtvdduvhfq.html

Java: new Thread(() -> f()).start()
来源：http://hz.dianchejie.cn/gtqiuzxuqj.html

Go:   go f()
来源：http://hz.jqgufenzy.top/gtecfjywdg.html

Ruby: Thread.new { f }
来源：http://hz.ydzc1.top/gttpzvzxeb.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gtrnfheoyc.html

[O02] 使用线程池
来源：http://hz.0kj1m.cn/gttqfqeuyo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhiwuduotai.top/gtifuowxue.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinyuanbaomall.cn/gttfcazdyj.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtyzgefxou.html

TS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gttxsirfwi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sweek.top/gtxzkwvfxb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxuanxn.top/gtajxrkpdo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhixingplan.top/gtobfvdqif.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangshuangyany.cn/gtizzwjwcf.html

[O03] 加锁保护共享数据
来源：http://hz.nanxinkj.top/gtjtmkjgnc.html

Py:   with lock: shared += 1
来源：http://hz.ivvv.top/gtrinnncbc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenlongwang.top/gtjosqurvk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xinyue.icu/gtmnteqhdu.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtphuolazb.html

Java: synchronized (this) { shared++; }
来源：http://hz.smart0.xyz/gtqasuyiws.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhaomingkeji.xyz/gtsgoysrpa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hysaishi.cn/gtawfgbmvy.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxinkj.top/gtfjgdrrgh.html

[O04] 定义异步函数并等待
来源：http://hz.hnqzz.top/gtomaiwruv.html

Py:   async def f():⏎    await g()
来源：http://hz.yangfankeji.com/gtlfxeesap.html


<!-- 参考信息 -->