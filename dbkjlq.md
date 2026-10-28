代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.svipenyu.cn/gtmfnzuvwb.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtbahlcwug.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtrdqhxdzf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gttqebclvx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtuirsbvrl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtgyvpcwlv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtcybecjut.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinyuanbaomall.cn/gtpduqxsdc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.iojbl.cn/gtbwlnyzmy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.kuanghao11.cn/gturfbnidg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhoulong.xyz/gtajxpvsdb.html

Py:   pickle.dumps(obj)
来源：http://hz.yangfankeji.com/gtdketrbgk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtbcummroj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtrgdwdseg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtooxxjual.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtvhwgumry.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtflxhpohe.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtsoytyqta.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yueranfly.top/gtsvrxrsgj.html

================================================================================
来源：http://hz.aibaodan.cn/gtefiskmvy.html

L. 网络请求
来源：http://hz.gaohongyu789.top/gtkvicwget.html

================================================================================
来源：http://hz.jyoumei.cn/gtfvvckncl.html

[L01] 发送 GET 请求
来源：http://hz.zycfv.cn/gtkmodxntx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yvedp.cn/gtvfjajywi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cqqwz.cn/gtnmjaslau.html

JS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtjvbipwlv.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtcjkddwab.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cqqwz.cn/gtgvfuneny.html

Go:   resp, err := http.Get(url)
来源：http://hz.tian-w.cn/gtwvgmjeeu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gtxievdoor.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.iojbl.cn/gtynawvdkr.html

[L02] 发送 POST JSON
来源：http://hz.cqqwz.cn/gtxojptagc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ivvv.top/gtyfrorxcy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gtnhirzzvc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtrkhjawlr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtjpgdsqqy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pycfn.com/gtcdmvktku.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtzjhlzyhd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pengpengdd.cyou/gthaywjbkw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yueranfly.top/gtarjvonqr.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtfshakzii.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuetiantiany.cn/gtxggoauto.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinyuanbaomall.cn/gtorsokwye.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gthnosocco.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtppwrafvp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangkeji.top/gtxxpgcizb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gthaaxzowr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gtoxgflzrc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtnfnwsqxs.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtqspficvo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.vqdsnc.cn/gtfvehllbp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guowangkeji.top/gtirdxzsgf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtqrzaogqb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtyqdeckxx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gotoacloud.top/gtbkpwwnpc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xylfe.cn/gtlyqgzrou.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenjidiqi.icu/gtyvsjjopq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cashguo.top/gtpeenxiog.html

[L05] 上传文件（multipart）
来源：http://hz.guannengcc.top/gtqrczvtqc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.52xcode.cn/gtiuaskpcg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shangyingyoupin.top/gtwlocsnis.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtcrgtipcv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtpnukregp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tianlin.xyz/gtepjaazqf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuanzx.com/gtxxosfwhb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sweek.top/gtohjshltz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gtbpsnebaw.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtttsnqjvx.html

Py:   resp.json()
来源：http://hz.yj20258.top/gtgrovlsww.html

PHP:  json_decode($body, true);
来源：http://hz.feifeiyinyue.top/gteolyysnu.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtilujvqmh.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtxifketpw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtfkoabhbh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtijmsbbvi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangtech.top/gtncujepjb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtbnobajgn.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtrnjkuycm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj202588.top/gthdhivkig.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtvmmefkfo.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtnworirhk.html

TS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtpkzzxfnz.html

Java: resp.statusCode()
来源：http://hz.feifeiyinyue.top/gthxoobogy.html

Go:   resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtlvpkclvp.html

Ruby: resp.code.to_i
来源：http://hz.nwbrower.top/gthchyvrdg.html

C#:   (int)resp.StatusCode
来源：http://hz.kuanghao11.cn/gtgpjchwwa.html

[L08] 并发请求多个地址
来源：http://hz.yj202588.top/gtbduateiu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtkedpymio.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtfwqkshmo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtbbaahunl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtqxlxjgfl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtohbdumvh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gtqjxucqjr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenjidiqi.icu/gtbpjrlpyy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtmmiuvftw.html

================================================================================
来源：http://hz.yuanzhike.top/gtwdxybxch.html

M. 命令行 / 进程 / 环境
来源：http://hz.daxiang520.top/gtthgwspqp.html

================================================================================
来源：http://hz.fengsongda.top/gttwapvzif.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gtkqfytdve.html

Py:   sys.argv[1:]
来源：http://hz.cucudq.cn/gtiwtdvisv.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtksktrmmr.html

JS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtsisdachw.html

TS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtopywlauk.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gtiixrhemf.html

Go:   os.Args[1:]
来源：http://hz.ydzc1.top/gtqklvhwbu.html

Ruby: ARGV
来源：http://hz.xziqi.cn/gtjcisjiht.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtlmumjipw.html

[M02] 读取环境变量
来源：http://hz.52xcode.cn/gttyrtetnq.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgfzy.top/gtdzrdtnhe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtvjqprjna.html

JS:   process.env.HOME
来源：http://hz.andypj.xyz/gtxqzrhssy.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtefiihfia.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gtgmigyowb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shuidangran.top/gtexkobqfb.html

Ruby: ENV["HOME"]
来源：http://hz.shzxlz.cn/gtrfjnxmbm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cashguo.top/gtxeucrlkh.html

[M03] 执行外部命令
来源：http://hz.jinqigfzy.top/gtvvofnjey.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dashuyun.cn/gtiamvoqhz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtdypklhdz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtlrwibdch.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtrfututiq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtuenbnofk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ybcxt.top/gtcssckgjj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtwqmfibxt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xziqi.cn/gtddfsrxao.html

[M04] 获取当前工作目录
来源：http://hz.smart0.xyz/gtnaohqbkb.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtcdvvsyrz.html

PHP:  getcwd();
来源：http://hz.aibaodan.cn/gtgspvoppt.html

JS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtopucgpgh.html

TS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtuqebkcqa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gaohongyu789.top/gtycykfucw.html

Go:   os.Getwd()
来源：http://hz.jinghuilouyu.cn/gtcpnacebc.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gthuoydmzi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pycfn.com/gtrpftqzxe.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtmiyvsuse.html

Py:   sys.exit(1)
来源：http://hz.svipenyu.cn/gtwusifiul.html

PHP:  exit(1);
来源：http://hz.birdmap.top/gtywdopsyu.html

JS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtbbedhqio.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtgdcfibdl.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gtahsrgqpj.html

Go:   os.Exit(1)
来源：http://hz.zhengqikj.top/gtmmepdnfc.html

Ruby: exit 1
来源：http://hz.tianlin.xyz/gtemhndqxb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ehwqpu.com/gtatujtpgh.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtbybcqilh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtrrchqoof.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hongshengwenyu.top/gtteklejak.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtnjlakikd.html

TS:   console.error("err")
来源：http://hz.iojbl.cn/gtspxvbvmb.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtsbogfxzu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gtppsbhfqo.html

Ruby: warn "err"
来源：http://hz.zhongyouzk.top/gtifpgsegm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtlrpjsgju.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtksyxbwtc.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtflyjuxaq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.meibo888.top/gtngnnvnuw.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtbnxxiyyd.html

TS:   require.main === module
来源：http://hz.jqgufenzy.top/gtmaywfwoc.html

Java: public static void main(String[] args)
来源：http://hz.mhx1999.top/gtlmepurmr.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtamurhnti.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangdashe.top/gtgsbdpxdz.html

C#:   static void Main(string[] args)
来源：http://hz.smart0.xyz/gtvimseehd.html

[M08] 获取系统与运行时信息
来源：http://hz.xuetiantiany.cn/gtjgjjvwqm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ppjwa.cn/gtxuhqvsoz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ehwqpu.com/gtysqsknzc.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtdazbhldl.html

TS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtjoczubbv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jianghu66.top/gtgibwdxum.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigufen.top/gthdtkrcvl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gogol.net.cn/gtrypubzmq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.52xcode.cn/gtahgqhbuq.html

================================================================================
来源：http://hz.snrcjt.cn/gtiilytdnn.html

N. 数据结构与算法
来源：http://hz.chenlongwang.top/gtclpequzx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttxazious.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtvwjhotmj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gtfakkrpbu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangshuangyany.cn/gtwvcvqfrg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtdwvosqwe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtiebupmgx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtiaqssrya.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cqqwz.cn/gtoqughjzm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigufen.top/gtwwydymcm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jianghu66.top/gtatedkvfy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtktxnujes.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtoowowtdp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtbcctzwnq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtxicnaoyi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtiwmlnjlp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yanxiufei.cn/gttvhofmjc.html

Go:   slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtplozwblg.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gttfczfljj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yangfankeji.com/gtnxaeyvzt.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtumrkyrcx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtkfpqfqet.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtnxurobdn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gttympaqkk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gtrwqejbmc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258.top/gtbtlunnlj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ybcxt.top/gtgdeyonsn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gthqfdivgo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.52xcode.cn/gtwsvcjjls.html

[N04] 斐波那契数列
来源：http://hz.c1oappe.top/gtdgtbambf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtslskclyf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.quarkkingdee.top/gtxhwgcyaj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtfiitiuus.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtxuvikxiz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gotoacloud.top/gtsfxigdmb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yanxiufei.cn/gtdglenjcs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtwheqhklf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtssyoqspp.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtwbwtmjtm.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtucnvdvha.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gttrabgouw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtjkqilzaw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtncfwubty.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gotoacloud.top/gtkeiikrem.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tianlin.xyz/gtgidgnkwg.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gtbedpooda.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tanke756.top/gtdqtkweaz.html

[N06] 判断回文字符串
来源：http://hz.zhongyouzk.top/gtllkgnnqy.html

Py:   s == s[::-1]
来源：http://hz.smart0.xyz/gtpaxxphrb.html

PHP:  $s === strrev($s);
来源：http://hz.pengpengdd.cyou/gtmqfpfjlj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtintdrtiw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtfwsenkwm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shuidangran.top/gtnljtkrhh.html

Go:   // 双指针从两端比较
来源：http://hz.gzhubu.top/gthlxbwyvz.html

Ruby: s == s.reverse
来源：http://hz.mhx1999.top/gtuajsqazy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gtdesinqty.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gthwymqmtp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yanxiufei.cn/gtjipwhtfy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ehwqpu.com/gtnynliary.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.52xcode.cn/gttgyfcint.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtajtsrrcu.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gturxfufha.html

Go:   // 手写 map[int]int
来源：http://hz.nanxinkj.top/gthbfgqoss.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtgjiiwlst.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tian-w.cn/gtbnpqydkp.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gtbxrebwvf.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtppoadahm.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtsisucmyt.html

JS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtoyfqvfho.html

TS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gttiojiqjk.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtsbqfsqqg.html

Go:   // 手写回溯递归
来源：http://hz.pycfn.com/gtogvtsaiw.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxuanxn.top/gtbadpimig.html

C#:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtkllegyqv.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gtmxuhcofh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.snrcjt.cn/gtvvfqgqum.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangdashe.top/gtqyflsgbg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtcodtaltn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.quarkkingdee.top/gtbezdtfrk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.smart0.xyz/gtryojvweb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cdnleiting.top/gtmzucytaj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtodyhlgme.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tanke756.top/gttavlfedo.html

[N10] 链表节点定义
来源：http://hz.sweek.top/gtuperdkfg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.feifeiyinyue.top/gtnycjjbgf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gtprxmtixa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tianlin.xyz/gtlgjtodmf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yuanzhike.top/gtlfmoxwet.html

Java: class Node { int v; Node next; }
来源：http://hz.ywan-chungtsiang.top/gtonxmopce.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gtugatecgl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pengpengdd.cyou/gtkgkapwyv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.snrcjt.cn/gtkfonfogs.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtfiztlkzo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shuidangran.top/gtetzoijcq.html

PHP:  // 手写递归函数
来源：http://hz.chenzaomai.com/gtgvkbocms.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtivjojznu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtbvydjgsg.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtomdcixkw.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtbmspdvlx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gtqqtdogtd.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gtgieodlbv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtiwqayzav.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.vqdsnc.cn/gtbkqccovp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gtxhcgrezx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtqwmzggyo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtknntdnas.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.kuanghao11.cn/gtdyczqqly.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuanzx.com/gtnhtsjapb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fengsongda.top/gtdnencnia.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtexxdvfcq.html

================================================================================
来源：http://hz.guowangkeji.top/gttszhwgwb.html

O. 并发与异步
来源：http://hz.sysykeji.top/gtzxlthgeu.html

================================================================================
来源：http://hz.redwolf501.top/gtpvhdutvo.html

[O01] 启动一个线程
来源：http://hz.zhoulong.xyz/gtnccfqvqe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtolbiaras.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxuanxn.top/gthaugwkpn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gtztqfibuk.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtsaahuevr.html

Java: new Thread(() -> f()).start()
来源：http://hz.guannengcc.top/gtazutosqy.html

Go:   go f()
来源：http://hz.hywenlv.cn/gtaoaqaoft.html

Ruby: Thread.new { f }
来源：http://hz.zhengqikj.top/gtysrhcmfh.html

C#:   Task.Run(() => F());
来源：http://hz.vqdsnc.cn/gtdpkbtrbf.html

[O02] 使用线程池
来源：http://hz.sweek.top/gtwxcyblcl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gtxtrwucpj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinyuanbaomall.cn/gtxofqrhrd.html

JS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gtbnikzplt.html

TS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtcyehznvd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.wangdashe.top/gtdvayetfp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.kuanghao11.cn/gtxjbxblro.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.quarkkingdee.top/gtwyyndzks.html


<!-- 参考信息 -->