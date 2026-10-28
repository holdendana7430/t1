代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hfpthk.cn/gtkvlzujyp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtzflxwyjj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtcsjhqkwb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cashguo.top/gtpdfbiuyq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gtlyfhxbvm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gzhubu.top/gtmbvvcvvf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shangyingyoupin.top/gtqcrzjfck.html

[K05] 深拷贝对象
来源：http://hz.zhengqikj.top/gtdwxrnzcd.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtmpvheohk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cheryme.top/gtxjdynxmb.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtbcelzzhm.html

TS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtavbleohg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yanxiufei.cn/gtlsoifqwo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pycfn.com/gtmiwjohnt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jlsjyb.cn/gtdstywllt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhaomingkeji.xyz/gtcotyurbt.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtrpynhwpp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gttmhlisss.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tianlin.xyz/gtmmnovffs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gttipxkqke.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtbspphxfq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yanxiufei.cn/gtqslbcyrm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cqqwz.cn/gtjzcnsqjs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cqqwz.cn/gtmvypqqjn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhengqikj.top/gtbsahhifq.html

[K07] 进制转换
来源：http://hz.ywan-chungtsiang.top/gtscwelmjp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.kuanghao11.cn/gtofldeaaw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cheryme.top/gtikxdylez.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtpnhfpgaa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtgeejyugv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtpsrwghsp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtfexaaqbq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtodjktdkm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydjk.org.cn/gtvbtbpahs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhiwuduotai.top/gttexqhghm.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtedjdiowo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtdyvddllh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtqfqvfxgv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtwmwkdxcc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sufxvd.cn/gtdrpkvncl.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtzuprvljd.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtjdtlvwov.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtohapqtfm.html

================================================================================
来源：http://hz.yj202588.top/gtudcwdulm.html

L. 网络请求
来源：http://hz.fengsongda.top/gttudftghn.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsonqjjew.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gttwsgbjdp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.birdmap.top/gtkobptckx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtqbhdhhfa.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtinowowwa.html

TS:   await fetch(url)
来源：http://hz.sxryk.cn/gtaglhciqx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zycfv.cn/gtatioqorr.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gtlzzyuhxn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gtusikvjpt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pengpengdd.cyou/gtpulaemse.html

[L02] 发送 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtvtvmwiyg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cdnleiting.top/gtdpkwnxrk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtpvyjnfti.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtqciapjlp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jianghu66.top/gtwtrjbuox.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tianlin.xyz/gtvntjolmo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.meibo888.top/gtykzihygp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jiagoushi.top/gtisouzecu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhiwuduotai.top/gttawkjdbv.html

[L03] 设置自定义请求头
来源：http://hz.zhaomingkeji.xyz/gtxpxlajeb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aibaodan.cn/gtiwdwgbso.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtvlmcauei.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtjpomzpri.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtitgekxpj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtmvxbkheq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtvlwilfqg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jlsjyb.cn/gttqzorpgi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtnxyknwdn.html

[L04] 设置超时
来源：http://hz.ydjk.org.cn/gtvrxiqarf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtgkgeczbr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ehwqpu.com/gtxvhqqrga.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtgxstyqry.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtoczmfssp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtgzmcjylp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xinyue.icu/gtgzeclpsc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gtfeaqnxwe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.meibo888.top/gtcljryopb.html

[L05] 上传文件（multipart）
来源：http://hz.sxryk.cn/gtyakhynsh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhijiandao.cn/gtikvbmauc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gttalinzjy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtobqqhkwm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gthsobjezo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cashguo.top/gticyagkuz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hfpthk.cn/gttuoptmcg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.c1oappe.top/gtkmtyiegq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gotoacloud.top/gtootjtvqi.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtkgskwjqg.html

Py:   resp.json()
来源：http://hz.vqdsnc.cn/gtjiflqkuw.html

PHP:  json_decode($body, true);
来源：http://hz.ybcxt.top/gtcqqgfodk.html

JS:   await resp.json()
来源：http://hz.aizwys.cn/gtqmizdttv.html

TS:   await resp.json()
来源：http://hz.nanxuanxn.top/gtqaukycgw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuanzx.com/gtocihbhdt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtmbwimrqb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sysykeji.top/gtwzsmxgga.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cheryme.top/gtntwranoh.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtiwsyswxz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtticxjxnm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtaoxrxlav.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtkyauojtt.html

TS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtnllkvcwk.html

Java: resp.statusCode()
来源：http://hz.meibo888.top/gtgeikcyxb.html

Go:   resp.StatusCode
来源：http://hz.yj20258.top/gtybropomm.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtrtcodgpl.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gtqjmqlxds.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtkmrvefwo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydzc1.top/gtxynorfzb.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinghuilouyu.cn/gtsnuvcqbc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtmgjezvkw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtrakdnvyi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnqzz.top/gttlstbbgb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cucudq.cn/gtklaxjxee.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ppjwa.cn/gtetzkagbg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gotoacloud.top/gtwrhynyax.html

================================================================================
来源：http://hz.pycfn.com/gtynpfcgoz.html

M. 命令行 / 进程 / 环境
来源：http://hz.gaohongyu789.top/gtgfiglxyu.html

================================================================================
来源：http://hz.316326.xyz/gtwmqebukb.html

[M01] 读取命令行参数
来源：http://hz.ywan-chungtsiang.top/gtceiiblbt.html

Py:   sys.argv[1:]
来源：http://hz.shzxlz.cn/gtrekuqziy.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtgkglzqqf.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtuaklqrnb.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtggpelend.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtnneoinul.html

Go:   os.Args[1:]
来源：http://hz.xuanzx.com/gtpbsjrmjr.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gtfnflfxul.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtxrgoixin.html

[M02] 读取环境变量
来源：http://hz.jianghu66.top/gthifstuwn.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtljtemyym.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtvrrcbrdw.html

JS:   process.env.HOME
来源：http://hz.cqqwz.cn/gtwzhlefjp.html

TS:   process.env.HOME
来源：http://hz.redwolf501.top/gtdtjmjczn.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtbxnrfpoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtbxjlywkf.html

Ruby: ENV["HOME"]
来源：http://hz.yonumen.top/gtqsbkyxfj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gttmhzohep.html

[M03] 执行外部命令
来源：http://hz.daxiang520.top/gthfysggio.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtqspqjirl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gtcdlhfazi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtbokmesgr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtiyuilqrm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ivvv.top/gtwttflieh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tanke756.top/gtwzbppnpb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.c1oappe.top/gtkpwozkdz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtsorwejit.html

[M04] 获取当前工作目录
来源：http://hz.yj20258888.top/gtmksajqvo.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gtcdhmzjtc.html

PHP:  getcwd();
来源：http://hz.zhiwuduotai.top/gtpjqasrbs.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gthrpylhgr.html

TS:   process.cwd()
来源：http://hz.gotoacloud.top/gttajcboes.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jyoumei.cn/gtbftearuf.html

Go:   os.Getwd()
来源：http://hz.yonumen.top/gtupsuquyj.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtxejehjhl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigfzy.top/gtartrmzui.html

[M05] 设置退出码
来源：http://hz.chenjidiqi.icu/gtvpkvppmh.html

Py:   sys.exit(1)
来源：http://hz.zhengqikj.top/gtgexsshdk.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtlpouzsjm.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtkicddyxr.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gtputmwjkf.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtepjgtqun.html

Go:   os.Exit(1)
来源：http://hz.zdqjudy.top/gtqjpwasar.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtpnuzmuna.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jyoumei.cn/gtnvtkxhyg.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtdmidmxee.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtfqolshyc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sysykeji.top/gthnjnmnvk.html

JS:   console.error("err")
来源：http://hz.dashuyun.cn/gtjwchfnig.html

TS:   console.error("err")
来源：http://hz.havefunace.top/gtjhveexzp.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtpcmnyatd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gthdsnmfhs.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gtktoctdxy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhixingplan.top/gtdofrxebk.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtewgsjdrf.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtqpxyegqi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtcbwzsjit.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gttnbjyefo.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtguliprxr.html

Java: public static void main(String[] args)
来源：http://hz.zhijiandao.cn/gtognoyawi.html

Go:   func main()
来源：http://hz.guannengcc.top/gtsohkobip.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.pycfn.com/gtzpbrcpqf.html

C#:   static void Main(string[] args)
来源：http://hz.cqqwz.cn/gtasmwlfsp.html

[M08] 获取系统与运行时信息
来源：http://hz.cucudq.cn/gtncmxwwoq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtqzwjytdk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cqqwz.cn/gtzyluwgmu.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtznhiyssh.html

TS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtutwlpcza.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sweek.top/gttjbacgab.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gtmkhatzpo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jlsjyb.cn/gtooguwxkn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dashuyun.cn/gtjxaomnyq.html

================================================================================
来源：http://hz.hysaishi.cn/gtfiznlhht.html

N. 数据结构与算法
来源：http://hz.316326.xyz/gtktvanxqk.html

================================================================================
来源：http://hz.snrcjt.cn/gtuzhrkyzs.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gtbqgkfptl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtcsyffjlq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.316326.xyz/gtbiuhntaq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gteswzghmj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtwooagdcs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtbzxxvyny.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtzflakqqv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tianlin.xyz/gtifihutfh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtryxjnoqx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtiqgjlgqc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gttueglcjq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sufxvd.cn/gtkhapaink.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtsveavhhz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtbipczxxc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenjidiqi.icu/gtnpxjuwfe.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258.top/gtvrhyscpa.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtcxxppjvz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangtech.top/gtdkmbtncw.html

[N03] 快速排序（分治示例）
来源：http://hz.ehwqpu.com/gtapkgddxa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jiagoushi.top/gtwocheinb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hfpthk.cn/gtfptgwtlh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtkbzzbqkd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtqhjaksah.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtvytoyawa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gticlvmrvl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtqmaoolkl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gtdmsgkjjv.html

[N04] 斐波那契数列
来源：http://hz.jlsjyb.cn/gtqcafvbea.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtgxidicmq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangshuangyany.cn/gtakjigael.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtcfvfyrjm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtwrpmzizq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gtezhcanih.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.andypj.xyz/gtjugzjaty.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtbzqsgoxv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.iojbl.cn/gtvgunewbs.html

[N05] 最大公约数
来源：http://hz.ydjk.org.cn/gtpltoibti.html

Py:   math.gcd(a, b)
来源：http://hz.shangyingyoupin.top/gtkjrneeta.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cucudq.cn/gtffbkshnb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtztggvqwp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtbbqinilx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenjidiqi.icu/gtpgvdbfeu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shuidangran.top/gtonlmqkas.html

Ruby: a.gcd(b)
来源：http://hz.ppjwa.cn/gtholqwmgs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gteawtxsog.html

[N06] 判断回文字符串
来源：http://hz.hysaishi.cn/gtzccbadgg.html

Py:   s == s[::-1]
来源：http://hz.ybcxt.top/gtiqycaycj.html

PHP:  $s === strrev($s);
来源：http://hz.gogol.net.cn/gtuqlxoaqj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtabvvsmjd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtrltzrdyt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtxkzsgzay.html

Go:   // 双指针从两端比较
来源：http://hz.yj202588.top/gtjbeipwfu.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gttcmhblog.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gthlhkxuir.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gthwjmtenn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sufxvd.cn/gtrljwvmly.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.meibo888.top/gtifnbmald.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aizwys.cn/gtozahtwdo.html

TS:   // 手写 Map<string, number>
来源：http://hz.yvedp.cn/gtymzecubf.html

Java: // 手写 HashMap
来源：http://hz.shangyingyoupin.top/gtbpvkqxao.html

Go:   // 手写 map[int]int
来源：http://hz.iojbl.cn/gtwpaqwbgr.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtywnfbiqn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhixingplan.top/gtrokwkemi.html

[N08] 生成全排列
来源：http://hz.xinyue.icu/gthfjsekva.html

Py:   itertools.permutations(arr)
来源：http://hz.sweek.top/gtbludnyhm.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gtbizoqzmh.html

JS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtpfnklcyl.html

TS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtssyosbcu.html

Java: // 手写回溯递归
来源：http://hz.tian-w.cn/gtsvcclery.html

Go:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtkezyfgai.html

Ruby: arr.permutation.to_a
来源：http://hz.jinghuilouyu.cn/gtfguhajrc.html

C#:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtedvlfuwx.html

[N09] 栈与队列
来源：http://hz.vqdsnc.cn/gtvzoakxko.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ehwqpu.com/gtjdklfbqw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtzxtcpufv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cucudq.cn/gtqkiyndrt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtvquprfyy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenjidiqi.icu/gtspzrkrps.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cheryme.top/gtnjevrggx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.snrcjt.cn/gtnpztphze.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtyjrmfroy.html

[N10] 链表节点定义
来源：http://hz.snrcjt.cn/gtfirzwujc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gtwswmxuxj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinqigfzy.top/gthvrxsrks.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.guannengcc.top/gtcacrxusi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydzc1.top/gtucnmwjrp.html

Java: class Node { int v; Node next; }
来源：http://hz.xinyue.icu/gtlxjpwlwf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gttosoodyo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hysaishi.cn/gtpwwgkzhd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.birdmap.top/gtgwzxqskm.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtrffftqoj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenzaomai.com/gtpfyxhdjh.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtecykjxas.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtbzphtuhe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtfiaidwfc.html

Java: // 手写递归
来源：http://hz.aizwys.cn/gtnychtqwy.html

Go:   // 手写递归
来源：http://hz.guannengcc.top/gtsimzlzhm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yangfankeji.com/gtmfkloudy.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtfkuohrmf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.smart0.xyz/gtvyflslub.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.quarkkingdee.top/gtsgjnirdk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhongyouzk.top/gtrunubqym.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtruzugedt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtuzcmiuoi.html


<!-- 参考信息 -->