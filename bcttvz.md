代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gtauanlsnu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtdankghbo.html

[K04] 读取 JSON 文件
来源：http://hz.quarkkingdee.top/gtvjpcvqhj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xziqi.cn/gthpxekxgb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtsvzrpsll.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtyjsaitfo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtcjtlbhik.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj202588.top/gtplvqezpb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtalvnoiyb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daxiang520.top/gtfhundwdp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuanzx.com/gtcukfivre.html

[K05] 深拷贝对象
来源：http://hz.hongshengwenyu.top/gtipuvmjrs.html

Py:   copy.deepcopy(obj)
来源：http://hz.hammf.cn/gtngiikdqe.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gttupfkdnd.html

JS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gtrnvgcdig.html

TS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtdyhgmckh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuxming.cn/gtrqgadkbg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtziolpvde.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinyuanbaomall.cn/gthxbtpeuy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daria6918.cn/gtundtzqau.html

[K06] 解析 URL 查询串
来源：http://hz.zhijiandao.cn/gtgoifyvqh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtxjrvtqgz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtrqkjifdu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtxdaaymuf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtpblizlha.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtdnwupqwt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zycfv.cn/gtcydxpyqf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hysaishi.cn/gtypeddtzu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtrjhthupp.html

[K07] 进制转换
来源：http://hz.yvedp.cn/gtuzezixuv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtnxjxkwtz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yonumen.top/gtoxoyycrw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtggfxrvyz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtykvcguwa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gthaesfkfb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhijiandao.cn/gttdomwjem.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtcgtezrhw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tian-w.cn/gtidylawhm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtmqczhckq.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtnqimjewn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtakioaoro.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtrrmkzqpj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtikgvyldd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hongshengwenyu.top/gtefoofzoh.html

Go:   encoding/gob
来源：http://hz.hongshengwenyu.top/gtssaaafdp.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtpqtiuwfo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hammf.cn/gtqsemyvrp.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbdehdglv.html

L. 网络请求
来源：http://hz.zhijiandao.cn/gtipzgpgjr.html

================================================================================
来源：http://hz.guowangkeji.top/gtadnyzyuh.html

[L01] 发送 GET 请求
来源：http://hz.gaohongyu789.top/gtdsupqcnj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gtnjqutrvs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtctntjstr.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtdnknsifz.html

TS:   await fetch(url)
来源：http://hz.cheryme.top/gtalonahgm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuxming.cn/gtuxcgztyy.html

Go:   resp, err := http.Get(url)
来源：http://hz.sufxvd.cn/gtueosdnrf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.52xcode.cn/gtkrrmcxby.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangtech.top/gtnklykgyt.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gtxrxyefer.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtawacindu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gogol.net.cn/gtjxkwkbpz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtsqifvkzi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtghttcymq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtgndjbncu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gtrgwznyfu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.andypj.xyz/gthioyqhgj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtafedhfez.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gtyktmyuhk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtyxorsjuf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hammf.cn/gtougkktbn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtfemgcwtl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtkhttkirk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zdqjudy.top/gtqescupfu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yueranfly.top/gtxobwsdgz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtpnaxhtaq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtthhuthnu.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtgyqwuviv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.guannengcc.top/gtyrcfocdm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.feifeiyinyue.top/gtdbathxfj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtcjmbatuw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtijdfgram.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tianlin.xyz/gtuifqpcmx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuanzx.com/gtbeknllac.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dianchejie.cn/gtetgvnint.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtsxkvaoxa.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtqubvxekj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xingfuxueyuan.xyz/gtcuujeofc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtdkqwbcef.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtwqycciwr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtueoecdab.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgufenzy.top/gtanplemvg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.snrcjt.cn/gtpbiqogwa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtkzticyzq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuxming.cn/gtrlungkqu.html

[L06] 解析响应为 JSON
来源：http://hz.zhaomingkeji.xyz/gtinghyyhi.html

Py:   resp.json()
来源：http://hz.kuanghao11.cn/gtascssmls.html

PHP:  json_decode($body, true);
来源：http://hz.chenjidiqi.icu/gtbapkmsfm.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtvnxabtaj.html

TS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtolkgqguy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fzhhl.top/gtnnrngyui.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxinkj.top/gtyuekjodr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gtonadwysp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtgocrglyt.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtcutxonpr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtrvvmkqbj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.snrcjt.cn/gtbidbywbx.html

JS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtaecdgyst.html

TS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtyrjsqoul.html

Java: resp.statusCode()
来源：http://hz.jiagoushi.top/gtupttrijr.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gteuupjcso.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtjjawwybf.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtakzjqbmt.html

[L08] 并发请求多个地址
来源：http://hz.guowangkeji.top/gtmfgpnmup.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hongshengwenyu.top/gtcpkkwefn.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtupdxewnl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtuzkcuvqf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtmfpaowux.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtndwgxjfy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtfzdacghi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yangfankeji.com/gtgazzywax.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pycfn.com/gtsubocdtq.html

================================================================================
来源：http://hz.sufxvd.cn/gtkfbvbjvj.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtnposhkja.html

================================================================================
来源：http://hz.hammf.cn/gtinstgpnt.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtkjahmlpk.html

Py:   sys.argv[1:]
来源：http://hz.jinghuilouyu.cn/gthazqoirl.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gtgraryqpx.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtxirphdsg.html

TS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtcsamtvdp.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtjleifkzs.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gthyclbcsl.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gtkhigakkg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dianchejie.cn/gtpitueqbm.html

[M02] 读取环境变量
来源：http://hz.yvedp.cn/gthqgklnjf.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtitgrzbmy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.redwolf501.top/gtzfelfzvy.html

JS:   process.env.HOME
来源：http://hz.cucudq.cn/gtlguwenzq.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtegtxaeld.html

Java: System.getenv("HOME")
来源：http://hz.dianchejie.cn/gteloikmht.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnqzz.top/gtlgzxfhbh.html

Ruby: ENV["HOME"]
来源：http://hz.cashguo.top/gtblqzbwgu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigufen.top/gtbsyucnsb.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtdjyfzhfo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtgbytrhit.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gaohongyu789.top/gtdsjnlqdc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gthuqdzwtw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtqgiutstt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtnupfzpov.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtfviyubur.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.52xcode.cn/gtgtdkucqy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtclnujvdi.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gtekutltmb.html

Py:   os.getcwd()
来源：http://hz.zhijiandao.cn/gtrqpbnvtc.html

PHP:  getcwd();
来源：http://hz.xinyue.icu/gtnapreaot.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtdknviaib.html

TS:   process.cwd()
来源：http://hz.redwolf501.top/gtwxoxqqhp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hywenlv.cn/gtbgtejbet.html

Go:   os.Getwd()
来源：http://hz.hammf.cn/gtayxogtod.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gttkupdxie.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhiwuduotai.top/gtvqwoldgm.html

[M05] 设置退出码
来源：http://hz.xinyue.icu/gtppaluduy.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gtflizoslu.html

PHP:  exit(1);
来源：http://hz.gotoacloud.top/gtbfzipcsz.html

JS:   process.exit(1)
来源：http://hz.dianchejie.cn/gtwkkhxjze.html

TS:   process.exit(1)
来源：http://hz.wangdashe.top/gtunhwkgqy.html

Java: System.exit(1)
来源：http://hz.yueranfly.top/gtilfbeyqx.html

Go:   os.Exit(1)
来源：http://hz.yueranfly.top/gtjjswuufg.html

Ruby: exit 1
来源：http://hz.birdmap.top/gtyetzfewi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gogol.net.cn/gtkvjamlgu.html

[M06] 向标准错误输出
来源：http://hz.cashguo.top/gtnaevhjpl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtejgflpwh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.haohaochexian.top/gtmcjhuyec.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtnamsubek.html

TS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtmwfiyjba.html

Java: System.err.println("err")
来源：http://hz.aibaodan.cn/gtthygifru.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtceefvxnj.html

Ruby: warn "err"
来源：http://hz.ppjwa.cn/gttlczuktb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sysykeji.top/gtlyqegpxm.html

[M07] 判断是否为主入口
来源：http://hz.yueranfly.top/gtiqctszjr.html

Py:   if __name__ == "__main__":
来源：http://hz.zhiwuduotai.top/gtxrtfqcox.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gtwibktsxm.html

JS:   require.main === module
来源：http://hz.chenlongwang.top/gtemiwbnef.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtftuigenl.html

Java: public static void main(String[] args)
来源：http://hz.svipenyu.cn/gtnxcxdtrk.html

Go:   func main()
来源：http://hz.shuidangran.top/gtdjfxgvdo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtdrbcubwy.html

C#:   static void Main(string[] args)
来源：http://hz.chenjidiqi.icu/gtktngjnrx.html

[M08] 获取系统与运行时信息
来源：http://hz.52xcode.cn/gtqzkytzkv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtdxgirmqz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jlsjyb.cn/gtjbogqukw.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtmutfzegt.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtddcldljt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hywenlv.cn/gttbyhczsj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ppjwa.cn/gtfhlcqqrg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtvevcqqjf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhaomingkeji.xyz/gtascslhpj.html

================================================================================
来源：http://hz.hysaishi.cn/gthwwyfcts.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gtscuoyitu.html

================================================================================
来源：http://hz.havefunace.top/gtesavdfmc.html

[N01] 二分查找（有序数组）
来源：http://hz.jiagoushi.top/gtiklafcpz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.9152youxi.cn/gtoyrpzadl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtwsndctkn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtbizaquab.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gthbrbvchl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtbtgtvulk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtjelxvezc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.iojbl.cn/gtmtynssnv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.andypj.xyz/gtofzrmwit.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtixkbnzey.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtwzphtmkq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ybcxt.top/gtyeaipnjs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtcaefbrsl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtfpakcvhq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtdefimhgy.html

Go:   slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtoksynmxb.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtgevdjrrq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.9152youxi.cn/gtzfsdetse.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtqnohihbw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gttnknjkzq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtzapzpoxm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gthhyfdewh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtqezyrkas.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cashguo.top/gtwmnjsyan.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hfpthk.cn/gtprfghmaz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gtcdqcnwhf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yueranfly.top/gthlpsfybm.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtkeieqzzl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtftdtcpqd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gtpsobskwh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtbuolzmzy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtckbljqnr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtindacpbl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtqwqoinwe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtmcszbcgf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sysykeji.top/gtqxkugaqr.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtuikowutd.html

Py:   math.gcd(a, b)
来源：http://hz.zhiwuduotai.top/gtezjhihce.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.9152youxi.cn/gtphfherhy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtjnmzcisw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtfedmetya.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtvkowodna.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gtgglorfzv.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gtoxdcxxrs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cheryme.top/gtpigobwze.html

[N06] 判断回文字符串
来源：http://hz.chenzaomai.com/gtpedwsmqo.html

Py:   s == s[::-1]
来源：http://hz.aizwys.cn/gtnxnzmrvu.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtmsnldzwd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtljtvpibh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtpidekofq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.vqdsnc.cn/gtqymzysxm.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtwxecxzvy.html

Ruby: s == s.reverse
来源：http://hz.wangshuangyany.cn/gttaerzigl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtierdxtkg.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtasktofrr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuanzhike.top/gtxvjugzil.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dianchejie.cn/gtzndsqsnq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xinyue.icu/gtmjbrrerz.html

TS:   // 手写 Map<string, number>
来源：http://hz.cdnleiting.top/gtteygjljp.html

Java: // 手写 HashMap
来源：http://hz.fengsongda.top/gtlizinfil.html

Go:   // 手写 map[int]int
来源：http://hz.iojbl.cn/gtxcmcpwem.html

Ruby: // 手写 Hash
来源：http://hz.xingfuxueyuan.xyz/gtzsaqanaa.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shzxlz.cn/gtpijhgoia.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtsbacqsoq.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtvrvmlmxt.html

PHP:  // 手写递归交换
来源：http://hz.c1oappe.top/gtidfnovvz.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtygrwvzie.html

TS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtjsmflnxr.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtmmjfgjow.html

Go:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtyplveuiv.html

Ruby: arr.permutation.to_a
来源：http://hz.daria6918.cn/gtllwgfekv.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtvibrbuuh.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtqnzuzhde.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtgkhurnnr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gtkobipzgg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.316326.xyz/gtxqjbchkt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ivvv.top/gtdzbiljxa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gtozminczc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtnmxufkqn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gtfensueoe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhoulong.xyz/gtoeuuovxq.html

[N10] 链表节点定义
来源：http://hz.tianlin.xyz/gtrwlnfonx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtjybfpgoh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gturiuqsit.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgfzy.top/gtpbdgohxe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xingfuxueyuan.xyz/gtmowzwjyb.html

Java: class Node { int v; Node next; }
来源：http://hz.sufxvd.cn/gtewhiddxk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cashguo.top/gthszqtbdn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nwbrower.top/gttakljqbe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gtapsubach.html

[N11] 二叉树中序遍历
来源：http://hz.jianghu66.top/gtjvdrcidt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gotoacloud.top/gtjoxfoius.html

PHP:  // 手写递归函数
来源：http://hz.9152youxi.cn/gtshhlwybp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtdycoztod.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtxievzbjs.html

Java: // 手写递归
来源：http://hz.zhiwuduotai.top/gtimymypvl.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtoqcdofrj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hongshengwenyu.top/gtwgbqzmye.html

C#:   // 手写递归
来源：http://hz.hfpthk.cn/gtdbzcdsmv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sufxvd.cn/gtgtdyhlin.html


<!-- 参考信息 -->