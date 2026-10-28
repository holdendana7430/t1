代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sufxvd.cn/gtupxnyumy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtvbswedqs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtiiseioix.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhijiandao.cn/gtlaroovao.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtkrwaobuu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.iojbl.cn/gtlztytrtf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gtpmhyostk.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtoyehawhx.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtxpvleroo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guowangkeji.top/gttbcbakot.html

JS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtsmnmottx.html

TS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtsgymkrxb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtoflgzdyt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtnzslnevp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtjzlzhaeb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtaqkuddec.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gtqqeikxuv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cdnleiting.top/gtfaixkwxx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtcmocrgzd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtgansxpji.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtatoqhsnq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.havefunace.top/gtdqfopout.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtgwsmdnsy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fzhhl.top/gtkiyijibh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dianchejie.cn/gtfypbaxok.html

[K07] 进制转换
来源：http://hz.nanxuanxn.top/gtztzcephq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daxiang520.top/gttmfhhngn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yongpay.top/gtysftmelo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtnloroonz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtapiupwck.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gthaowpurn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zdqjudy.top/gtpggncadj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gttfkvwhgf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtgournrzq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gtoofrivir.html

Py:   pickle.dumps(obj)
来源：http://hz.zhongyouzk.top/gtvkfwasvh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtbtzymbho.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtvktmgvuw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtuqbisplo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtqcgdqwop.html

Go:   encoding/gob
来源：http://hz.c1oappe.top/gtpscxnvpv.html

Ruby: Marshal.dump(obj)
来源：http://hz.yvedp.cn/gtudlihadw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hammf.cn/gtmjijfduw.html

================================================================================
来源：http://hz.hysaishi.cn/gtjboeuthh.html

L. 网络请求
来源：http://hz.yuanzhike.top/gtvpdmbdee.html

================================================================================
来源：http://hz.cdnleiting.top/gttjulngwf.html

[L01] 发送 GET 请求
来源：http://hz.yj20258.top/gtegzzctpa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtbczspbgj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jianghu66.top/gthivyqbkj.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtwhoaszzz.html

TS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtvghfbmar.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ppjwa.cn/gtxfellywj.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtcmtfpbxy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhijiandao.cn/gtgolrkjlm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtxlxlvgjm.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtvftmdjdi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aizwys.cn/gtrpvlqsva.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtnxxyqcvd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtqaetqizn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtuetlgvkc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xinyue.icu/gtlirbllqh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtjknebrjq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dianchejie.cn/gtimcewvnp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sweek.top/gtldeptzfn.html

[L03] 设置自定义请求头
来源：http://hz.tianlin.xyz/gtyurjipvo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gtwtfovjfj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.c1oappe.top/gtrmfluqxx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtmlicpejn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtefdxeqji.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtfjtipkpe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gthhehdcjx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fengsongda.top/gtmtdxenvn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydzc1.top/gtmivdcwsc.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtkpztadub.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gogol.net.cn/gtprnolazt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtoaqqztxm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtdrbqguhf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtbkvyfnvf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258888.top/gttkuhekvb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtqbhcgkju.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gteudfdoxl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dianchejie.cn/gtxdqkbybw.html

[L05] 上传文件（multipart）
来源：http://hz.shuidangran.top/gtevxchssk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jyoumei.cn/gttmigqjkn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.0kj1m.cn/gtlcoxqouq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtebravvgz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtzxhzfxra.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtbdxqfyud.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guowangkeji.top/gtodgwasas.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtlyjaasgz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gtwwmlmrzo.html

[L06] 解析响应为 JSON
来源：http://hz.zdqjudy.top/gtpffeckjs.html

Py:   resp.json()
来源：http://hz.feifeiyinyue.top/gtzracoyvm.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gtxugysgxf.html

JS:   await resp.json()
来源：http://hz.andypj.xyz/gtfssubcfb.html

TS:   await resp.json()
来源：http://hz.316326.xyz/gtghfnuarw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sufxvd.cn/gtpkxhewex.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinyuanbaomall.cn/gtiakuvxad.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtvaegkmra.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dianchejie.cn/gtvxjtvaps.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtusdmnmus.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydjk.org.cn/gtqincppxf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtujqesqkp.html

JS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtucjtbwmy.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtousybzzq.html

Java: resp.statusCode()
来源：http://hz.yangfankeji.com/gtvjownvvj.html

Go:   resp.StatusCode
来源：http://hz.pycfn.com/gtilelasuj.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gtrhnepter.html

C#:   (int)resp.StatusCode
来源：http://hz.hnqzz.top/gtjhyhsszh.html

[L08] 并发请求多个地址
来源：http://hz.chenlongwang.top/gtmjcwypkg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shangyingyoupin.top/gtynsobbbu.html

PHP:  curl_multi_init() 系列
来源：http://hz.shangyingyoupin.top/gtzgzuhzhn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtojjsrhmt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtlmfviatp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jiagoushi.top/gtbwllhraa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtknshbsso.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.0kj1m.cn/gtvtiosaju.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sweek.top/gtcjjoauzd.html

================================================================================
来源：http://hz.cashguo.top/gtaqopvtvf.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gthjgqughp.html

================================================================================
来源：http://hz.ydjk.org.cn/gtivrajhmv.html

[M01] 读取命令行参数
来源：http://hz.zdqjudy.top/gtetcvnwqg.html

Py:   sys.argv[1:]
来源：http://hz.gaohongyu789.top/gtnhfxwkbs.html

PHP:  $argv;  $argc;
来源：http://hz.quarkkingdee.top/gtulgryrmf.html

JS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtowzawzzx.html

TS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtrqkartzf.html

Java: args 数组（main 方法参数）
来源：http://hz.sufxvd.cn/gtwktgsqtl.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtkgddzyjy.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gtemxtnuhi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtndvooqvv.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtthjniwjo.html

Py:   os.environ.get("HOME")
来源：http://hz.guannengcc.top/gtthkqmtcd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtjkkwgstm.html

JS:   process.env.HOME
来源：http://hz.cucudq.cn/gtgunqgtsq.html

TS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtzbagbtrv.html

Java: System.getenv("HOME")
来源：http://hz.ydzc1.top/gtgouboxpn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtiyjblzcx.html

Ruby: ENV["HOME"]
来源：http://hz.xuetiantiany.cn/gtdsfbsiyj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhijiandao.cn/gtszjskkwv.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gthgoejflp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.feifeiyinyue.top/gtkyeusjeh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtdexnprkm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtrmzuqgty.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtbvnfspil.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtdohfqqad.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gtggyauihj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtiorpuwof.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtpmpbkrps.html

[M04] 获取当前工作目录
来源：http://hz.daria6918.cn/gtfdsqhxbe.html

Py:   os.getcwd()
来源：http://hz.sweek.top/gtetawpdvs.html

PHP:  getcwd();
来源：http://hz.jqgfzy.top/gtnuojgkln.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtvkywfjvo.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gtzjfmkkpp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtiyfutsju.html

Go:   os.Getwd()
来源：http://hz.52xcode.cn/gtmvyybodw.html

Ruby: Dir.pwd
来源：http://hz.sufxvd.cn/gtrkmcgrws.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.wangshuangyany.cn/gtnlejaccs.html

[M05] 设置退出码
来源：http://hz.tianlin.xyz/gtjxcykdin.html

Py:   sys.exit(1)
来源：http://hz.jqgufenzy.top/gtvhqhwlqc.html

PHP:  exit(1);
来源：http://hz.ydzc1.top/gtvwkkmtcw.html

JS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtwwddrsbb.html

TS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtpuzsewmj.html

Java: System.exit(1)
来源：http://hz.redwolf501.top/gtiqictnbr.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtwpnjghkm.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gtxhepwyro.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhijiandao.cn/gteizumppl.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gtwfiwkcuu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtokqlhwin.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guannengcc.top/gtyjybbpjf.html

JS:   console.error("err")
来源：http://hz.sweek.top/gtepodzaqh.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtrwkrsapc.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtzgituyla.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtwrexlmrv.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtmvlryeaf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtfsoczhhk.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gtqjwwwdwc.html

Py:   if __name__ == "__main__":
来源：http://hz.aibaodan.cn/gtfszyogpp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtbqnbsosi.html

JS:   require.main === module
来源：http://hz.smart0.xyz/gtryhjgiim.html

TS:   require.main === module
来源：http://hz.hfpthk.cn/gtzrpjyszi.html

Java: public static void main(String[] args)
来源：http://hz.tianlin.xyz/gthazrnupv.html

Go:   func main()
来源：http://hz.hnxiangtu.top/gtvezczzzo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sufxvd.cn/gtitmghpdn.html

C#:   static void Main(string[] args)
来源：http://hz.gzhubu.top/gtcnnxzzcv.html

[M08] 获取系统与运行时信息
来源：http://hz.c1oappe.top/gtqustptln.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gzhubu.top/gtsxorhrpw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shuidangran.top/gtpttibqyc.html

JS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtteiqjgrw.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtegviefjs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtmcngmjok.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.52xcode.cn/gtvqomzkbv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigfzy.top/gtqxqhssda.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yangfankeji.com/gtrsmrponf.html

================================================================================
来源：http://hz.nanxuanxn.top/gtlsuhdmsx.html

N. 数据结构与算法
来源：http://hz.cqqwz.cn/gtbalvyzoi.html

================================================================================
来源：http://hz.ehwqpu.com/gtsmcfdccg.html

[N01] 二分查找（有序数组）
来源：http://hz.tian-w.cn/gtcequfuzy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gttlmrbguj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pycfn.com/gttucpydgo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shangyingyoupin.top/gtjsgzdpdq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtwebghdln.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtafhvwnvs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtjusixcjk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.316326.xyz/gtcwvtxzce.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gtoritrntt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinyuanbaomall.cn/gtofeqwuts.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtepffcuoa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hongshengwenyu.top/gtxxufxbpu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtguqqwclf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtuvgcwkgw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenjidiqi.icu/gtospuleqk.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtfkcpbjuz.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtypyjlmax.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gtusdiykhv.html

[N03] 快速排序（分治示例）
来源：http://hz.chenzaomai.com/gtgyatlgfq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtsvcdwpkh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aizwys.cn/gtsbpgpfps.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtshzwlseb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtwqtkbjob.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hywenlv.cn/gtzinleqea.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtxgyjhmcu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gtlkakaksd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shangyingyoupin.top/gtbrernxah.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtddxwqwxw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gtkojfrioo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.meibo888.top/gtseapuytc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtsnekliph.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtnnfrpkno.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.9152youxi.cn/gtevdcdrfu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtdjliifzb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtdqemvjnd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.9152youxi.cn/gtktdpbunp.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtqhotxlyt.html

Py:   math.gcd(a, b)
来源：http://hz.gzhubu.top/gtkprpgvwt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cdnleiting.top/gtwdfoxgzs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gttcqzrqyp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtcebncprx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinyuanbaomall.cn/gtzzicijso.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigfzy.top/gtmlbsfolg.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtbtswpwpf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gtaansnsic.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gtyygqpwtp.html

Py:   s == s[::-1]
来源：http://hz.pengpengdd.cyou/gtrwstumei.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gtbkdynjvl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtctxqpsdo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtgcbkxfpv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pycfn.com/gtjmazlfkl.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigufen.top/gtcjtapuwv.html

Ruby: s == s.reverse
来源：http://hz.sxryk.cn/gtvwkqpmxg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtuuasjnpu.html

[N07] 两数之和（返回下标）
来源：http://hz.shuidangran.top/gtntkmfmwq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cucudq.cn/gtlnsepaet.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgufenzy.top/gturnsiaey.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zycfv.cn/gtyvhzvjxh.html

TS:   // 手写 Map<string, number>
来源：http://hz.xingfuxueyuan.xyz/gtkxhtodoz.html

Java: // 手写 HashMap
来源：http://hz.guowangkeji.top/gtajcytukg.html

Go:   // 手写 map[int]int
来源：http://hz.c1oappe.top/gtcykeqhrk.html

Ruby: // 手写 Hash
来源：http://hz.aizwys.cn/gttvgcynxw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aibaodan.cn/gtpfitnvpr.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtwwgklzfk.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtbmcjhiyq.html

PHP:  // 手写递归交换
来源：http://hz.zycfv.cn/gtsaezvore.html

JS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtlvjlhoeu.html

TS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtbmbkbbwc.html

Java: // 手写回溯递归
来源：http://hz.shzxlz.cn/gtoidfybkg.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtuyfmncsj.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtqbcilrzx.html

C#:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtkopfbspa.html

[N09] 栈与队列
来源：http://hz.tian-w.cn/gtoowvibnc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xuanzx.com/gtozbtjadp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258.top/gtmbefshuy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sysykeji.top/gtecgnjfzt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daxiang520.top/gtwkknrpsc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pengpengdd.cyou/gtppqxczkh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tianlin.xyz/gtprxpesog.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.0kj1m.cn/gtsyinhfiy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cucudq.cn/gthihmcgub.html

[N10] 链表节点定义
来源：http://hz.zhiwuduotai.top/gtpucljtef.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cdnleiting.top/gtmrovgmig.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnxiangtu.top/gtrpolvbvz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nanxinkj.top/gtembakxpy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shzxlz.cn/gtibkuozoq.html

Java: class Node { int v; Node next; }
来源：http://hz.9152youxi.cn/gtcaaxmeze.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pengpengdd.cyou/gttaiwfncx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ybcxt.top/gtmjptkbos.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hywenlv.cn/gtexkvonvc.html

[N11] 二叉树中序遍历
来源：http://hz.zhixingplan.top/gthpccjsrx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.dianchejie.cn/gtlmsyidjb.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtowvzghea.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtepcposwl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shzxlz.cn/gtfwocecvq.html

Java: // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtqqxzwqyl.html

Go:   // 手写递归
来源：http://hz.dashuyun.cn/gtywvdexmw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtphgyciov.html

C#:   // 手写递归
来源：http://hz.zdqjudy.top/gtsebuuanw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtzyisypyt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hywenlv.cn/gtpgxlpbsj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtgfdhlknb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtihaaonwu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtvafjxqfn.html


<!-- 参考信息 -->