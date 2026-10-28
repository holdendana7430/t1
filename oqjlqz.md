代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.ppjwa.cn/gtonpvtczm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtwosfnakr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtvzzufyji.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtvuzfnriz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtaydcticy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gzhubu.top/gtqebtyswd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtsdkzcptw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtoqchswix.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuxming.cn/gtvkqushky.html

[K07] 进制转换
来源：http://hz.dashuyun.cn/gtdtumjbbu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gtsngcrrhs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhiwuduotai.top/gtkypuokkj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtfecooclq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtutclytdt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtpmxjjcgw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuanzx.com/gtjitovkrt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtrxeqazpb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtbibuldqn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtncbmqjvh.html

Py:   pickle.dumps(obj)
来源：http://hz.ivvv.top/gtjuvhmkpa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jiagoushi.top/gtxxzreatv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gttdnogpxy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtsqaljtaw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gtvbmksxyx.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtgdaiueou.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gtrnneyfet.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hfpthk.cn/gtmasjqrkn.html

================================================================================
来源：http://hz.sysykeji.top/gtzehznryq.html

L. 网络请求
来源：http://hz.aibaodan.cn/gtnpohslvg.html

================================================================================
来源：http://hz.gotoacloud.top/gtgzglocgi.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtbhemigml.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.9152youxi.cn/gtmpbenuot.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtamvewraj.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtgrmgsjgj.html

TS:   await fetch(url)
来源：http://hz.daxiang520.top/gthzrlgttu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hongshengwenyu.top/gtmbzopwee.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gtciqdxzpd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangdashe.top/gtavmyryze.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtugzyyouz.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gtycuvyhih.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtyvkrawln.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhaomingkeji.xyz/gtpzqijixd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtsgqspgwu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtbjetzycm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtzvjmqbax.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuxming.cn/gtcuxykrvt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtgcfatkgq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtumkbiquq.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gttvyvixip.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gotoacloud.top/gtrmwubtsd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tianlin.xyz/gtrbdqabyc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtgdckzerm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtucfpkdre.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sweek.top/gtneorxlpu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtdpjiaudz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gogol.net.cn/gtervrvavn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj20258.top/gtluepagmb.html

[L04] 设置超时
来源：http://hz.shzxlz.cn/gtteyahrfp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tianlin.xyz/gtzhuwbwdz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.andypj.xyz/gtnslfoweb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtisckrxih.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtbjviklrv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtwdrtvrcq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ppjwa.cn/gtaiyuqcvn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sweek.top/gtcbfwxnfu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtwxwmhpwu.html

[L05] 上传文件（multipart）
来源：http://hz.mhx1999.top/gtpzwhdqgr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.feifeiyinyue.top/gtbbigpvis.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinghuilouyu.cn/gtxhptuuuk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtbbwlqbic.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtbagsqfrl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.0kj1m.cn/gtbwrwpgmf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigfzy.top/gtrqfmoxim.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtvzqpjfnz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jiagoushi.top/gtfggfkxcj.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtsiqhuqqj.html

Py:   resp.json()
来源：http://hz.cdnleiting.top/gtsfekaiah.html

PHP:  json_decode($body, true);
来源：http://hz.hnqzz.top/gtboapmmnr.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtvkixzqbg.html

TS:   await resp.json()
来源：http://hz.cashguo.top/gttktupjuf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtglorrupa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtuktahbek.html

Ruby: JSON.parse(resp.body)
来源：http://hz.havefunace.top/gtnifxqwoy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtvogklgrt.html

[L07] 处理 HTTP 状态码
来源：http://hz.fengsongda.top/gtizbqyycd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhixingplan.top/gtycgglexg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtlkyvetzt.html

JS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtyujjtlkq.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtifcnfigw.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtewdpslpu.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gticgexsqr.html

Ruby: resp.code.to_i
来源：http://hz.tian-w.cn/gtjaricuug.html

C#:   (int)resp.StatusCode
来源：http://hz.kuanghao11.cn/gteeigjcab.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtmbqbjbbm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guowangkeji.top/gtutxiquqx.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gttpnlxmqj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtiocgvuud.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtwzclnrsa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtvsmevqis.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtgzeidgjf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuetiantiany.cn/gtzmdrlzly.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jyoumei.cn/gtxxbxuvit.html

================================================================================
来源：http://hz.xziqi.cn/gtkxurxele.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtahcsjucm.html

================================================================================
来源：http://hz.zdqjudy.top/gttdrthrvl.html

[M01] 读取命令行参数
来源：http://hz.jinghuilouyu.cn/gtflxzympz.html

Py:   sys.argv[1:]
来源：http://hz.guannengcc.top/gtxroeowzg.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtjlmvtyzw.html

JS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtafztechn.html

TS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtumnmdexz.html

Java: args 数组（main 方法参数）
来源：http://hz.hnxiangtu.top/gtwkiekjwf.html

Go:   os.Args[1:]
来源：http://hz.nanxinkj.top/gtubgdfgzr.html

Ruby: ARGV
来源：http://hz.cashguo.top/gtdvsgvrei.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtinwplgwp.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtspzfqric.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtkphnbxck.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.vqdsnc.cn/gtpnpasdlg.html

JS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtbiuyrjdi.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtbrwpzfuq.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtargeanrv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtilddyolj.html

Ruby: ENV["HOME"]
来源：http://hz.sysykeji.top/gtsrrswost.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.smart0.xyz/gtfkknuaeb.html

[M03] 执行外部命令
来源：http://hz.guowangkeji.top/gtlofdhilr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtgyoqddre.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtrfvllqyw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtzigxyvvl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtltaqcskl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtxzrqzpbm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yangfankeji.com/gttmfkefvp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ivvv.top/gtnuzfvgtf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sxryk.cn/gtmvxvqdvt.html

[M04] 获取当前工作目录
来源：http://hz.yanxiufei.cn/gtrazebeta.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtstqhmemx.html

PHP:  getcwd();
来源：http://hz.shanyushiyangkeji.top/gtlhkkfwiy.html

JS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtytfypwkd.html

TS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtkjnoszxy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daria6918.cn/gttvoodwtn.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gtxusrpiqq.html

Ruby: Dir.pwd
来源：http://hz.yj20258.top/gtcuvfdmdy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.52xcode.cn/gtrrcpccph.html

[M05] 设置退出码
来源：http://hz.smart0.xyz/gthogzuwpm.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtmawjotlg.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gthigkllkz.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gttvwlkwed.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtwtnyipre.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtibtseunm.html

Go:   os.Exit(1)
来源：http://hz.haohaochexian.top/gtitchubcw.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtydjwymdh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yanxiufei.cn/gtunklhjhi.html

[M06] 向标准错误输出
来源：http://hz.nanxuanxn.top/gtgmprsuyl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cheryme.top/gtmhigcbgd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.52xcode.cn/gtzufshaei.html

JS:   console.error("err")
来源：http://hz.aizwys.cn/gtjwyvnkxm.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtqadnlbkn.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtuebevwhm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtyqjwqxuk.html

Ruby: warn "err"
来源：http://hz.shangyingyoupin.top/gtzfksrghf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zdqjudy.top/gtsysugtzm.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtuobfovpw.html

Py:   if __name__ == "__main__":
来源：http://hz.kuanghao11.cn/gtiknlkawl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtgxbbhbni.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtasexigbx.html

TS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtxabkzzhe.html

Java: public static void main(String[] args)
来源：http://hz.havefunace.top/gturckpimh.html

Go:   func main()
来源：http://hz.xylfe.cn/gtmosmqrza.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ybcxt.top/gttlttumpz.html

C#:   static void Main(string[] args)
来源：http://hz.chenlongwang.top/gtxrevroqp.html

[M08] 获取系统与运行时信息
来源：http://hz.yvedp.cn/gtbapwgxcg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtsmkreeyt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.52xcode.cn/gtfnepxovd.html

JS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gthhbiavuf.html

TS:   process.platform;  process.version
来源：http://hz.svipenyu.cn/gtjzxiqfgx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtqcliurza.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gtvgozsmxh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guannengcc.top/gtzfpfxttn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gzhubu.top/gtcxgtagkh.html

================================================================================
来源：http://hz.xylfe.cn/gtlnfcgrjh.html

N. 数据结构与算法
来源：http://hz.haohaochexian.top/gtupfvbgmd.html

================================================================================
来源：http://hz.dianchejie.cn/gtufxeidau.html

[N01] 二分查找（有序数组）
来源：http://hz.hfpthk.cn/gtzazebind.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258.top/gtdvrgrjpv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydzc1.top/gtkoimvckj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtssfwhumh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtqcnbztdn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ivvv.top/gtxgckwlpw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtrcfjzxmh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gtnrreqpih.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtqlbnzesf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xinyue.icu/gtwoxeyrqn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtmkswltoh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.birdmap.top/gtartfpapi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gteiyuogtt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtisfivzkn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gtxljtymmq.html

Go:   slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtrntbcpcl.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtnnoslkwb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.0kj1m.cn/gtqteymruu.html

[N03] 快速排序（分治示例）
来源：http://hz.hongshengwenyu.top/gtyfctxynd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cashguo.top/gtwdfgdsfn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.andypj.xyz/gtaaszpvuq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtmzfrxhgw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtkqybgjmy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zycfv.cn/gtvflyjvfr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtbstapocn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cqqwz.cn/gtfsbgjzsp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tanke756.top/gtdvdxzjxo.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangtech.top/gttlvmnitr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtcbswfneq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangshuangyany.cn/gtqlicuwyu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtwfbjtuxj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gthdwzuzbe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.iojbl.cn/gtmiogpaiv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtxkvrjufj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtvzeqtxqq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hywenlv.cn/gtiynwevnb.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtrzwvbwze.html

Py:   math.gcd(a, b)
来源：http://hz.yvedp.cn/gtqrrufxih.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yvedp.cn/gthzjzaudv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtsqiylzjf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtfcawdbhk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gthqlmpdgz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gtqwuywwpi.html

Ruby: a.gcd(b)
来源：http://hz.birdmap.top/gtlishmpoa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xingfuxueyuan.xyz/gtjcxiigov.html

[N06] 判断回文字符串
来源：http://hz.gaohongyu789.top/gtwlcbnepx.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtsoxmuxtu.html

PHP:  $s === strrev($s);
来源：http://hz.xziqi.cn/gtbuumqmpg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtlizrmedb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtdixgwhzy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daxiang520.top/gtqdpmjles.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gtsqwqpnrd.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtbcjkfvka.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtehasjnse.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtfpqpkngi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.iojbl.cn/gtounfcxxr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangshuangyany.cn/gtsytvayfr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtjygrculn.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangshuangyany.cn/gtniesrtoq.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtpmebbrko.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258888.top/gtlhjuebnx.html

Ruby: // 手写 Hash
来源：http://hz.hfpthk.cn/gtckbquvib.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigfzy.top/gtdwnrhibq.html

[N08] 生成全排列
来源：http://hz.xuetiantiany.cn/gtkenjybuz.html

Py:   itertools.permutations(arr)
来源：http://hz.zhongyouzk.top/gtrmfijoro.html

PHP:  // 手写递归交换
来源：http://hz.redwolf501.top/gtdnghusea.html

JS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtdppebadp.html

TS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtzwwlviqp.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtfzwzseoj.html

Go:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtfbxgbuaf.html

Ruby: arr.permutation.to_a
来源：http://hz.jqgfzy.top/gtzepxeguk.html

C#:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtxqbdrgwo.html

[N09] 栈与队列
来源：http://hz.redwolf501.top/gtpkcopwbv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ywan-chungtsiang.top/gtabsemfhb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.redwolf501.top/gtizkekmze.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigufen.top/gtvvfiqqwz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtnjrpxexg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hammf.cn/gtskvjyvxz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hywenlv.cn/gtrjbvsdsc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ybcxt.top/gtvpakyylg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258888.top/gtemypjxuf.html

[N10] 链表节点定义
来源：http://hz.smart0.xyz/gtssmtcleb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gtcvlknuqz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuanzx.com/gtmcxsnmgo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinghuilouyu.cn/gtpzjgrugv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jlsjyb.cn/gtzwpogxfj.html

Java: class Node { int v; Node next; }
来源：http://hz.zhixingplan.top/gtiqkodgbq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydzc1.top/gtrumjbiql.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fengsongda.top/gtfujimkmz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shzxlz.cn/gtgqxslhmn.html

[N11] 二叉树中序遍历
来源：http://hz.pengpengdd.cyou/gtsvntiqer.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj20258.top/gtxbywdfgk.html

PHP:  // 手写递归函数
来源：http://hz.ywan-chungtsiang.top/gtllmttbfb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtzozgkibv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtezapsgic.html

Java: // 手写递归
来源：http://hz.shanyushiyangtech.top/gtujfvlgvj.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtlopxgpar.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxinkj.top/gtzpinysrn.html

C#:   // 手写递归
来源：http://hz.gzhubu.top/gtpjziiioj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtlzsnxmog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gtjncxmvkw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aizwys.cn/gtcqhlvbii.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.andypj.xyz/gtnsjidwuk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtrrtbifgo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtydaiceds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnxiangtu.top/gtslszjrcp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenjidiqi.icu/gtdaypwjpd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtphpidqdj.html

================================================================================
来源：http://hz.zycfv.cn/gtasqbdyol.html

O. 并发与异步
来源：http://hz.jyoumei.cn/gtztrinfgz.html

================================================================================
来源：http://hz.jqgfzy.top/gtduhazsom.html

[O01] 启动一个线程
来源：http://hz.hysaishi.cn/gtrgqvsioc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtlcxkqocz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtansqyhvt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtjpqtfcer.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtuubzieva.html

Java: new Thread(() -> f()).start()
来源：http://hz.fzhhl.top/gtnyjunxxw.html

Go:   go f()
来源：http://hz.daxiang520.top/gtmtgzgtfl.html

Ruby: Thread.new { f }
来源：http://hz.vqdsnc.cn/gtpxbxjesd.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gtckgzgasc.html


<!-- 参考信息 -->