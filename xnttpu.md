代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hnqzz.top/gtdnejujbu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gtoaibudzr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.52xcode.cn/gtxzyaibaq.html

Py:   pickle.dumps(obj)
来源：http://hz.hnqzz.top/gtxykrfipg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dianchejie.cn/gteznzohxc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtnjkduicz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtvzyqkfzh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuanzhike.top/gtjnhvyoso.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtngdlyjtf.html

Ruby: Marshal.dump(obj)
来源：http://hz.yvedp.cn/gtzqznsobo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinghuilouyu.cn/gthtxeobgc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjuwknguc.html

L. 网络请求
来源：http://hz.guannengcc.top/gtvayefdub.html

================================================================================
来源：http://hz.sweek.top/gtcnjzxjpe.html

[L01] 发送 GET 请求
来源：http://hz.ydzc1.top/gtagwhlbkb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.redwolf501.top/gtlzvqyoor.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jiagoushi.top/gtpvwabdfa.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtqgitvzkp.html

TS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtgcnakhyo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtncaakepg.html

Go:   resp, err := http.Get(url)
来源：http://hz.redwolf501.top/gtrhjtbbfi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.52xcode.cn/gtlvdntvhl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigfzy.top/gtfuqzobao.html

[L02] 发送 POST JSON
来源：http://hz.yuxming.cn/gtxpsexwcm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yongpay.top/gtaxwkzzel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daxiang520.top/gtoosagvzu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtuxvsntws.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtiprdzmls.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhengqikj.top/gtmiywtamj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cdnleiting.top/gtiljsnvmd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnxiangtu.top/gtlngecuap.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangshuangyany.cn/gtusheepjs.html

[L03] 设置自定义请求头
来源：http://hz.c1oappe.top/gtqhybgpvl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gthuvzuuxu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.havefunace.top/gtbghrepam.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtjvtzhvaq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtnacduixl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dianchejie.cn/gtmayibfnn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtyhhubkcq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigfzy.top/gtcejxqdgy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtizevzikp.html

[L04] 设置超时
来源：http://hz.guannengcc.top/gtzsitaedl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgufenzy.top/gtpeihwhpi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.c1oappe.top/gtjgixsomy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtkzsatnyd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtsblqlkym.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxuanxn.top/gtjunvsgka.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtpgxrlmjq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtzmnpzypa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shangyingyoupin.top/gtskbolstx.html

[L05] 上传文件（multipart）
来源：http://hz.iojbl.cn/gtkcwblmzg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gotoacloud.top/gtoawjqlsu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cqqwz.cn/gtiwouaowl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtneupkzgx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtxvxkidxt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtwhinelcd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ywan-chungtsiang.top/gtkarmcftx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtftbijuws.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.9152youxi.cn/gtudakqvjv.html

[L06] 解析响应为 JSON
来源：http://hz.316326.xyz/gtlyzhiwpn.html

Py:   resp.json()
来源：http://hz.hywenlv.cn/gtwfcbqakx.html

PHP:  json_decode($body, true);
来源：http://hz.hywenlv.cn/gtsnhvefgw.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtuhbngaxi.html

TS:   await resp.json()
来源：http://hz.redwolf501.top/gtrxrcvely.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtuoeigsto.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtmzkcculo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtsenozfko.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtognhutix.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtezzracve.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jiagoushi.top/gttliwrmkk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.kuanghao11.cn/gtccutselt.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtqpqusdwp.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtnjfczuxj.html

Java: resp.statusCode()
来源：http://hz.zhiwuduotai.top/gtnuvzbyct.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gtfhnctimw.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtverobskh.html

C#:   (int)resp.StatusCode
来源：http://hz.yueranfly.top/gtmkoddjaw.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtmbgdoiqw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.smart0.xyz/gtdxqwedpi.html

PHP:  curl_multi_init() 系列
来源：http://hz.gotoacloud.top/gtncpxkcir.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtcymlggkb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtogywkuep.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtanpsxygt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgufenzy.top/gtobksjaek.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtwruqpolk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.mhx1999.top/gtjdwlatik.html

================================================================================
来源：http://hz.guannengcc.top/gtnjuweyfa.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhongyouzk.top/gtsbrwnztb.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqldnkqpu.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtkgsnfird.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gtixulaeea.html

PHP:  $argv;  $argc;
来源：http://hz.ppjwa.cn/gtkbtchske.html

JS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtulcmtueu.html

TS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtmuhyejwo.html

Java: args 数组（main 方法参数）
来源：http://hz.yj202588.top/gtabomdksh.html

Go:   os.Args[1:]
来源：http://hz.xinyue.icu/gtwebiptkt.html

Ruby: ARGV
来源：http://hz.xuetiantiany.cn/gtnimnqlxu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gtyecztiwz.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtqbexjrzg.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtizwaggeu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtqyzveaph.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtedoflzig.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtxnluuzka.html

Java: System.getenv("HOME")
来源：http://hz.chenjidiqi.icu/gtrwrzqxmh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydjk.org.cn/gtnzqkolgv.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gthteawkjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinghuilouyu.cn/gtamypsade.html

[M03] 执行外部命令
来源：http://hz.yj202588.top/gtfjphldin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtnwrbwnoq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gtrzskaufj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtouiciuaa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gthvjrxnac.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cashguo.top/gtkqvxkhue.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gtduqjfmft.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guowangkeji.top/gtyfeydcxz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jyoumei.cn/gtknghghcz.html

[M04] 获取当前工作目录
来源：http://hz.cheryme.top/gtjitdzfcn.html

Py:   os.getcwd()
来源：http://hz.yvedp.cn/gtwdskzfou.html

PHP:  getcwd();
来源：http://hz.cdnleiting.top/gtndlnawjc.html

JS:   process.cwd()
来源：http://hz.316326.xyz/gtuxgswewr.html

TS:   process.cwd()
来源：http://hz.yj202588.top/gteixddhkk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtnfnhymih.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtaiwlpzlu.html

Ruby: Dir.pwd
来源：http://hz.sufxvd.cn/gtxsmvbuss.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zycfv.cn/gtyrgrsaru.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gtmoqgwkkh.html

Py:   sys.exit(1)
来源：http://hz.hfpthk.cn/gtxbzyzubx.html

PHP:  exit(1);
来源：http://hz.daxiang520.top/gtqgohbsxi.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtlmtgixnc.html

TS:   process.exit(1)
来源：http://hz.jiagoushi.top/gttjrrwsya.html

Java: System.exit(1)
来源：http://hz.kuanghao11.cn/gtvllkmfse.html

Go:   os.Exit(1)
来源：http://hz.316326.xyz/gtqgwuztwz.html

Ruby: exit 1
来源：http://hz.c1oappe.top/gtrnkziqsc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.vqdsnc.cn/gthlzxbipw.html

[M06] 向标准错误输出
来源：http://hz.ywan-chungtsiang.top/gtxjqoehgn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtewucvxjy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtvnmlzqtu.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gttdpvodsv.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtwmgtcxsc.html

Java: System.err.println("err")
来源：http://hz.feifeiyinyue.top/gtawifvhrl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gtjtijnvyx.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtcpykpdyn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gtrxugnmbz.html

[M07] 判断是否为主入口
来源：http://hz.zdqjudy.top/gtzgbrndqu.html

Py:   if __name__ == "__main__":
来源：http://hz.zhixingplan.top/gtqjrokyxg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.iojbl.cn/gtepoabscj.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtsvzflyke.html

TS:   require.main === module
来源：http://hz.yj202588.top/gtkbiyutir.html

Java: public static void main(String[] args)
来源：http://hz.aibaodan.cn/gtgukzsttf.html

Go:   func main()
来源：http://hz.kuanghao11.cn/gtjgxojtlz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtfakvqrpz.html

C#:   static void Main(string[] args)
来源：http://hz.xuanzx.com/gtnnpmgsry.html

[M08] 获取系统与运行时信息
来源：http://hz.zhaomingkeji.xyz/gtiucskinv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtrbalcnkg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gteiczbyya.html

JS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gtepsoyfkq.html

TS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gthxnbuuda.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gtuuizbfje.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xinyue.icu/gtzuupwclp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtaphuzidq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aibaodan.cn/gtqfjecmek.html

================================================================================
来源：http://hz.wangdashe.top/gtwcsndxoc.html

N. 数据结构与算法
来源：http://hz.xuanzx.com/gtxvntesyv.html

================================================================================
来源：http://hz.iojbl.cn/gtdwzbbmdb.html

[N01] 二分查找（有序数组）
来源：http://hz.redwolf501.top/gtbovybsyz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yonumen.top/gtqhvhwvfx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.iojbl.cn/gtywbaagtd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtfadffglw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtpbjmentj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yvedp.cn/gtvqytplnh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shangyingyoupin.top/gtrqcuwyfn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daria6918.cn/gtnhmuvewj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fzhhl.top/gtifjsvsqn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jlsjyb.cn/gtqbuxbarf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtibjheroy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.andypj.xyz/gtyiobgagf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtwpidgmiz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtejgcokqt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cucudq.cn/gtajblifsg.html

Go:   slices.Sort(arr)
来源：http://hz.gzhubu.top/gtjspuapis.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtobzhucsy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hysaishi.cn/gtawfonyep.html

[N03] 快速排序（分治示例）
来源：http://hz.wangdashe.top/gttolvkrlx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.dianchejie.cn/gtimjjgaio.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangshuangyany.cn/gtnaqzxdpr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtmrghwnqj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtwvkenbcu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangdashe.top/gtfibutwjy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gtwcshxsbz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hammf.cn/gtwgfwwlue.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yanxiufei.cn/gtkfixxvwh.html

[N04] 斐波那契数列
来源：http://hz.gotoacloud.top/gtnritqpla.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtbxaqlfke.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xziqi.cn/gtngcjenht.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtpeenbrte.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jiagoushi.top/gtivcfbrdl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtagwjzfmv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dianchejie.cn/gtxlplrgiu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gthidgqdsg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yanxiufei.cn/gtkngzebyu.html

[N05] 最大公约数
来源：http://hz.aizwys.cn/gtszjxhflb.html

Py:   math.gcd(a, b)
来源：http://hz.jlsjyb.cn/gtldaucuzc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.meibo888.top/gteffjglca.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtloscdcqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtdiqucveb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sxryk.cn/gtjlvlvulw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtwyibrshn.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gtatpytmpy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydzc1.top/gtflriicnr.html

[N06] 判断回文字符串
来源：http://hz.shzxlz.cn/gtlndmvfrv.html

Py:   s == s[::-1]
来源：http://hz.hammf.cn/gtztgmrqvs.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtztstnxgz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gthicsveds.html

TS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtmlknojgp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guannengcc.top/gtonzzfgwe.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtsoiqrfgp.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtcejtbpdb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtpoonyeje.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gtowojjiie.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shangyingyoupin.top/gtlvdrruoo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhixingplan.top/gtrnkkbiob.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.9152youxi.cn/gtwpknbsls.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuetiantiany.cn/gtbkbhgtzt.html

Java: // 手写 HashMap
来源：http://hz.zhaomingkeji.xyz/gtgphkolfv.html

Go:   // 手写 map[int]int
来源：http://hz.tianlin.xyz/gtfnfibbqq.html

Ruby: // 手写 Hash
来源：http://hz.gzhubu.top/gtctutslqf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtnzolehmp.html

[N08] 生成全排列
来源：http://hz.zhiwuduotai.top/gtwqkddfox.html

Py:   itertools.permutations(arr)
来源：http://hz.yuxming.cn/gtsnhquqkm.html

PHP:  // 手写递归交换
来源：http://hz.jianghu66.top/gtovktgxjj.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtsaovwehk.html

TS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtlgloncbx.html

Java: // 手写回溯递归
来源：http://hz.snrcjt.cn/gtcdombkta.html

Go:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtpwmuetyh.html

Ruby: arr.permutation.to_a
来源：http://hz.zhaomingkeji.xyz/gtbrpgvrdi.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtrxpvozgg.html

[N09] 栈与队列
来源：http://hz.zhijiandao.cn/gtrwlzbzil.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhaomingkeji.xyz/gtjqbcmmwh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhixingplan.top/gtqchoqjhl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtjxnrogcw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hysaishi.cn/gtvpbbvicw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xinyue.icu/gtobuduile.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnqzz.top/gtxfrvlxit.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gthkvpkdgz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cucudq.cn/gtkkdhihzz.html

[N10] 链表节点定义
来源：http://hz.nanxuanxn.top/gthtncfrjy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtkpizhxyp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxuanxn.top/gtyqiddpnb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.svipenyu.cn/gtvdzuqqcm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.svipenyu.cn/gtkshqejjw.html

Java: class Node { int v; Node next; }
来源：http://hz.tanke756.top/gtbmsgwaoq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinghuilouyu.cn/gtldzjhyhm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtovlppqqj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.c1oappe.top/gtdwuuyxdw.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258888.top/gttjfsglcz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj202588.top/gtojqbwgtk.html

PHP:  // 手写递归函数
来源：http://hz.nanxinkj.top/gtcoshgzce.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtnhbtsfbn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtazoqotst.html

Java: // 手写递归
来源：http://hz.52xcode.cn/gtkrhywlxs.html

Go:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtukqfpgzk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aizwys.cn/gtabfixaaf.html

C#:   // 手写递归
来源：http://hz.sxryk.cn/gtksxroxjb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhixingplan.top/gtjvnknylk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shzxlz.cn/gtyiiqtwig.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ivvv.top/gtiuqhpyqj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtjjyapkhp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtywbrwxwt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gteeqtffrr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtdmtqhtcd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtclwslqgn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtyehvqgvt.html

================================================================================
来源：http://hz.snrcjt.cn/gtptizffwr.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gtefzqdhmv.html

================================================================================
来源：http://hz.ybcxt.top/gtpsypbshm.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtyhyicavg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gtdvvmyyyy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xingfuxueyuan.xyz/gtzxfkgojz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgfzy.top/gtcweseirb.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtzsluuqqb.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgfzy.top/gttddvictr.html

Go:   go f()
来源：http://hz.feifeiyinyue.top/gtrxmwcjmk.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtkttnhhuo.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gtsbkqhfpm.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gtlwjnmnwl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.redwolf501.top/gtevnqxaif.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.vqdsnc.cn/gthrgptbyw.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtfqihczme.html

TS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtjkphdhcf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhiwuduotai.top/gtcwposfcn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gtrdtiowgk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj202588.top/gtbugybwnh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aibaodan.cn/gtgmcysktz.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtmkyoqjdv.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtbnkvtvhk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aizwys.cn/gtopbftbpv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gaohongyu789.top/gtmaknqoed.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtnyotbbub.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydjk.org.cn/gtfaegsnco.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangshuangyany.cn/gtdqsnpcwd.html


<!-- 参考信息 -->