代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtvntgqibt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtcjibzcst.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258.top/gtbysituys.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtezhcptoh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gtethzbimc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jlsjyb.cn/gtfjxnximt.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtejylykgm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cucudq.cn/gtkecxqjdb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtffoziulp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtcmuoyktn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtlvsorlll.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtzuzzdgrj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gttlmtasuw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gtsqauxvbs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zycfv.cn/gthjfwnhwg.html

[K05] 深拷贝对象
来源：http://hz.fzhhl.top/gtgfqzrmro.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtjobhjouk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtesscsjix.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtddhmpvkt.html

TS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtlmpovarm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtijzhwrnm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gturjpsyfg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.52xcode.cn/gtbdehmwcj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.birdmap.top/gtrxdmgwal.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gtchmdpdlm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtwpskfskf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jyoumei.cn/gtteyvkipa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtvdgwqvad.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtdutenqlb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtphrkvipj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuxming.cn/gttbfforoo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gtbrwnwppb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtryhveyml.html

[K07] 进制转换
来源：http://hz.bjfxy.top/gtsstrtcjw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtopfvdbzt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yueranfly.top/gtgwnvshrm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtrboghoyc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtxwjuvjfv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtnmnolubz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenlongwang.top/gtgxwcykmn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtfukcdecz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tianlin.xyz/gtuerynihn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydzc1.top/gtmlfxmkkc.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtvvsdxrfn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuxming.cn/gtowelrvms.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtuxyhhaza.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtgcnoduda.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tanke756.top/gtswbsvtac.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtksvpvbmo.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258888.top/gtalsipxeh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtjvmgziwr.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtaufjqmfp.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gtfmgsttbp.html

================================================================================
来源：http://hz.yongpay.top/gttbrlcyya.html

[L01] 发送 GET 请求
来源：http://hz.hysaishi.cn/gtbimdtbyk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtludqyvxs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.svipenyu.cn/gtdetvdmwp.html

JS:   await fetch(url)
来源：http://hz.yuxming.cn/gtdxwywkvh.html

TS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtirmrzeco.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tian-w.cn/gteoakhate.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gtthaoqlbo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.svipenyu.cn/gtdxhikqyr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtlrybsoll.html

[L02] 发送 POST JSON
来源：http://hz.zhoulong.xyz/gtpojopnlg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangkeji.top/gtgbsslpic.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cashguo.top/gtrfsxcwil.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtmvygvmwn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtrithxcam.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.andypj.xyz/gtovvqeyfa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenlongwang.top/gtwovqqibq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nwbrower.top/gttrciookw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuetiantiany.cn/gtpgkuofyo.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gtuafyopoz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.c1oappe.top/gtjohojlso.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnxiangtu.top/gtbbncpjam.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtitvjifrq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtsyegidpt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gthoiacoeu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtnchwpycb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtlfmessnv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtfmlupqlj.html

[L04] 设置超时
来源：http://hz.sweek.top/gtotiatayb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cqqwz.cn/gtamxlkklx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shangyingyoupin.top/gtpbqmqndi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtuqaiqxtm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtutamufqq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hywenlv.cn/gtuzxjphdz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.0kj1m.cn/gtgdqkkeku.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtxhcnqkkg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtgsmgvdeg.html

[L05] 上传文件（multipart）
来源：http://hz.nanxuanxn.top/gtnmkbsvce.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtxlrtyrlc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ybcxt.top/gtfdkkprbb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtnkwurtrb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtpyrrrqtl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jyoumei.cn/gtdmoxedyq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.316326.xyz/gtrkdpbwoj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sysykeji.top/gtuazcryjj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258888.top/gtisycmcpx.html

[L06] 解析响应为 JSON
来源：http://hz.bjfxy.top/gthjmfeaix.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gtqbewmwpm.html

PHP:  json_decode($body, true);
来源：http://hz.cheryme.top/gtcerutkph.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gteprwghpm.html

TS:   await resp.json()
来源：http://hz.yj202588.top/gtfzxrnhge.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtohafmdys.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhaomingkeji.xyz/gtsvhobksr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jlsjyb.cn/gtrpdrvqdq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtgfcforaw.html

[L07] 处理 HTTP 状态码
来源：http://hz.aizwys.cn/gtgiprifih.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yangfankeji.com/gtpotxrcpk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tian-w.cn/gttoazingd.html

JS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtolkqifqf.html

TS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtnmkjgtow.html

Java: resp.statusCode()
来源：http://hz.zhijiandao.cn/gtfeqcyfyf.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtvhbssdei.html

Ruby: resp.code.to_i
来源：http://hz.xinyue.icu/gtbrribqge.html

C#:   (int)resp.StatusCode
来源：http://hz.daxiang520.top/gtskwjjaya.html

[L08] 并发请求多个地址
来源：http://hz.sufxvd.cn/gttiukrick.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aizwys.cn/gtvshrtzpw.html

PHP:  curl_multi_init() 系列
来源：http://hz.jianghu66.top/gteqfbdkag.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtsfxwmrqw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gthlfhzbxc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yueranfly.top/gtbyaxohkr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtjmkrbvxw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtmlnijtap.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxuanxn.top/gtttwtefjy.html

================================================================================
来源：http://hz.zycfv.cn/gtwdkqtmpw.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtycczeibu.html

================================================================================
来源：http://hz.shuidangran.top/gtvojabyzl.html

[M01] 读取命令行参数
来源：http://hz.hnxiangtu.top/gtstnkyrpz.html

Py:   sys.argv[1:]
来源：http://hz.zhixingplan.top/gthvblkvub.html

PHP:  $argv;  $argc;
来源：http://hz.zhiwuduotai.top/gtuiddcnrv.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtwkwgjxfn.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtjdleruwe.html

Java: args 数组（main 方法参数）
来源：http://hz.yuxming.cn/gtucquzhrp.html

Go:   os.Args[1:]
来源：http://hz.nanxinkj.top/gtfaljbfxr.html

Ruby: ARGV
来源：http://hz.ydjk.org.cn/gtwzyapqro.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shangyingyoupin.top/gtbsksjgrq.html

[M02] 读取环境变量
来源：http://hz.snrcjt.cn/gtbplymxan.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtmcvmdcno.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtzhnyjdcg.html

JS:   process.env.HOME
来源：http://hz.haohaochexian.top/gtuojcvroc.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtopikfisg.html

Java: System.getenv("HOME")
来源：http://hz.snrcjt.cn/gtxmsszclz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtxgjiidfw.html

Ruby: ENV["HOME"]
来源：http://hz.zhixingplan.top/gtrtgsyotk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtmhlwlvgs.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangkeji.top/gtcssrwlkx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.haohaochexian.top/gtmrmgoekp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtckdsrrmy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tianlin.xyz/gtifraprnl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtoykmpooh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gteklezngy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zycfv.cn/gtmxksbjhn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xziqi.cn/gtfbwgjrur.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gtqhxiiife.html

[M04] 获取当前工作目录
来源：http://hz.gaohongyu789.top/gtphezcgkd.html

Py:   os.getcwd()
来源：http://hz.gaohongyu789.top/gtygobhokv.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtneuxkgxv.html

JS:   process.cwd()
来源：http://hz.ivvv.top/gtlhalbzfa.html

TS:   process.cwd()
来源：http://hz.bjfxy.top/gtjarrwpjg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gthyvyyudm.html

Go:   os.Getwd()
来源：http://hz.pengpengdd.cyou/gtyhijuneb.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtpsvxdrah.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnqzz.top/gtqtbmjqvp.html

[M05] 设置退出码
来源：http://hz.tian-w.cn/gtekxnngqy.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gtawraxqeq.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtdwqtqria.html

JS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtnjtcxlot.html

TS:   process.exit(1)
来源：http://hz.shangyingyoupin.top/gtgpxixsve.html

Java: System.exit(1)
来源：http://hz.zhengqikj.top/gtyerntzmu.html

Go:   os.Exit(1)
来源：http://hz.cashguo.top/gtsfghslnw.html

Ruby: exit 1
来源：http://hz.zhaomingkeji.xyz/gttirakxzl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ywan-chungtsiang.top/gtqyxcbbum.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtkuzvqwam.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtsgcofbti.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.iojbl.cn/gttymfsxqt.html

JS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtiouldfqk.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtvggfwpjy.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtzscqnojo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtsxltfist.html

Ruby: warn "err"
来源：http://hz.quarkkingdee.top/gtzubiwnns.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtasffedwy.html

[M07] 判断是否为主入口
来源：http://hz.gotoacloud.top/gtrudqpeob.html

Py:   if __name__ == "__main__":
来源：http://hz.ybcxt.top/gtxxiyenyc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ivvv.top/gtjgnnkrho.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtzugzeuxl.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtpxvwjxry.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtvsilzjwb.html

Go:   func main()
来源：http://hz.zhaomingkeji.xyz/gtuqqzseiq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtlpxdcjyw.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtglejxrff.html

[M08] 获取系统与运行时信息
来源：http://hz.havefunace.top/gtankowhsi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtlbvvwfbv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xziqi.cn/gtsnczplts.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtivqwpqhu.html

TS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gttexzqgiu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tanke756.top/gtpsfyxbyh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cucudq.cn/gthfiwxdab.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.andypj.xyz/gtzrtfjofk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shuidangran.top/gtokvewfao.html

================================================================================
来源：http://hz.ydjk.org.cn/gtlswkkkxf.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtkxxkossi.html

================================================================================
来源：http://hz.yuxming.cn/gtsavesmlr.html

[N01] 二分查找（有序数组）
来源：http://hz.dianchejie.cn/gtikdhecpo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhongyouzk.top/gtpnepdclb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhongyouzk.top/gtbocysalx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtvogszdce.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtvgsmqhjv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtziqqvqqj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gtanqieppp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sxryk.cn/gtyndjqmnl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xziqi.cn/gtlvpicqbo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sxryk.cn/gtivxabdeg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtebyvntcp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gtltrfmyiy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtzheffmuj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtnfzptfrk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pengpengdd.cyou/gtqmmdbdkz.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtckslffls.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtbbcpyxxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gtdmvvqrxi.html

[N03] 快速排序（分治示例）
来源：http://hz.zhoulong.xyz/gtnilaafdj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jlsjyb.cn/gtukljsccq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtcryqzlww.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gttaftlqrj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtfiaexqkk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.birdmap.top/gtbniguude.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gtbrhmgowj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtatuabxwl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtmyxilpti.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtrcsseqrq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtpbzljahi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnqzz.top/gtliolzckv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gttmllsisc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhengqikj.top/gtyhasrnrf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtdqaitogp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nwbrower.top/gtuusvmkzj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtjbzwhvim.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sweek.top/gtvndmsdwp.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtccivztno.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gtuttullvd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hywenlv.cn/gtoaqffkgz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtbzjapwlt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtftiqtrqn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtwwsnoirb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtssxlarcd.html

Ruby: a.gcd(b)
来源：http://hz.meibo888.top/gtjgxipayx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sysykeji.top/gtugayzmqe.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtatjxxbom.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtrewalbee.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gtadnphhjp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtfgspslhk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtykufyqpu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangshuangyany.cn/gtihnclgxc.html

Go:   // 双指针从两端比较
来源：http://hz.chenzaomai.com/gtamnegyeh.html

Ruby: s == s.reverse
来源：http://hz.wangshuangyany.cn/gtedxeaflg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtlmzlmpxw.html

[N07] 两数之和（返回下标）
来源：http://hz.daxiang520.top/gtfhfdpein.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuetiantiany.cn/gtarqtlpgk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.9152youxi.cn/gtbwndigcx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hfpthk.cn/gtdajhfhot.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtjspmknwx.html

Java: // 手写 HashMap
来源：http://hz.52xcode.cn/gtsjgekohx.html

Go:   // 手写 map[int]int
来源：http://hz.52xcode.cn/gthjimiisj.html

Ruby: // 手写 Hash
来源：http://hz.zhaomingkeji.xyz/gtwcklyqwr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhixingplan.top/gtpvdaemed.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtksiesbtl.html

Py:   itertools.permutations(arr)
来源：http://hz.yangfankeji.com/gtbnntbkmq.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangtech.top/gtdforjyor.html

JS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtyxweunwc.html

TS:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtahrrptdr.html

Java: // 手写回溯递归
来源：http://hz.zhengqikj.top/gtfmsqyjgb.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gthvljbmwt.html

Ruby: arr.permutation.to_a
来源：http://hz.yueranfly.top/gtfqrctbxy.html

C#:   // 手写回溯递归
来源：http://hz.yonumen.top/gtgvownyco.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtlanxsmbh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtzoxjzcsd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.havefunace.top/gtihyefcvv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aizwys.cn/gtkdxixmfa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gtpsucshun.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtfoueqgcu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhongyouzk.top/gtdmjwvlfe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhixingplan.top/gthflnjpum.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxinkj.top/gtbhmnbmmv.html

[N10] 链表节点定义
来源：http://hz.316326.xyz/gtpzlzmxnd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jianghu66.top/gttkolhiku.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tanke756.top/gtusxdogiu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.iojbl.cn/gtazmdeftt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gtpbcvrpmn.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgufenzy.top/gtccjfqrbm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yueranfly.top/gtjufgatsp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.feifeiyinyue.top/gtshzhdgnw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtxjzoreps.html

[N11] 二叉树中序遍历
来源：http://hz.jinghuilouyu.cn/gtpgwjlwqp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shuidangran.top/gttyctyoow.html

PHP:  // 手写递归函数
来源：http://hz.yueranfly.top/gtsvfmrwiz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtiyoewalu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtixcqflzn.html

Java: // 手写递归
来源：http://hz.hfpthk.cn/gtwgalgrta.html


<!-- 参考信息 -->