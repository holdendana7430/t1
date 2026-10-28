代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtqzmfptmi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gttnvyepew.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtxxezwnlz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtlufjinfk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtnxebjila.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ybcxt.top/gtkuuakzoj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtmxlvkpzj.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gtgjhxulwq.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenjidiqi.icu/gtfgiqvqmq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sweek.top/gtqncujqqz.html

JS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtabggjqbx.html

TS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtkpgipeta.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gttuttzcos.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtncnxtxvf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtpsywbzij.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigufen.top/gtqcpwwcft.html

[K06] 解析 URL 查询串
来源：http://hz.jqgfzy.top/gtfhejfjwz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jlsjyb.cn/gtfwaetvnu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.snrcjt.cn/gtxnjyezyu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtjnlxvner.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtcxfcmbvb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydzc1.top/gtrfqifnjl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtyrtfhkgb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gtzppapiby.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtdfiuwyeg.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtfddkqzyd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtwfefyjwj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhixingplan.top/gtjzbdzfky.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtedtqoyyk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtujkzdfmv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtgvdtjinf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258.top/gtbkgufxdw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtboalohlq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ybcxt.top/gtcwhtvkom.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtbbsxjqkp.html

Py:   pickle.dumps(obj)
来源：http://hz.hywenlv.cn/gthilqxvhz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtwdobahfh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtxgxopuwz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtavnavgld.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtilfusnfg.html

Go:   encoding/gob
来源：http://hz.ybcxt.top/gtqgkwhyow.html

Ruby: Marshal.dump(obj)
来源：http://hz.sweek.top/gtnzsjweme.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhiwuduotai.top/gtyevasdow.html

================================================================================
来源：http://hz.wangdashe.top/gtweuovsoi.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtnusslnke.html

================================================================================
来源：http://hz.ivvv.top/gtamkowcrr.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtckvbaqed.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jianghu66.top/gtwycvlfny.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtmtzuwyfz.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtfdlbvwzo.html

TS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtbvlojmlj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.mhx1999.top/gtosvejbcu.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtarlnkzcm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenzaomai.com/gtzdjcaddu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ybcxt.top/gtnyjjqgsn.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gtddsnfzoq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jlsjyb.cn/gtkklqlmqt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ivvv.top/gtvtandbal.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtfeovwmky.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtybfthynr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aibaodan.cn/gttybvfpwv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtsukbrwrm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ppjwa.cn/gtgyhhfcnb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangtech.top/gtdfpgudlm.html

[L03] 设置自定义请求头
来源：http://hz.chenlongwang.top/gtgnmpnkni.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.dashuyun.cn/gtmqiaoivg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtdknnbvpt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gttjaolpgr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtzqxaxtpk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gtpkvbveeu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.mhx1999.top/gtfpygxyil.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yongpay.top/gtfhyovzno.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuanzx.com/gtrabgtqne.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gttdqfhhom.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtpwunfmes.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtfvmzvcpg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtuzblihdu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtqwzypjlb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtgzddbwam.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinyuanbaomall.cn/gtadocbkfn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtdxfkdikb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtivzuizvs.html

[L05] 上传文件（multipart）
来源：http://hz.jianghu66.top/gtoydkuhwo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cheryme.top/gtfvoxufas.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtqspomshb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtbursxarb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtiaxjmlvb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guannengcc.top/gtpwfafhqk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhengqikj.top/gtfazmyqnw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtkorlpfuu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gtfooyiaaq.html

[L06] 解析响应为 JSON
来源：http://hz.chenzaomai.com/gtniwygdzw.html

Py:   resp.json()
来源：http://hz.snrcjt.cn/gtugcxpbau.html

PHP:  json_decode($body, true);
来源：http://hz.yj202588.top/gtbfjeqjra.html

JS:   await resp.json()
来源：http://hz.yonumen.top/gtlgeyqpeb.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gtuplgyypg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtilzqcawl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxinkj.top/gtzcxhuspj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtszjkiznm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jyoumei.cn/gtuoamoqhe.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtmbczmqsg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sweek.top/gtnfqqowpk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtheobefyg.html

JS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtsaztxwcq.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtadkwhwmy.html

Java: resp.statusCode()
来源：http://hz.cashguo.top/gtlcevlypn.html

Go:   resp.StatusCode
来源：http://hz.redwolf501.top/gtzgmkqmlq.html

Ruby: resp.code.to_i
来源：http://hz.wangshuangyany.cn/gtxmdezjlz.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtfqbwfxwv.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtlsayskmu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtmbqxhlqm.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gtmgazxjet.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtpvvklsgp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtduyebesr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtubrfgqnk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnqzz.top/gtzcsalxrw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hywenlv.cn/gtzhabmidu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hywenlv.cn/gtjfljvjxc.html

================================================================================
来源：http://hz.zycfv.cn/gtjdznflky.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtmwqbaapb.html

================================================================================
来源：http://hz.tianlin.xyz/gthnzasbkb.html

[M01] 读取命令行参数
来源：http://hz.gaohongyu789.top/gtcymiiplm.html

Py:   sys.argv[1:]
来源：http://hz.xingfuxueyuan.xyz/gtmjpepegm.html

PHP:  $argv;  $argc;
来源：http://hz.zhongyouzk.top/gtltorhrlm.html

JS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtnvvgcgqq.html

TS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtlffhjrpx.html

Java: args 数组（main 方法参数）
来源：http://hz.zhiwuduotai.top/gtrycqlrxs.html

Go:   os.Args[1:]
来源：http://hz.gotoacloud.top/gtwnwjwpwa.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gtkujoltli.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gtytmnezml.html

[M02] 读取环境变量
来源：http://hz.andypj.xyz/gtwwllokjb.html

Py:   os.environ.get("HOME")
来源：http://hz.yueranfly.top/gtlncnjxcp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zdqjudy.top/gtzzilxegj.html

JS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtfdlvrbxf.html

TS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtnyeiozfv.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gtqrlhtlay.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtkxkrqzpa.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtanroevsd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinghuilouyu.cn/gtqjsdrmxt.html

[M03] 执行外部命令
来源：http://hz.cucudq.cn/gttaeaybfb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhengqikj.top/gthzldfeiw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtdfdykblt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gttzzovzfc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gttuqliojt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gtuoacqxys.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sufxvd.cn/gtxbjkjwjk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtehdabhda.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hfpthk.cn/gtmqaveuku.html

[M04] 获取当前工作目录
来源：http://hz.shzxlz.cn/gtimzrwbtk.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtenufidaw.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gttssmutrj.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtzextuunt.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtubjmrrzh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtjwjewfkz.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtuupxuqjw.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtqobioinv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gaohongyu789.top/gtjsuhecjz.html

[M05] 设置退出码
来源：http://hz.jianghu66.top/gtaewjjizm.html

Py:   sys.exit(1)
来源：http://hz.chenjidiqi.icu/gtlwnygdvk.html

PHP:  exit(1);
来源：http://hz.zhiwuduotai.top/gtcikajocp.html

JS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtqmfhnbpr.html

TS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtohqwhthv.html

Java: System.exit(1)
来源：http://hz.sysykeji.top/gtedhkfbmw.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtrdzalkza.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtxokygwxh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhijiandao.cn/gtmbkfmksu.html

[M06] 向标准错误输出
来源：http://hz.yuxming.cn/gtepdimvmh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenjidiqi.icu/gtfwhkbcbf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gaohongyu789.top/gtmducmtzj.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtjcqptjro.html

TS:   console.error("err")
来源：http://hz.dashuyun.cn/gtceozruoc.html

Java: System.err.println("err")
来源：http://hz.quarkkingdee.top/gtjnuquplh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtcxzfwdnm.html

Ruby: warn "err"
来源：http://hz.cdnleiting.top/gthvejyjtz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zycfv.cn/gtdgcdfnki.html

[M07] 判断是否为主入口
来源：http://hz.gogol.net.cn/gtqcyqtcpj.html

Py:   if __name__ == "__main__":
来源：http://hz.jinghuilouyu.cn/gtbdidwtkh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xziqi.cn/gtoxhebpcq.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtnsxzdlcp.html

TS:   require.main === module
来源：http://hz.guannengcc.top/gtieakatbj.html

Java: public static void main(String[] args)
来源：http://hz.ivvv.top/gtybjxljxo.html

Go:   func main()
来源：http://hz.shanyushiyangtech.top/gtsxsyufzj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shzxlz.cn/gtesxhwhws.html

C#:   static void Main(string[] args)
来源：http://hz.gogol.net.cn/gtrrrzeopg.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gthfjlybxy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtnoamqikq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guowangkeji.top/gtwwjuzbiz.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtozwuyjmj.html

TS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtixdaurgb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtfrvhliyo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtwfavautw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtqvhocney.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtbcknrict.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtpumktcvu.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gtbhiiblbv.html

================================================================================
来源：http://hz.pycfn.com/gtmnlhesbx.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtdkjcbqnw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tianlin.xyz/gtfddfasha.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtmpeyvndj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtawfluomj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtkoagdhnt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtjkxqahlq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtkipvxapg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dashuyun.cn/gtxmutquth.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fengsongda.top/gtwytzhdes.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.feifeiyinyue.top/gtraujbapo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtdufmrbjm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtwrjlxagc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtsstezouc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtkwdhgixk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zdqjudy.top/gtwdevqqcm.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gttofhbadq.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtfqmrurux.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yueranfly.top/gtdecoegtu.html

[N03] 快速排序（分治示例）
来源：http://hz.zhongyouzk.top/gtqcvqmblu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtbjcmgnau.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtzlfffxgk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtferxzmbq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtfqmsgbuw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xylfe.cn/gtjwukooob.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yonumen.top/gtbqapvtuv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.quarkkingdee.top/gtzkwdplwa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtgylihptm.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtdidnoswr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtfglqofme.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jiagoushi.top/gtzzhyuwgb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtxnpcfwwn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtizcuulvh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj202588.top/gtqqafdhee.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydzc1.top/gtgefhbbph.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtprlgltsx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtnqubeugg.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtqbuamogj.html

Py:   math.gcd(a, b)
来源：http://hz.ydjk.org.cn/gtwbndloot.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtmxmkeabs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtuoxiwhtb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtrgtxzrrn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtzfjkngdq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.kuanghao11.cn/gtnxqthpuf.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtfbbjcoly.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dashuyun.cn/gtcctjlixj.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtafkedxjt.html

Py:   s == s[::-1]
来源：http://hz.bjfxy.top/gtoqkwidzb.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gtrfihpcow.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtwhxpyviz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtfiwzdodn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yvedp.cn/gtxslthxfe.html

Go:   // 双指针从两端比较
来源：http://hz.ehwqpu.com/gtlnadyfyk.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gtfazwragk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtkaundoqr.html

[N07] 两数之和（返回下标）
来源：http://hz.nanxuanxn.top/gtlltdeczw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jiagoushi.top/gtgegzpdqx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.316326.xyz/gtdrqnjrav.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shuidangran.top/gtrvnuxwnh.html

TS:   // 手写 Map<string, number>
来源：http://hz.ppjwa.cn/gtxsffsclh.html

Java: // 手写 HashMap
来源：http://hz.sxryk.cn/gtltjtpokd.html

Go:   // 手写 map[int]int
来源：http://hz.yuanzhike.top/gtskukhgnx.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtgwsxmqfq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xingfuxueyuan.xyz/gtpaotebdz.html

[N08] 生成全排列
来源：http://hz.316326.xyz/gtivpaqgum.html

Py:   itertools.permutations(arr)
来源：http://hz.xylfe.cn/gtdannicny.html

PHP:  // 手写递归交换
来源：http://hz.yuxming.cn/gtxjadkoau.html

JS:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtckjfvvbl.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtedrewimv.html

Java: // 手写回溯递归
来源：http://hz.chenzaomai.com/gtrrvuuwzu.html

Go:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtoizoxmzm.html

Ruby: arr.permutation.to_a
来源：http://hz.zhaomingkeji.xyz/gtnocordvr.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gtxpdwelge.html

[N09] 栈与队列
来源：http://hz.c1oappe.top/gtzvpznlcu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gotoacloud.top/gthydomdoc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.9152youxi.cn/gtzbflwbav.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daria6918.cn/gtgfdrecpx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yanxiufei.cn/gtprfrtngd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnxiangtu.top/gthvkkwfmv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.quarkkingdee.top/gtmgovjuvu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nwbrower.top/gtzqmnyvku.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.redwolf501.top/gtywmgnrzt.html

[N10] 链表节点定义
来源：http://hz.hnxiangtu.top/gttszxzkgp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gtwnktkvpe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtwruacdrg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtgqasacmj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangdashe.top/gtgwgzqbni.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gtrrsugiit.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangtech.top/gtfvtdwymp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangdashe.top/gtsnvawqgg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tian-w.cn/gtussuxwoq.html

[N11] 二叉树中序遍历
来源：http://hz.jqgufenzy.top/gtkfxfflyo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yvedp.cn/gtumqvpvdm.html

PHP:  // 手写递归函数
来源：http://hz.pycfn.com/gtwrajxwgk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtjbmzabkh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtpwrusird.html

Java: // 手写递归
来源：http://hz.svipenyu.cn/gtunhhfjwt.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtasudyenr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guannengcc.top/gtgnntnnfn.html

C#:   // 手写递归
来源：http://hz.xinyue.icu/gtkffsrlle.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtkmcgtbnx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhoulong.xyz/gtlwgvqlvj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xylfe.cn/gtmevqxgre.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtiayizxyk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtusciolys.html


<!-- 参考信息 -->