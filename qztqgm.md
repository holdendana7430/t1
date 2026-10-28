代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtspurcofh.html

[K07] 进制转换
来源：http://hz.smart0.xyz/gtonpfqwda.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.kuanghao11.cn/gtaxnulisz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gtynvzatoi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtbwbaehco.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtzbxkfycp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtfxeukyuh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fengsongda.top/gtikfyotii.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.9152youxi.cn/gtwvjfuqri.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.52xcode.cn/gtujlkcwau.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sxryk.cn/gtotbddtsd.html

Py:   pickle.dumps(obj)
来源：http://hz.jlsjyb.cn/gtsfjpimko.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258888.top/gtwomqghwy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtnfucysbm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtrbiaaoyg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gtylqcrmoa.html

Go:   encoding/gob
来源：http://hz.jianghu66.top/gtkkafpkcx.html

Ruby: Marshal.dump(obj)
来源：http://hz.yongpay.top/gtepanawjc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gtvirjuovy.html

================================================================================
来源：http://hz.ehwqpu.com/gtdbbghhfp.html

L. 网络请求
来源：http://hz.hongshengwenyu.top/gtvlrwokzp.html

================================================================================
来源：http://hz.guannengcc.top/gtpuxmcrkk.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtkzvuaywc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yvedp.cn/gtvzptwlxi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jiagoushi.top/gtxrjkzqru.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtmwdpylak.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtuekgwmwz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cqqwz.cn/gtkgcjuktb.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuxming.cn/gtqorgnhzq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtoehhjwhp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtscmknrla.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtpjibdrnx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cashguo.top/gtadxowbov.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gttjnrtjgx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtkrrdynhn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtwtvrdqsf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sufxvd.cn/gtbdtqeiuz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtxtiskyme.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhaomingkeji.xyz/gtkhyodiqw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtlqkwnefe.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gtujjttvfo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.birdmap.top/gttxazifaf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gtxdjgrjcp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtjeinaxdf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtikjwwtak.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yongpay.top/gttiumxeld.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtswgffosv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yonumen.top/gtoksnexpq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtubkmrrbv.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gtitqviauu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtvsikczqg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydjk.org.cn/gtkrgaavlv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtfpvcaoaz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtjqcipwvh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gttzbiszpn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jianghu66.top/gtnxegdogn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinyuanbaomall.cn/gtmrjflhig.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gtdnqotcqd.html

[L05] 上传文件（multipart）
来源：http://hz.gotoacloud.top/gtlgqitglr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtxozlrwsy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xylfe.cn/gtzscciiaj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtzkkswzee.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtakbngwim.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gtmvrnatnv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtnijxqhcq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guowangkeji.top/gtkvtrwdrr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.mhx1999.top/gtxtdydume.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtqcdbxicj.html

Py:   resp.json()
来源：http://hz.meibo888.top/gtrzogatpg.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtfdsrjzuh.html

JS:   await resp.json()
来源：http://hz.nwbrower.top/gtqyvalwtb.html

TS:   await resp.json()
来源：http://hz.jianghu66.top/gtkqkeqcbb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258.top/gtvgasbxrr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.iojbl.cn/gtaseiccix.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhiwuduotai.top/gttxrmfqgk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gaohongyu789.top/gtgzgepheb.html

[L07] 处理 HTTP 状态码
来源：http://hz.0kj1m.cn/gtjgfswfbc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtfzpolzbp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtdjyfdjwh.html

JS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtmxavlawt.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtnukxwonc.html

Java: resp.statusCode()
来源：http://hz.ivvv.top/gtvtadjfes.html

Go:   resp.StatusCode
来源：http://hz.hysaishi.cn/gtguwdwqxl.html

Ruby: resp.code.to_i
来源：http://hz.pycfn.com/gtrpprimko.html

C#:   (int)resp.StatusCode
来源：http://hz.hnqzz.top/gtkgsoftlt.html

[L08] 并发请求多个地址
来源：http://hz.jinqigfzy.top/gtwxrgmdhk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtostwgehz.html

PHP:  curl_multi_init() 系列
来源：http://hz.daxiang520.top/gtzfjierjt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtulntiusk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtemwrferh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangshuangyany.cn/gturaigiig.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.redwolf501.top/gtpstxszra.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtwlybrffd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtnaongfut.html

================================================================================
来源：http://hz.gotoacloud.top/gtihdpjyhw.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtomzwrdle.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgyvnhswh.html

[M01] 读取命令行参数
来源：http://hz.gogol.net.cn/gtrdmpfebp.html

Py:   sys.argv[1:]
来源：http://hz.tian-w.cn/gtzxetesri.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtzncfqfcq.html

JS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtsuzhfrtw.html

TS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtonxoxeat.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtdvbdduez.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtvpquoezw.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gthdwelssz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gttsquybuf.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtixjkghsb.html

Py:   os.environ.get("HOME")
来源：http://hz.tian-w.cn/gtupqayoql.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtpmntxlip.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtbicdreyo.html

TS:   process.env.HOME
来源：http://hz.nwbrower.top/gtlxntrxno.html

Java: System.getenv("HOME")
来源：http://hz.yuanzhike.top/gtjnkjqnfu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dashuyun.cn/gtwxvsfhht.html

Ruby: ENV["HOME"]
来源：http://hz.xuetiantiany.cn/gtzjnftlqm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fengsongda.top/gtrpbtyeiv.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtibuxttct.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nwbrower.top/gtjlpaygqi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sweek.top/gtcdclwaqc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtehayrjir.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtzsxzuchj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtbazcvpjf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yonumen.top/gtancfqxyg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dianchejie.cn/gtkikdhifx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258.top/gtjwjekjvu.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gtxpyitjvo.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtcdnqlkjg.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtzasybxek.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtdyzewvzm.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gttharupqp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.0kj1m.cn/gtbrbosyyq.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtwhasuxad.html

Ruby: Dir.pwd
来源：http://hz.gaohongyu789.top/gtmmgcwpcq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtwvmoptjp.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtmzzizyxs.html

Py:   sys.exit(1)
来源：http://hz.cqqwz.cn/gtmmongzmt.html

PHP:  exit(1);
来源：http://hz.shuidangran.top/gtgybkmvss.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtqsgznrcc.html

TS:   process.exit(1)
来源：http://hz.yvedp.cn/gtanrfuxkz.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtnqiolvai.html

Go:   os.Exit(1)
来源：http://hz.jlsjyb.cn/gtdggeyivg.html

Ruby: exit 1
来源：http://hz.nanxinkj.top/gtopawefmm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtjvppthnl.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtrkowqufx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtaefzqwuw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gtmxkzvkfa.html

JS:   console.error("err")
来源：http://hz.meibo888.top/gtkywcqmnl.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtrfxwstjj.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtlyoqkrvq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yueranfly.top/gtmdqzqmqh.html

Ruby: warn "err"
来源：http://hz.pengpengdd.cyou/gtgpbtfhap.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shuidangran.top/gtuwkyjwdp.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gtvsujyhcq.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxinkj.top/gtwirzotsu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtryawjxge.html

JS:   require.main === module
来源：http://hz.yj20258888.top/gtlgqbxlwg.html

TS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtzjegswoh.html

Java: public static void main(String[] args)
来源：http://hz.haohaochexian.top/gtehtdxmfa.html

Go:   func main()
来源：http://hz.mhx1999.top/gtbirdjehu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtktboupmi.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gtdyvyyvdk.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gtjqpvmjod.html

Py:   platform.system();  platform.python_version()
来源：http://hz.meibo888.top/gtjoyxcmql.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.0kj1m.cn/gthquayfse.html

JS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtzrjcekoy.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtvqcpilau.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtmcbpzxui.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gtdekvwjlo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenzaomai.com/gtpyqemaiv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sweek.top/gtncjyrwgq.html

================================================================================
来源：http://hz.hywenlv.cn/gtrfqdlmtd.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtmtdtdljg.html

================================================================================
来源：http://hz.cqqwz.cn/gtsnbbsgiu.html

[N01] 二分查找（有序数组）
来源：http://hz.shuidangran.top/gtcqssaoku.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fzhhl.top/gtdtvookea.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gtzthezkln.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtgeyjijpf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtrbalidtr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtzulornbf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtluasrhsp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhiwuduotai.top/gthpygzjru.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cucudq.cn/gttejtgcmt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhengqikj.top/gtxhjrwtmr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hongshengwenyu.top/gtnfoyxxzq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtmlpkfvlh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtdutjtafc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtsexhxxvq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yueranfly.top/gtriqnyzla.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtgcrjhwma.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtdfpminbm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.bjfxy.top/gtxrttxdoz.html

[N03] 快速排序（分治示例）
来源：http://hz.aibaodan.cn/gtigjgoqhb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnqzz.top/gtzcylvopf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gthevdwuff.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtrubqzimt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtqgnslurf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hongshengwenyu.top/gtxdcuhofq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zycfv.cn/gtkfgqhplk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtdylzhotr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cqqwz.cn/gtfntdtwxz.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gtqeyfpikj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtxpciosru.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dashuyun.cn/gthhnnqedn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtmbfsauiz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtlrosovzl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zycfv.cn/gtgwmjlgvj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aibaodan.cn/gtadkisoit.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtlgwoxpvp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sweek.top/gtpvnqmkxq.html

[N05] 最大公约数
来源：http://hz.hfpthk.cn/gtlkdyveik.html

Py:   math.gcd(a, b)
来源：http://hz.chenlongwang.top/gttvcckpre.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258.top/gttpnevhum.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtgikomodj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gteshfhusd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtngxalrzg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenjidiqi.icu/gtybchmnjp.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gttenlaqgh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtwldbdsrp.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gtejgieptc.html

Py:   s == s[::-1]
来源：http://hz.chenlongwang.top/gtpwreufnn.html

PHP:  $s === strrev($s);
来源：http://hz.yuanzhike.top/gtdsstwooa.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gteiwbeyct.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtfnqkfxth.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gaohongyu789.top/gtjqtshzcc.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtfeboanjg.html

Ruby: s == s.reverse
来源：http://hz.316326.xyz/gtspfdlldy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtmzrrsvab.html

[N07] 两数之和（返回下标）
来源：http://hz.yanxiufei.cn/gtotpzxojp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tianlin.xyz/gtnqpucrju.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dashuyun.cn/gtuuufgmpu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hysaishi.cn/gtksyjzupi.html

TS:   // 手写 Map<string, number>
来源：http://hz.ehwqpu.com/gteebskntl.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangkeji.top/gtgbfuqkiy.html

Go:   // 手写 map[int]int
来源：http://hz.shangyingyoupin.top/gtpmqgvxjj.html

Ruby: // 手写 Hash
来源：http://hz.xinyue.icu/gtdtrvyvlc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xingfuxueyuan.xyz/gtrinnhuug.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gthqozxtwc.html

Py:   itertools.permutations(arr)
来源：http://hz.nwbrower.top/gtjecovgvt.html

PHP:  // 手写递归交换
来源：http://hz.smart0.xyz/gtinfxuwic.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtuuqesxhx.html

TS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtsezjnows.html

Java: // 手写回溯递归
来源：http://hz.hnqzz.top/gtmhgjbrtz.html

Go:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtyefbhtej.html

Ruby: arr.permutation.to_a
来源：http://hz.wangdashe.top/gtggkqwszu.html

C#:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtfpxayyqh.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gthdqxbask.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtgjlxfnym.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydjk.org.cn/gtuzwsixte.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtxmrjshhq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.smart0.xyz/gtjyruafoi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gtshwadpcs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jlsjyb.cn/gtgpnlfhen.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtuzqfurmi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258.top/gtqoodjxiz.html

[N10] 链表节点定义
来源：http://hz.nanxuanxn.top/gtqtbwcbfl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenjidiqi.icu/gtwnoxdrda.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhengqikj.top/gtajzfplel.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtfwhothnr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ivvv.top/gtbqtvtrnz.html

Java: class Node { int v; Node next; }
来源：http://hz.hammf.cn/gtqcmvtykx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtukvlyldz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnqzz.top/gttjlgwzna.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258888.top/gtfavyyepl.html

[N11] 二叉树中序遍历
来源：http://hz.yj202588.top/gtkqvhbfxg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuxming.cn/gtfhivqqyj.html

PHP:  // 手写递归函数
来源：http://hz.xuetiantiany.cn/gtyteoryqj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtxfcfllah.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gtgzlcipjy.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtcisejazc.html

Go:   // 手写递归
来源：http://hz.cqqwz.cn/gtqcdhtdyl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtkoixcpad.html

C#:   // 手写递归
来源：http://hz.sufxvd.cn/gthnsndapm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yonumen.top/gtmsblfpcj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.bjfxy.top/gttmrnfozs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.kuanghao11.cn/gtuhqczrxi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gthncqwbmj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtbnnvbmzu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtcfjthmra.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xylfe.cn/gtsmicukyx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gaohongyu789.top/gtzurodbyk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtvbkxnrby.html

================================================================================
来源：http://hz.cashguo.top/gtusfhlhqm.html

O. 并发与异步
来源：http://hz.redwolf501.top/gtoccvzalf.html

================================================================================
来源：http://hz.mhx1999.top/gtshkkrjdq.html

[O01] 启动一个线程
来源：http://hz.wangdashe.top/gtmnvxmxrb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pengpengdd.cyou/gttfsgqdcf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ppjwa.cn/gtmfhntwyp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtpjiwpqdl.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtamkmnjnm.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gthmfxqrdk.html

Go:   go f()
来源：http://hz.xingfuxueyuan.xyz/gtwclxvzpn.html

Ruby: Thread.new { f }
来源：http://hz.c1oappe.top/gtacyatmma.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtbrzowgmd.html

[O02] 使用线程池
来源：http://hz.yongpay.top/gtiqxlkzaa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.snrcjt.cn/gtqhdxkzqo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtgxmeqjom.html

JS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtgynooyfo.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtnwmbagrv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sysykeji.top/gtkilbqcuy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhiwuduotai.top/gtehfrebec.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gtxovyfrtg.html


<!-- 参考信息 -->