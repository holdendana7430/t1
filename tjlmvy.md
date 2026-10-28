代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gtolpiolba.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtbrzxkqxc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xylfe.cn/gtfabzephq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fzhhl.top/gtazwcahff.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtxatlejsb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtvngfanyb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtcjxycgut.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shuidangran.top/gtxawmuafu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangtech.top/gtmcrvvyka.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtyaycihrp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gtfsitezms.html

Py:   pickle.dumps(obj)
来源：http://hz.bjfxy.top/gtdcwfydqm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgfzy.top/gtngpkglqr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtxamchmzc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtxjsuvqym.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hywenlv.cn/gtlfzifczv.html

Go:   encoding/gob
来源：http://hz.andypj.xyz/gtpiuiagwq.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gtzzajfezp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258.top/gtvcxzupgx.html

================================================================================
来源：http://hz.sxryk.cn/gtsxgrhrcj.html

L. 网络请求
来源：http://hz.zhoulong.xyz/gtcwlxwyea.html

================================================================================
来源：http://hz.guowangkeji.top/gtqbdrnzmd.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtnjwxjkxp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fengsongda.top/gtyaoxsloc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xylfe.cn/gttbjhehvd.html

JS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtckisdbaw.html

TS:   await fetch(url)
来源：http://hz.zhengqikj.top/gttabeftzg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.birdmap.top/gtrzbwcwda.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangtech.top/gtgrqdkbds.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangtech.top/gtrvzgkoob.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258.top/gtbrvpvmpr.html

[L02] 发送 POST JSON
来源：http://hz.52xcode.cn/gtjxmwexhy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ivvv.top/gtpzgfbzeq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtgtdsthhl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gticetnhpb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtvktwnqnc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hongshengwenyu.top/gtvhaiqbgh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xingfuxueyuan.xyz/gtiulhfmxp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.redwolf501.top/gtpnqdvfrt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtyoknhgti.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtnvirccgt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuxming.cn/gtmpokbngn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.52xcode.cn/gtxjzlklod.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gtsphnfkzo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gteyjhocec.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtuypupthb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ybcxt.top/gteoggddss.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jyoumei.cn/gthadhhhfw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gthwgrthwi.html

[L04] 设置超时
来源：http://hz.ybcxt.top/gtyzfppfqg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtsrcvwcfy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gotoacloud.top/gtyltsdzyd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtldldcldw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtikihrpfe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jianghu66.top/gtckjzsfxx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.c1oappe.top/gtkimbkphv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtldgwclgw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shuidangran.top/gtyyrlizac.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtnnatvvnc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtcoyepmfa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.havefunace.top/gtsvhtfgdw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtopquyumo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtcfbgmfec.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhengqikj.top/gtctubenxj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gttpbzybxn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtyidcqysg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtgqtbvcfz.html

[L06] 解析响应为 JSON
来源：http://hz.zycfv.cn/gtcrukdwov.html

Py:   resp.json()
来源：http://hz.0kj1m.cn/gtflzqxtkt.html

PHP:  json_decode($body, true);
来源：http://hz.ehwqpu.com/gtvqeqjcqy.html

JS:   await resp.json()
来源：http://hz.gzhubu.top/gtjkyqickl.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtumnxgfwd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zdqjudy.top/gtadncitwi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gogol.net.cn/gtnizwdote.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtwpocopeg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangdashe.top/gttqpwrqzq.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gtmlutjbqg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuxming.cn/gtwdqghcrb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.quarkkingdee.top/gtcrktbape.html

JS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtjicsqgdm.html

TS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtfwrqeacy.html

Java: resp.statusCode()
来源：http://hz.zhoulong.xyz/gtlnedweqv.html

Go:   resp.StatusCode
来源：http://hz.hnqzz.top/gtzxhldzfy.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gttdlagqxy.html

C#:   (int)resp.StatusCode
来源：http://hz.jiagoushi.top/gtzzlaxlha.html

[L08] 并发请求多个地址
来源：http://hz.yanxiufei.cn/gtzeyfvxob.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnxiangtu.top/gtkjoeooxg.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenjidiqi.icu/gtfpakruoo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtnntaczch.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtbrhhctls.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtmbcqwiqa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtuefudkxf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhoulong.xyz/gtnejzvzor.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenjidiqi.icu/gtllsydcsi.html

================================================================================
来源：http://hz.chenlongwang.top/gtnipynygs.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhengqikj.top/gtbheraoih.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbhpiegeu.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtejpydgsi.html

Py:   sys.argv[1:]
来源：http://hz.yonumen.top/gttpnkmpno.html

PHP:  $argv;  $argc;
来源：http://hz.pengpengdd.cyou/gtksurgfms.html

JS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gthoxsqoaz.html

TS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtjaowfdkj.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtnuahvceu.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtfxukfwhe.html

Ruby: ARGV
来源：http://hz.hfpthk.cn/gtcgodnfue.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigfzy.top/gtvdvyynqa.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gteplvvtds.html

Py:   os.environ.get("HOME")
来源：http://hz.iojbl.cn/gtqnvdcmsr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gthtcodixl.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtrtlbrzfc.html

TS:   process.env.HOME
来源：http://hz.cucudq.cn/gtqcmdqkai.html

Java: System.getenv("HOME")
来源：http://hz.zdqjudy.top/gtfqjptujo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtygaxlwzi.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtqzfbpyuj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ybcxt.top/gtngfaqbse.html

[M03] 执行外部命令
来源：http://hz.xuanzx.com/gtvseektuz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtpmfufyxq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtebasbfnq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtllqvicrn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gtjwqfxcti.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnqzz.top/gtzxcyfxkw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenzaomai.com/gtkrfjehus.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhoulong.xyz/gtwliqbwpb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhengqikj.top/gtndqhbeed.html

[M04] 获取当前工作目录
来源：http://hz.9152youxi.cn/gtoumbckaw.html

Py:   os.getcwd()
来源：http://hz.tian-w.cn/gtojhdcsdj.html

PHP:  getcwd();
来源：http://hz.hywenlv.cn/gtrnvenwkc.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtwilepymq.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtsrpvciaa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtuauyeukh.html

Go:   os.Getwd()
来源：http://hz.hammf.cn/gthseokmjj.html

Ruby: Dir.pwd
来源：http://hz.ivvv.top/gtgduivrrh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sysykeji.top/gtftaaueua.html

[M05] 设置退出码
来源：http://hz.andypj.xyz/gtjehaqkjw.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtxfzscozx.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtzsgokigo.html

JS:   process.exit(1)
来源：http://hz.xuanzx.com/gtyxseqnag.html

TS:   process.exit(1)
来源：http://hz.cashguo.top/gtofntnnev.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gtdrmvrmlw.html

Go:   os.Exit(1)
来源：http://hz.zycfv.cn/gtzggozikf.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtmghuldbu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.9152youxi.cn/gtfolzxcji.html

[M06] 向标准错误输出
来源：http://hz.guannengcc.top/gtrcsmxkoc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtbuwqijyi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tianlin.xyz/gtxhqxfdgi.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtuuqdbsxz.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gthokzlwzz.html

Java: System.err.println("err")
来源：http://hz.gzhubu.top/gtfkhnqhes.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtppmgjirj.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtpetbvpmi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.redwolf501.top/gtxshwpdlk.html

[M07] 判断是否为主入口
来源：http://hz.havefunace.top/gtibwvdeiq.html

Py:   if __name__ == "__main__":
来源：http://hz.aizwys.cn/gtdmlzrkjc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuetiantiany.cn/gtpemhzjfh.html

JS:   require.main === module
来源：http://hz.hysaishi.cn/gttrhqcqwm.html

TS:   require.main === module
来源：http://hz.redwolf501.top/gtvseohpez.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangtech.top/gtdtvwbwtq.html

Go:   func main()
来源：http://hz.jinqigufen.top/gtzpgujgva.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.316326.xyz/gtzzpoohed.html

C#:   static void Main(string[] args)
来源：http://hz.tian-w.cn/gtqboynegk.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gthfnlcrfo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtptpadtzh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtkffezjcx.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtnixwssjw.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtkawecwin.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xziqi.cn/gtcxsgfcca.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gteelrslyh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgfzy.top/gtzehvlwfg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jqgufenzy.top/gtuavdasit.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdrddttxu.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gtwpzdkyeh.html

================================================================================
来源：http://hz.birdmap.top/gtmmqhtzuk.html

[N01] 二分查找（有序数组）
来源：http://hz.ehwqpu.com/gtuescyzta.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gtwnqsqtfg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtfmuxqdln.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtfaqpneio.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtsqgqroie.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtryoxcqyq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtivojqlau.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.andypj.xyz/gtiziycjhu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sysykeji.top/gtxkoteahp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gttlwsbvlt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gtpfuqxvcv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtmilybbmn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtwgjyqgjj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtxxbhkjdk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigfzy.top/gthhmiqmkr.html

Go:   slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtqzccjgdq.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtdjglhyzg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shzxlz.cn/gtwlroggrg.html

[N03] 快速排序（分治示例）
来源：http://hz.ydzc1.top/gtnjjlqqnn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtrcdztwpq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sysykeji.top/gtxvtloxwi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtnskoashi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtqeqfqfmz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gtuwnslgaf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guannengcc.top/gtsokmdtiy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gtjbflyago.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhiwuduotai.top/gtmhvldrsi.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtjlppxvvg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gttgoyyxmg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtpitqzcru.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtwwnibank.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtrohifwib.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.kuanghao11.cn/gtkpekwyfd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.52xcode.cn/gtwthsnggr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtyrdfgwmo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jqgfzy.top/gtindkpbis.html

[N05] 最大公约数
来源：http://hz.jiagoushi.top/gtosrypgfm.html

Py:   math.gcd(a, b)
来源：http://hz.bjfxy.top/gtngqypcnm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.birdmap.top/gtfomqlbqx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtjqpaghat.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtsusmbkvl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zdqjudy.top/gthylsiube.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gtijnzdqlh.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtzwesclvs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtxbdyipnp.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtnadnyvon.html

Py:   s == s[::-1]
来源：http://hz.ydjk.org.cn/gtpemuemgl.html

PHP:  $s === strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtsgrqiiio.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtfasfffef.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtqdmislxn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tianlin.xyz/gtprtburoa.html

Go:   // 双指针从两端比较
来源：http://hz.nanxuanxn.top/gtfykecqdh.html

Ruby: s == s.reverse
来源：http://hz.redwolf501.top/gttbbtlbip.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtmnraiqcq.html

[N07] 两数之和（返回下标）
来源：http://hz.jinghuilouyu.cn/gtqryzhags.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sysykeji.top/gtwgcnybjo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258888.top/gtbxuaacac.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ivvv.top/gtjkxhdywe.html

TS:   // 手写 Map<string, number>
来源：http://hz.gzhubu.top/gthvmdkbmw.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtoprirmrd.html

Go:   // 手写 map[int]int
来源：http://hz.cucudq.cn/gtyeoqbshg.html

Ruby: // 手写 Hash
来源：http://hz.mhx1999.top/gtybrjpexw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hywenlv.cn/gtmflabqhr.html

[N08] 生成全排列
来源：http://hz.mhx1999.top/gtvejuzarp.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtlgithfmv.html

PHP:  // 手写递归交换
来源：http://hz.yuxming.cn/gtroerpizc.html

JS:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtsctbmucu.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtdsvvswyx.html

Java: // 手写回溯递归
来源：http://hz.sxryk.cn/gtnbuqmmwf.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtoencgkjs.html

Ruby: arr.permutation.to_a
来源：http://hz.yuxming.cn/gtjqcfaqnh.html

C#:   // 手写回溯递归
来源：http://hz.havefunace.top/gtfudhnpdx.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtbvbmzxbv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tianlin.xyz/gtndzcudrg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.quarkkingdee.top/gtzyndlsjf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.andypj.xyz/gtwwynbwhj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuanzx.com/gtqobibcta.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gttdsqkive.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtgkoxuhml.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pycfn.com/gtljdjojuc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pengpengdd.cyou/gtkhmknlcs.html

[N10] 链表节点定义
来源：http://hz.gaohongyu789.top/gtgwvclmfo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuxming.cn/gtuqcovjdn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ybcxt.top/gtyeipwnop.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtgeemdiqn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtluzujzbe.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigufen.top/gtmctyubdz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenlongwang.top/gtngeudnbf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guannengcc.top/gtbaaodowx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtotzfphpo.html

[N11] 二叉树中序遍历
来源：http://hz.sufxvd.cn/gtpfzdntgy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtatxwuwwo.html

PHP:  // 手写递归函数
来源：http://hz.birdmap.top/gtdzqogabp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gttnupkuga.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtofipgcgx.html

Java: // 手写递归
来源：http://hz.shuidangran.top/gteloepxnr.html

Go:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtiirqlfmo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.kuanghao11.cn/gtwrjxpjbg.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gtleghonyy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yueranfly.top/gtozvvhnuf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtynhopjzz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtauxsqptv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtiqlykrac.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fzhhl.top/gtwgdqrvyw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gtryyjuwzj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.birdmap.top/gtfwilnoln.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtnjmtshox.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtfsgyxwps.html

================================================================================
来源：http://hz.jqgufenzy.top/gtejsbeuxu.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtlnbbkvpq.html

================================================================================
来源：http://hz.wangdashe.top/gtukujpfuj.html

[O01] 启动一个线程
来源：http://hz.ydjk.org.cn/gtitcfgwir.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daxiang520.top/gtoddlhupn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cashguo.top/gtanadsljp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.9152youxi.cn/gtipvddcbb.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtrbljazen.html

Java: new Thread(() -> f()).start()
来源：http://hz.9152youxi.cn/gtuwyfpevu.html

Go:   go f()
来源：http://hz.guowangkeji.top/gthyeituuh.html

Ruby: Thread.new { f }
来源：http://hz.jlsjyb.cn/gtnwivcrlb.html

C#:   Task.Run(() => F());
来源：http://hz.dashuyun.cn/gtzylszomj.html

[O02] 使用线程池
来源：http://hz.yj20258888.top/gtygdwdxqi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shuidangran.top/gtkvfehvsk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.daxiang520.top/gtujwbtejo.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtejhgascn.html

TS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtmnyftftx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.smart0.xyz/gtwmfvtnru.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.quarkkingdee.top/gtmhdghgaw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jianghu66.top/gtstbxxfwx.html


<!-- 参考信息 -->