代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtgktubupx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhoulong.xyz/gtbpyasvdi.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gteghzgqzl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aibaodan.cn/gtqzzcuntb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtqoyfikqp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gtdevknltn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtgywttetj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aizwys.cn/gtzqpbpisr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtihlmzjsy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yvedp.cn/gtuvgpvavo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtgllhiddd.html

[K05] 深拷贝对象
来源：http://hz.ydzc1.top/gtbrahvnds.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gttwvjdciz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xylfe.cn/gtxpmdcfgi.html

JS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtorvrnrcd.html

TS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtvvjffivp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guannengcc.top/gtlingprdm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tianlin.xyz/gtsednwjzz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenjidiqi.icu/gtoldemlxr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.iojbl.cn/gtajtzwlxy.html

[K06] 解析 URL 查询串
来源：http://hz.hongshengwenyu.top/gtxqmyhihj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtqapubira.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtmncugylp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtwqwkzsgc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtylghlokr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuanzhike.top/gtuhrtbmhf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtsutlndzh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zycfv.cn/gtbtighxsy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtqdgxvjff.html

[K07] 进制转换
来源：http://hz.snrcjt.cn/gtatjckirw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.quarkkingdee.top/gtxmsbrkap.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gtuoyghtjm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtooenftlq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtgwqjhguf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtrhvjrglg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hongshengwenyu.top/gtnkgckrbp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hfpthk.cn/gtfexluzsf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtldyhvtmo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sufxvd.cn/gtoushpjya.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtlnwdrbci.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.bjfxy.top/gtuiaavuvt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtxdgkappu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtrysqilqh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pengpengdd.cyou/gtaaoeaelz.html

Go:   encoding/gob
来源：http://hz.52xcode.cn/gtngoytrmu.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtwktkfuvc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gttkuudaov.html

================================================================================
来源：http://hz.hnqzz.top/gtboshnbao.html

L. 网络请求
来源：http://hz.yuxming.cn/gtopayacvi.html

================================================================================
来源：http://hz.nanxuanxn.top/gtowymywou.html

[L01] 发送 GET 请求
来源：http://hz.jlsjyb.cn/gtqimimkyt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhixingplan.top/gtlqwppjtb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtrenobcax.html

JS:   await fetch(url)
来源：http://hz.hammf.cn/gttwoboyhj.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtntrjybqt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtequjynwp.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtkbyikgru.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxinkj.top/gtimtvyexp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtrneistzm.html

[L02] 发送 POST JSON
来源：http://hz.guowangkeji.top/gteufchcld.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jyoumei.cn/gtqeytxpzm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gtnrjiwire.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtphwpfkfq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtbxtwrpty.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnxiangtu.top/gtcvyhkwvz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.0kj1m.cn/gtmfojqfpn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtuhmrmehf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gogol.net.cn/gtvusaovlu.html

[L03] 设置自定义请求头
来源：http://hz.zhongyouzk.top/gtipmbdgad.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtfswzvunc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtfnediedn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtqeaybtpo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtmehwoull.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xinyue.icu/gtbvrirnyz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sweek.top/gtrpgvctfl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nanxuanxn.top/gttqlpdxcc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtqxspujbx.html

[L04] 设置超时
来源：http://hz.yj20258888.top/gtklrizlmr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj202588.top/gtktlutszb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtkcmznhxw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtfoyupdjq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtwgaeejvm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jianghu66.top/gtwtjniynh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gtuhdmmhly.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.quarkkingdee.top/gtnfhgxmym.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtvwllpotg.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtyngjvhoy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtjpflthzq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hfpthk.cn/gtwujdjxqy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtbrvlxkti.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtqtlatuhv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydjk.org.cn/gtmksqnazo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gtxevcnerc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gtrgnvlwvt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangshuangyany.cn/gtfoifqqop.html

[L06] 解析响应为 JSON
来源：http://hz.ybcxt.top/gtrzwshtvt.html

Py:   resp.json()
来源：http://hz.gzhubu.top/gtxadvkpoq.html

PHP:  json_decode($body, true);
来源：http://hz.feifeiyinyue.top/gtxjaaivhp.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtwzkwliqf.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtprvrdxrw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuxming.cn/gtsaiowkjv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxinkj.top/gtvmncapxk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtfmpmvybh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shangyingyoupin.top/gtxicqiulk.html

[L07] 处理 HTTP 状态码
来源：http://hz.yvedp.cn/gtvezdqwen.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtvvgszyyo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jlsjyb.cn/gtqpvdmfgh.html

JS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtncmwrerb.html

TS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gthngpomce.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gttektujmo.html

Go:   resp.StatusCode
来源：http://hz.smart0.xyz/gttnmszddy.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtsjgrcgyx.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtobgpjvyc.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtglfdovjb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nanxuanxn.top/gtzbsbqbly.html

PHP:  curl_multi_init() 系列
来源：http://hz.hfpthk.cn/gtbvlaugjl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtkmdwqumu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtmflrbesj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.meibo888.top/gtgdotumcv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.svipenyu.cn/gtlxuweyyy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ywan-chungtsiang.top/gtaqamlijl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.birdmap.top/gtaoatmogy.html

================================================================================
来源：http://hz.jqgufenzy.top/gtephbcnpu.html

M. 命令行 / 进程 / 环境
来源：http://hz.ehwqpu.com/gtfjajmoey.html

================================================================================
来源：http://hz.0kj1m.cn/gtqjjwgonu.html

[M01] 读取命令行参数
来源：http://hz.daxiang520.top/gtysomrxkj.html

Py:   sys.argv[1:]
来源：http://hz.jinyuanbaomall.cn/gtmcofxlwa.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtchifjkrw.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtwrqqnrkp.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gteuidwhjg.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtzirctmpp.html

Go:   os.Args[1:]
来源：http://hz.yj20258888.top/gtlocwtlxb.html

Ruby: ARGV
来源：http://hz.shuidangran.top/gtnxwjvzhs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtxicsupsy.html

[M02] 读取环境变量
来源：http://hz.mhx1999.top/gtxpjzdqyu.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtwdssbnnw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gtwjusxfer.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtdsyrliko.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtozhlvywx.html

Java: System.getenv("HOME")
来源：http://hz.pengpengdd.cyou/gtegsmppak.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtasjhdoxn.html

Ruby: ENV["HOME"]
来源：http://hz.xingfuxueyuan.xyz/gtwcbcneol.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tian-w.cn/gteakaczpb.html

[M03] 执行外部命令
来源：http://hz.yj20258.top/gtvhtjsrog.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtqqhoaymq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gteudcgohw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtxbvfvmke.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtbtbyqnsb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gotoacloud.top/gtinktqvcv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtypwfupef.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtitkmbrcm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gtmblzhxkd.html

[M04] 获取当前工作目录
来源：http://hz.svipenyu.cn/gtusycwsxr.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtuwrtdlgw.html

PHP:  getcwd();
来源：http://hz.aizwys.cn/gtcbluhfav.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtnkqfkjdq.html

TS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtiwrizsft.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daria6918.cn/gtutmsspcc.html

Go:   os.Getwd()
来源：http://hz.xingfuxueyuan.xyz/gtouvdcwgm.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtudnabviz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtgtqwemjt.html

[M05] 设置退出码
来源：http://hz.pycfn.com/gtwyigbgir.html

Py:   sys.exit(1)
来源：http://hz.daria6918.cn/gtpxyegkrx.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gturmxpeny.html

JS:   process.exit(1)
来源：http://hz.dianchejie.cn/gtebcmjfmb.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtdlebdpsz.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtjlksqjoe.html

Go:   os.Exit(1)
来源：http://hz.chenjidiqi.icu/gtjswthdsf.html

Ruby: exit 1
来源：http://hz.jinyuanbaomall.cn/gtwphoebsr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sweek.top/gtepkdskiv.html

[M06] 向标准错误输出
来源：http://hz.aibaodan.cn/gtxlzxldlf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtodsqivlb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigfzy.top/gtulnjmpkv.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtmiaawohu.html

TS:   console.error("err")
来源：http://hz.cashguo.top/gtjugmbkki.html

Java: System.err.println("err")
来源：http://hz.ywan-chungtsiang.top/gtkxghdlji.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ivvv.top/gtqeemjihi.html

Ruby: warn "err"
来源：http://hz.cashguo.top/gtjgionhha.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtwcwflojc.html

[M07] 判断是否为主入口
来源：http://hz.feifeiyinyue.top/gtzmksgeoi.html

Py:   if __name__ == "__main__":
来源：http://hz.hysaishi.cn/gtybgljrkt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtthzdsawn.html

JS:   require.main === module
来源：http://hz.yj20258.top/gtaaiirncv.html

TS:   require.main === module
来源：http://hz.c1oappe.top/gtqueudkob.html

Java: public static void main(String[] args)
来源：http://hz.jinyuanbaomall.cn/gtrvysvshn.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtllaqpvpr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtwlsdresw.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtbzbwlbjv.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258.top/gtumtxgzmo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhongyouzk.top/gtccafhpxx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.feifeiyinyue.top/gtygpbmozi.html

JS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gtftkbyhov.html

TS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtuvlwfcqh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtptlvozno.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hongshengwenyu.top/gttcvqxvtl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangtech.top/gtozxaocan.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yongpay.top/gtnurkgsup.html

================================================================================
来源：http://hz.gzhubu.top/gtbynxfjxg.html

N. 数据结构与算法
来源：http://hz.gotoacloud.top/gtjybutqdm.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtojanzvqy.html

[N01] 二分查找（有序数组）
来源：http://hz.chenzaomai.com/gtksmohnqp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnqzz.top/gtzvfvzvyd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnqzz.top/gtvgohayrt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gtsncxliyu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtuehpocom.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtmfnktqkh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtdpuvykmw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pengpengdd.cyou/gtvcpvtgbv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtsudbvaum.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangshuangyany.cn/gtuqmjapmf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zycfv.cn/gttzzbnugj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gtqtrtvorf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtmnbxfzfw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtcrapwgla.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tian-w.cn/gtpivswmzz.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtbqwopsqh.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtmvwpikaf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hysaishi.cn/gtkqycdiyy.html

[N03] 快速排序（分治示例）
来源：http://hz.shzxlz.cn/gtpcdnlweg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenzaomai.com/gtbprftoed.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigfzy.top/gtrpotrhaq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinyuanbaomall.cn/gterkcyfdp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtvujftndk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtqitfkbus.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yongpay.top/gtfsblrmxb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtxooaifpp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhijiandao.cn/gtdhnlmzid.html

[N04] 斐波那契数列
来源：http://hz.ehwqpu.com/gtksdweorr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtnoxwpepa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangtech.top/gtluwyijgn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtxzjangyv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jiagoushi.top/gtkoxvsvjo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aibaodan.cn/gtfcgnwgqa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zycfv.cn/gtebmsddca.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtsyrsgrbq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hywenlv.cn/gtmjyzpppn.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gtdtaoxxps.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gtxkkpmlot.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ivvv.top/gtgdzomcvd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtqfiagonz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtdkwjzbvu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtwgdnecre.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuxming.cn/gtwloracnx.html

Ruby: a.gcd(b)
来源：http://hz.shanyushiyangkeji.top/gtqoyvieim.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gttkaeelnw.html

[N06] 判断回文字符串
来源：http://hz.zhiwuduotai.top/gtvjejnklr.html

Py:   s == s[::-1]
来源：http://hz.bjfxy.top/gtdvccqgrs.html

PHP:  $s === strrev($s);
来源：http://hz.9152youxi.cn/gtgqvrxltr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtmhossspa.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gthsmpgkhl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtcgignail.html

Go:   // 双指针从两端比较
来源：http://hz.9152youxi.cn/gtbwsonhiw.html

Ruby: s == s.reverse
来源：http://hz.chenlongwang.top/gtrluscxih.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtmhzbmfpi.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gtzpnfeixw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhijiandao.cn/gtqxwjcsqo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shuidangran.top/gtqebvbgez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtvzfxaywp.html

TS:   // 手写 Map<string, number>
来源：http://hz.9152youxi.cn/gtwcigirif.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtkiuptmky.html

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gtsokgsvpv.html

Ruby: // 手写 Hash
来源：http://hz.cdnleiting.top/gtjsrqkwng.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtveryxqtq.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtalrlpuks.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgfzy.top/gtqvdqoxpi.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtswbouuvc.html

JS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtuzckgoyg.html

TS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtmfyinxxo.html

Java: // 手写回溯递归
来源：http://hz.yangfankeji.com/gttchwrorp.html

Go:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtacxssdej.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gttmqoqvwq.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtxeofpcmx.html

[N09] 栈与队列
来源：http://hz.bjfxy.top/gtgqivxoup.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gogol.net.cn/gtdwfmtpzp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgufenzy.top/gtdvbavvky.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pycfn.com/gtphiupyyu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sysykeji.top/gtncbhsmee.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.redwolf501.top/gtnjgrsmqx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hywenlv.cn/gtrcjlkmsd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.birdmap.top/gtromqpnub.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.52xcode.cn/gtneplbjxy.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gthuqahsjy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.birdmap.top/gttumkfjtn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gtgycrocsm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shanyushiyangtech.top/gttvovmprz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.iojbl.cn/gtbzncesdz.html

Java: class Node { int v; Node next; }
来源：http://hz.yonumen.top/gtrnbwcpws.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yangfankeji.com/gtjbmjsljc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhoulong.xyz/gtgtoamlnu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangkeji.top/gtkwyamegt.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtttmgstlg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cqqwz.cn/gteyuqrunj.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gteezgndvb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtpnvltutp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtzyrfihlv.html

Java: // 手写递归
来源：http://hz.jiagoushi.top/gtuimylsox.html

Go:   // 手写递归
来源：http://hz.chenzaomai.com/gthrsulgki.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.kuanghao11.cn/gtanmcndee.html

C#:   // 手写递归
来源：http://hz.yueranfly.top/gtfzhpxhnj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gtjrvryimo.html


<!-- 参考信息 -->