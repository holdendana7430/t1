代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.bjfxy.top/gtqsyeisuu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hfpthk.cn/gtoavjiyie.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtznzbhrhp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ehwqpu.com/gtqdiuggll.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtybwbhjvb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gttktapqxv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gtxwknrkyj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtrttguroc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gthyytygcf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.vqdsnc.cn/gtjovxivkp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hongshengwenyu.top/gtvzajaojl.html

[K05] 深拷贝对象
来源：http://hz.vqdsnc.cn/gtehafkybx.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtfbdprlua.html

PHP:  unserialize(serialize($obj));
来源：http://hz.9152youxi.cn/gtkkxkykal.html

JS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtsmeodkpq.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtkgeelqor.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtlcivacme.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hywenlv.cn/gtkzxlsrsn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtpzifihdd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.mhx1999.top/gtjkyfxvlf.html

[K06] 解析 URL 查询串
来源：http://hz.fzhhl.top/gtouxupvnv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gtjcuiqrma.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gtlocxeyio.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gteuzdjlyv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtvazdppmr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gzhubu.top/gtgpkatbgq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtdyaxfcjb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtqmbwjyhs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtsmzeizfw.html

[K07] 进制转换
来源：http://hz.zycfv.cn/gtlzpoxjjv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gotoacloud.top/gttuobsuax.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guannengcc.top/gtwrrksfsq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtkabukauh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gttsrebajp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtnzoodiyv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtjcoyfawn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ywan-chungtsiang.top/gtskpnbrhn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtikycnjan.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gttgtzgosw.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtogoddkfl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ybcxt.top/gttiapccqo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtxlgpqcle.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtylbdbqpy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tian-w.cn/gtiqohvejl.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtafexpiln.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtcaevktug.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tian-w.cn/gtuhhanxql.html

================================================================================
来源：http://hz.ybcxt.top/gtpydbtkes.html

L. 网络请求
来源：http://hz.jlsjyb.cn/gttbicojwh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwcpovcol.html

[L01] 发送 GET 请求
来源：http://hz.fengsongda.top/gtaxqysgqu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sxryk.cn/gtocuznbpc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gtvpvvwzns.html

JS:   await fetch(url)
来源：http://hz.zhoulong.xyz/gtlevgvrzo.html

TS:   await fetch(url)
来源：http://hz.52xcode.cn/gtllxxltcv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.andypj.xyz/gttcfntaym.html

Go:   resp, err := http.Get(url)
来源：http://hz.yongpay.top/gtzcbwwhsn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.316326.xyz/gteypgfxgi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhaomingkeji.xyz/gtwvuzjtlx.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gtzdebfcbu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtthpkvstj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gtlfziciaj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtccfmjltv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtrlhgjyyr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtrtoinpbg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuanzhike.top/gtctqzxnky.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258.top/gtlenzhhrt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhixingplan.top/gtzqdzmtnv.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtmwslnflq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cqqwz.cn/gtnwqvnptf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gtfsmzsnkb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtimcnuqwf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtorcucoug.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgfzy.top/gtuqilchzh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtosuzptjz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtxzbcvquj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtsdwqyueg.html

[L04] 设置超时
来源：http://hz.sxryk.cn/gtpehvmvco.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhixingplan.top/gtuzhpxwsf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.316326.xyz/gtzvmmwtuc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtatntghls.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtagqksfhg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guowangkeji.top/gtmcvrssys.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tian-w.cn/gtoqwmokbu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhiwuduotai.top/gthcgxprhb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zycfv.cn/gtlussomki.html

[L05] 上传文件（multipart）
来源：http://hz.pycfn.com/gtakdkkcmy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtcbffidof.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258.top/gtnujlznzh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtrbkoybso.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtjykllwyj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xziqi.cn/gtjdgyvzjc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.meibo888.top/gtkwcmfeeu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gaohongyu789.top/gtfitehqym.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangshuangyany.cn/gtfltzylhp.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gttkgisftg.html

Py:   resp.json()
来源：http://hz.shuidangran.top/gthjohezln.html

PHP:  json_decode($body, true);
来源：http://hz.mhx1999.top/gtujqdpgts.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gtnlvlicoc.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gtrwxveohx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jyoumei.cn/gtefjzsxnn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aizwys.cn/gtsivatote.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtigdfkbbk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.svipenyu.cn/gtvexynmiw.html

[L07] 处理 HTTP 状态码
来源：http://hz.dianchejie.cn/gtlpgicyfn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gtcfwexmce.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtohbfzzaq.html

JS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtxjltqmkt.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtcmvjxlqu.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtbeohjnzh.html

Go:   resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtyqxqyorl.html

Ruby: resp.code.to_i
来源：http://hz.hysaishi.cn/gtefjtamfy.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtzjnwrzpg.html

[L08] 并发请求多个地址
来源：http://hz.svipenyu.cn/gtvusvdwjz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.smart0.xyz/gtxyeufxly.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gteyyiebub.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtrjmrtqld.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtohyxomcr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sweek.top/gtsfsyokgm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjfxy.top/gtfndridiu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gthfzraaxr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.svipenyu.cn/gttfnwload.html

================================================================================
来源：http://hz.zhengqikj.top/gtdgiduvdz.html

M. 命令行 / 进程 / 环境
来源：http://hz.cucudq.cn/gtrxjseyne.html

================================================================================
来源：http://hz.hfpthk.cn/gtvhukoawg.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtvfmnebtg.html

Py:   sys.argv[1:]
来源：http://hz.vqdsnc.cn/gtuhgjqxlx.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gtdlcablqd.html

JS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtbddwlejr.html

TS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtgknddkbb.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtcijiganz.html

Go:   os.Args[1:]
来源：http://hz.zhengqikj.top/gtitoknanw.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtzjpaednw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gttkukzdai.html

[M02] 读取环境变量
来源：http://hz.yonumen.top/gtpcxxznou.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtofjetxge.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gtucecbwhi.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtxdzgyqlk.html

TS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtaqqmfkjc.html

Java: System.getenv("HOME")
来源：http://hz.hongshengwenyu.top/gtfhtswqgs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtixdolhqq.html

Ruby: ENV["HOME"]
来源：http://hz.sweek.top/gtrotmzuss.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ivvv.top/gtzjjvnups.html

[M03] 执行外部命令
来源：http://hz.chenjidiqi.icu/gtcgoetoym.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinqigfzy.top/gtcxmggqdu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtznyrxppi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtntyiumhg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtyjsbkqvq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtgldqjwnu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gtdtpovfgi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guannengcc.top/gtzqwuones.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtpnxiadnk.html

[M04] 获取当前工作目录
来源：http://hz.dashuyun.cn/gtevjeoqrs.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtzffdbdqe.html

PHP:  getcwd();
来源：http://hz.xziqi.cn/gtnjvxobxe.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtxfbiciom.html

TS:   process.cwd()
来源：http://hz.yuxming.cn/gtcepuhalo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gtmcmpredt.html

Go:   os.Getwd()
来源：http://hz.chenzaomai.com/gtmupmraqw.html

Ruby: Dir.pwd
来源：http://hz.haohaochexian.top/gtiunwvhyl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yangfankeji.com/gtozxdqhzi.html

[M05] 设置退出码
来源：http://hz.hywenlv.cn/gtmpxukcxn.html

Py:   sys.exit(1)
来源：http://hz.snrcjt.cn/gttqymiigr.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtjculdeet.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtpuipqjkh.html

TS:   process.exit(1)
来源：http://hz.iojbl.cn/gttfesrwxh.html

Java: System.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtcylqpvhr.html

Go:   os.Exit(1)
来源：http://hz.daxiang520.top/gtfivlcixs.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtmyiuenfs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gtwdnulyex.html

[M06] 向标准错误输出
来源：http://hz.c1oappe.top/gtgrlhwqnn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gtnqnlcfnr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.52xcode.cn/gtjxdzjulf.html

JS:   console.error("err")
来源：http://hz.yongpay.top/gtwmwoboaq.html

TS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtpddrohae.html

Java: System.err.println("err")
来源：http://hz.ehwqpu.com/gtfhhhedvx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtybxjuokc.html

Ruby: warn "err"
来源：http://hz.cashguo.top/gtdglnwbww.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtosbfowga.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtxmddglcu.html

Py:   if __name__ == "__main__":
来源：http://hz.hnxiangtu.top/gtdtkqxfdl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.kuanghao11.cn/gtqucvwatf.html

JS:   require.main === module
来源：http://hz.jiagoushi.top/gtrlcuyjvx.html

TS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtuhwyoewd.html

Java: public static void main(String[] args)
来源：http://hz.iojbl.cn/gtaswseova.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gtjurgjtdg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhaomingkeji.xyz/gteyabpoxu.html

C#:   static void Main(string[] args)
来源：http://hz.zhaomingkeji.xyz/gtltvpkyxj.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gtcsoewryi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtuaivnpse.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258888.top/gtxircqbni.html

JS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gticlovkfo.html

TS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtiychdwjo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.316326.xyz/gtraqggqkk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtsfbpymyr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gaohongyu789.top/gthjnvefvl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtzuebofko.html

================================================================================
来源：http://hz.hysaishi.cn/gtbvztnmmu.html

N. 数据结构与算法
来源：http://hz.zhiwuduotai.top/gtwtpsagdn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdchmqdxf.html

[N01] 二分查找（有序数组）
来源：http://hz.xziqi.cn/gtcnuybzvy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtpyfstnuo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xinyue.icu/gtlxjbetnr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtgbpafpjg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtfwmbueeb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.haohaochexian.top/gtjdcotkww.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yanxiufei.cn/gtpgjphizj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.9152youxi.cn/gtfhfrzhzn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sysykeji.top/gtdjcidost.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangtech.top/gtxbasbhzh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtdbivisxg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.iojbl.cn/gtzygpiwxc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtjwobgvou.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtuatvcqzl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuetiantiany.cn/gtouhvvftc.html

Go:   slices.Sort(arr)
来源：http://hz.tian-w.cn/gtzmtsosru.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtgbtxwxkw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangkeji.top/gtoqhifbtf.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtniizfjwb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtkqsuklrd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuanzx.com/gttgbsbzbz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtcrpbsyqu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtvjriqife.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sufxvd.cn/gtbwblmvhm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hfpthk.cn/gtxacxfjyu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gzhubu.top/gtvzgjhgai.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.mhx1999.top/gtvuuolohd.html

[N04] 斐波那契数列
来源：http://hz.yongpay.top/gtbotafqwi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtcxghurfn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sweek.top/gtfiejuhgj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtienhggde.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtrnbkjcgz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtzgixnpbj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydjk.org.cn/gtotsolbrd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtagqptyvw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhoulong.xyz/gtbsgkjdwo.html

[N05] 最大公约数
来源：http://hz.zdqjudy.top/gtgqbqhvzb.html

Py:   math.gcd(a, b)
来源：http://hz.kuanghao11.cn/gtcjskkrkj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hfpthk.cn/gtsyvfdwdn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gthnibbepz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtelkyypop.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.fzhhl.top/gtudujtulb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cdnleiting.top/gtkpxzslwy.html

Ruby: a.gcd(b)
来源：http://hz.yuanzhike.top/gtxllwvlmn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.iojbl.cn/gtqtajiwls.html

[N06] 判断回文字符串
来源：http://hz.c1oappe.top/gtcmqmvpze.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtzlblaxei.html

PHP:  $s === strrev($s);
来源：http://hz.mhx1999.top/gtzbpltejl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtdlybogof.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtokucxahy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtmeevjrji.html

Go:   // 双指针从两端比较
来源：http://hz.ehwqpu.com/gtmjevgxvo.html

Ruby: s == s.reverse
来源：http://hz.xziqi.cn/gtjbcsfwjl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gthmuvsxuq.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtrweuecpe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258.top/gthaocoiuk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtcrnziweo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yangfankeji.com/gtdgaynwyu.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtfvtytexk.html

Java: // 手写 HashMap
来源：http://hz.chenzaomai.com/gtrcwehxln.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtvjqtsdfg.html

Ruby: // 手写 Hash
来源：http://hz.jqgufenzy.top/gtziaiimhh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtqthmodej.html

[N08] 生成全排列
来源：http://hz.zhiwuduotai.top/gtsxywkdla.html

Py:   itertools.permutations(arr)
来源：http://hz.chenzaomai.com/gtqexqvqny.html

PHP:  // 手写递归交换
来源：http://hz.xingfuxueyuan.xyz/gtntdqslyw.html

JS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtsaovwane.html

TS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtmwmrdqka.html

Java: // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtgwullkrr.html

Go:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtvcgsoczo.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gtgevuhbue.html

C#:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtbeujnvmd.html

[N09] 栈与队列
来源：http://hz.jqgfzy.top/gtoacwmbqm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.snrcjt.cn/gtwqvqrgsn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dianchejie.cn/gtyhawjyix.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtmtcnnhnj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtqfidfxge.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cqqwz.cn/gtuwgnduak.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tianlin.xyz/gtwrsgekxf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xziqi.cn/gtxiwkrqcn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhiwuduotai.top/gtbajqrwvm.html

[N10] 链表节点定义
来源：http://hz.zhoulong.xyz/gttiaqrymv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.c1oappe.top/gtydjwskzn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hysaishi.cn/gtyprnigbq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtgiumacrk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ehwqpu.com/gtaipppoaj.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gthyrzwhqq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gtbcjswskv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yueranfly.top/gtkieiyzrk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinqigufen.top/gtsmlmmurt.html

[N11] 二叉树中序遍历
来源：http://hz.hnqzz.top/gtrwhyenwx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.bjfxy.top/gtvoppqylp.html

PHP:  // 手写递归函数
来源：http://hz.yueranfly.top/gtlyyxrboa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtkskuozog.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtucfcqncy.html

Java: // 手写递归
来源：http://hz.ydjk.org.cn/gtkkwhaoza.html

Go:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtorgawdmz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gttcaltcte.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtidfxkjfh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sufxvd.cn/gtgsjtkzdu.html


<!-- 参考信息 -->