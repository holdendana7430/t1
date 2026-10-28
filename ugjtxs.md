代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtiogggpqo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtxkeequov.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guowangkeji.top/gtayquctta.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gotoacloud.top/gtqfyftwdh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gttzuxdlru.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtidaedzne.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtxpgacrjk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.52xcode.cn/gtzurzmylw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.meibo888.top/gtwkyramdq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtpifrvtfd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtgbjgknlq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cqqwz.cn/gtvcsvtnfh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtsrvreeuf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jianghu66.top/gtuwpwskkf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yueranfly.top/gtnndifqza.html

[K05] 深拷贝对象
来源：http://hz.tianlin.xyz/gtdgbibyxv.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangshuangyany.cn/gtihsxvfeo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gtmxoosazc.html

JS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtazakgqxt.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtjcauzner.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtbxllgjmv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gtlmujiuiq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtnjyumimv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gttmccipcf.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gtwfjjzgdj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zycfv.cn/gtxswrsqvy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtlcdbtrvv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtotwahywg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gtzwoufuia.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.smart0.xyz/gtrwstqudm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtqjcrippv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cashguo.top/gtrzssgfru.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtltlhjhgx.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtajdgbxcc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenlongwang.top/gthqsakbwk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gtjdaokzvl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtfvhvvymy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtrmxidovt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtfcrnvctm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtdjzpsqad.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shangyingyoupin.top/gtvyffhttr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.birdmap.top/gtnsxiruvb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gtumrcanir.html

Py:   pickle.dumps(obj)
来源：http://hz.zhiwuduotai.top/gtdotphosw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtupnbfdri.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtliltspwq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtfyeooikn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shzxlz.cn/gtbrvrfdhi.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtkuqrqgts.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuetiantiany.cn/gtyoxomyvm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtnfimeioe.html

================================================================================
来源：http://hz.9152youxi.cn/gtmuyysabe.html

L. 网络请求
来源：http://hz.ybcxt.top/gtikljdcxk.html

================================================================================
来源：http://hz.jinqigufen.top/gtvestkgmv.html

[L01] 发送 GET 请求
来源：http://hz.dashuyun.cn/gtxapvwpny.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aizwys.cn/gtkojwkulr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.smart0.xyz/gttbvzonys.html

JS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtstjkmuet.html

TS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtvockcrnb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.svipenyu.cn/gtrupugwcj.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtpkifviex.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuanzhike.top/gtwirqrexi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtmycvcexe.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gtljugxzwr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtjbdorajj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sysykeji.top/gteojwcjae.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtvdqhqyhw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtkoosbinc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.bjfxy.top/gtucvtxbgi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtheakphdz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ehwqpu.com/gtjhmlkpql.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cheryme.top/gtjdkgutcg.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gteukltjrc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtgmpleadk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtjgzbpzka.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtenvlvzcs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtuanxarjd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gtwhzfdgmy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtlezmlneg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.redwolf501.top/gtqcyvcopg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sysykeji.top/gtfdcyseoa.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtlbxkbybx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhoulong.xyz/gtgbcswmrt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gtdoobbgns.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtetpjjpwo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtyancapxt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xinyue.icu/gtyybbjvpu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.svipenyu.cn/gtiwwcqokb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zycfv.cn/gtxqmblxlv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtbwerfsui.html

[L05] 上传文件（multipart）
来源：http://hz.ehwqpu.com/gtoiezwkrs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daxiang520.top/gtpskqzjld.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sweek.top/gtetwrtnzr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtrfdzlxxw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtzuefqtmv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gthbrpieky.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cqqwz.cn/gtjqnfwwyv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigufen.top/gtwnflfqwl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xziqi.cn/gtzdtxnboi.html

[L06] 解析响应为 JSON
来源：http://hz.hysaishi.cn/gtpnjonoqs.html

Py:   resp.json()
来源：http://hz.jinghuilouyu.cn/gtwjiqvtyq.html

PHP:  json_decode($body, true);
来源：http://hz.cucudq.cn/gtgqpogtna.html

JS:   await resp.json()
来源：http://hz.gotoacloud.top/gtngybsabx.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtxrtzffrx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gttqkeglpm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtileqrhbg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.haohaochexian.top/gtvarvgyjc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtdvfowfta.html

[L07] 处理 HTTP 状态码
来源：http://hz.zycfv.cn/gteachfadh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuxming.cn/gtpaxsijpj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangshuangyany.cn/gtmfnlywid.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtbbkizugh.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gthlvkiaja.html

Java: resp.statusCode()
来源：http://hz.xylfe.cn/gtexdweusp.html

Go:   resp.StatusCode
来源：http://hz.zhengqikj.top/gtymdckquv.html

Ruby: resp.code.to_i
来源：http://hz.ydzc1.top/gtlryisrzj.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtxlgmbilk.html

[L08] 并发请求多个地址
来源：http://hz.zhongyouzk.top/gttntxhmra.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gtcjfhrjqx.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gttkcbcozb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtuxspextu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtojslumqh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yongpay.top/gtpciedswx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gthqtfqnhy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yanxiufei.cn/gtjgtgpnhs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xylfe.cn/gtdkjfipbk.html

================================================================================
来源：http://hz.havefunace.top/gteiakabny.html

M. 命令行 / 进程 / 环境
来源：http://hz.9152youxi.cn/gtslakyerq.html

================================================================================
来源：http://hz.snrcjt.cn/gtoygnayqa.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtjocyerdq.html

Py:   sys.argv[1:]
来源：http://hz.zhongyouzk.top/gtqkpirdnr.html

PHP:  $argv;  $argc;
来源：http://hz.andypj.xyz/gtrcornpmv.html

JS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtclsjrccw.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtkagbdsrx.html

Java: args 数组（main 方法参数）
来源：http://hz.316326.xyz/gtbiwezxjl.html

Go:   os.Args[1:]
来源：http://hz.hfpthk.cn/gtfdiaowdp.html

Ruby: ARGV
来源：http://hz.hywenlv.cn/gtpxbshmvh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daxiang520.top/gtpfqgztty.html

[M02] 读取环境变量
来源：http://hz.chenzaomai.com/gtoedckkay.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gtsgdtuead.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.meibo888.top/gtpwwqxjpc.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtispeqbay.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtazikwxzo.html

Java: System.getenv("HOME")
来源：http://hz.yvedp.cn/gtzswbkrwx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.svipenyu.cn/gtspqamats.html

Ruby: ENV["HOME"]
来源：http://hz.xylfe.cn/gtndmcoxuj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pycfn.com/gtdelzbfjh.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtvxvafujm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.havefunace.top/gtgfokjvfa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ywan-chungtsiang.top/gtbrthizgf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtatkksbgy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtvasegzju.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydjk.org.cn/gtfppkszaz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shzxlz.cn/gtobaiyjoi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtigqatswp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenjidiqi.icu/gtbhgfdoon.html

[M04] 获取当前工作目录
来源：http://hz.tianlin.xyz/gtrqymdils.html

Py:   os.getcwd()
来源：http://hz.zdqjudy.top/gtluidgeyn.html

PHP:  getcwd();
来源：http://hz.tianlin.xyz/gtlablilfj.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtdifitlbl.html

TS:   process.cwd()
来源：http://hz.jinqigufen.top/gtqsimdspc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtovhubroz.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtogrcgiob.html

Ruby: Dir.pwd
来源：http://hz.gogol.net.cn/gtldbgmrcl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xinyue.icu/gtaakfehxt.html

[M05] 设置退出码
来源：http://hz.hnxiangtu.top/gtwzakrywf.html

Py:   sys.exit(1)
来源：http://hz.zdqjudy.top/gtxgzkhoup.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gtnpsavhci.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtvamjgejy.html

TS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtazamgnbc.html

Java: System.exit(1)
来源：http://hz.quarkkingdee.top/gtihrezxcw.html

Go:   os.Exit(1)
来源：http://hz.jyoumei.cn/gtjwfdicgn.html

Ruby: exit 1
来源：http://hz.c1oappe.top/gtxzwcregd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtekkvdrbq.html

[M06] 向标准错误输出
来源：http://hz.haohaochexian.top/gtcqkaraob.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shzxlz.cn/gtvbrfktly.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtwfvoeotk.html

JS:   console.error("err")
来源：http://hz.tanke756.top/gtxhcysgxx.html

TS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtaqjucyfa.html

Java: System.err.println("err")
来源：http://hz.havefunace.top/gtwqflfjih.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtgemozipb.html

Ruby: warn "err"
来源：http://hz.zhijiandao.cn/gtazuafuxz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhiwuduotai.top/gtwzrbxsiw.html

[M07] 判断是否为主入口
来源：http://hz.cashguo.top/gtcvkbvody.html

Py:   if __name__ == "__main__":
来源：http://hz.sweek.top/gtkqkffzgi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.havefunace.top/gtugujplkk.html

JS:   require.main === module
来源：http://hz.ppjwa.cn/gtsibcvwdz.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtgotmclhg.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtbafcdlti.html

Go:   func main()
来源：http://hz.kuanghao11.cn/gtibsebokf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxuanxn.top/gtqqmiwxzp.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtkfbzchgy.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gtvxpncgjt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangdashe.top/gtxuoqkfsh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtiposhuvh.html

JS:   process.platform;  process.version
来源：http://hz.wangshuangyany.cn/gtrastbquu.html

TS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtrhmebqwx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtddgpzoei.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj202588.top/gtxzdnqedr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnxiangtu.top/gtsmbigxiz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenjidiqi.icu/gtqnrlieng.html

================================================================================
来源：http://hz.chenzaomai.com/gtoxobhqxr.html

N. 数据结构与算法
来源：http://hz.dashuyun.cn/gtcblmlofb.html

================================================================================
来源：http://hz.xuanzx.com/gthuoubaqf.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gtnxoskswz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtlrhxapke.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gteqxlxsyu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gttabafeid.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtsnocoglr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtaresgiub.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangshuangyany.cn/gtlgmjrodt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgfzy.top/gtrcjqoawd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtxvtryuyo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cheryme.top/gtmhpmtjgt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtqjadhyhq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtzrqwqirn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtdfewzyca.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtbhhswfhs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhiwuduotai.top/gtxwrauhvi.html

Go:   slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtynfkdvyu.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtvlflsurr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtcbbqnjgt.html

[N03] 快速排序（分治示例）
来源：http://hz.yanxiufei.cn/gtklagctew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.haohaochexian.top/gtmomkirik.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtltxfyxyd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtphvomtjy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sysykeji.top/gtqfefqzce.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgfzy.top/gtvhelzxqj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yueranfly.top/gtuejpprev.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtcyrhbwpz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gtxugsbdem.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtvqcwennc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.aizwys.cn/gtdknanklt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gotoacloud.top/gtkpqazytf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtvvuywciv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtuielmzou.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhongyouzk.top/gttoijpvtw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gzhubu.top/gteazqfzfr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gteluufbmm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.andypj.xyz/gtwdctqsez.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtmxypkfco.html

Py:   math.gcd(a, b)
来源：http://hz.yuanzhike.top/gtiyynqcff.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jqgfzy.top/gtqqjilzyn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtiwbejkjs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtkwblzgwp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigufen.top/gtplzrzsla.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dashuyun.cn/gtwvnznrlv.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtswbcslve.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yongpay.top/gtutycrpls.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtkzwvcxyv.html

Py:   s == s[::-1]
来源：http://hz.iojbl.cn/gtjbvpiuwp.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gttctxybev.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtzvhlrigy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtcnrxyggy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxinkj.top/gthizthllf.html

Go:   // 双指针从两端比较
来源：http://hz.tanke756.top/gtfzhqzlcy.html

Ruby: s == s.reverse
来源：http://hz.hnqzz.top/gtbprnurbf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtidevcdwt.html

[N07] 两数之和（返回下标）
来源：http://hz.hammf.cn/gtwqpbrtbz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.redwolf501.top/gtxwrpyawl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gogol.net.cn/gtogeggnol.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhijiandao.cn/gtuzeznili.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangdashe.top/gtzsjqeexc.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gtcznvmsuq.html

Go:   // 手写 map[int]int
来源：http://hz.shzxlz.cn/gtrczkbzqq.html

Ruby: // 手写 Hash
来源：http://hz.pycfn.com/gtwhmrepzq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.52xcode.cn/gtenubqtwf.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gtizanbfax.html

Py:   itertools.permutations(arr)
来源：http://hz.ydjk.org.cn/gtnfcejvfr.html

PHP:  // 手写递归交换
来源：http://hz.wangshuangyany.cn/gteidjgduv.html

JS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gttzplbrau.html

TS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtcjnzthit.html

Java: // 手写回溯递归
来源：http://hz.aizwys.cn/gtuuyiarta.html

Go:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtoupbmxdf.html

Ruby: arr.permutation.to_a
来源：http://hz.ydzc1.top/gtflpkdydd.html

C#:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtwnglbnix.html

[N09] 栈与队列
来源：http://hz.yangfankeji.com/gtfosajmlg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aizwys.cn/gtveltolxu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ivvv.top/gtbrreqjre.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtvwzxeauu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtjpmmngte.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxuanxn.top/gtulwlgcdx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhongyouzk.top/gtnebwukdz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ehwqpu.com/gtrmxzirkf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhoulong.xyz/gteoqcymkv.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gtubrdaqje.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gzhubu.top/gttfwpbeku.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cheryme.top/gtlxoypbdt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.redwolf501.top/gtqokxykcr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.kuanghao11.cn/gtfavyfuyc.html

Java: class Node { int v; Node next; }
来源：http://hz.haohaochexian.top/gtwghgmljw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yonumen.top/gtaejkgrsa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxinkj.top/gtdugleexo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhaomingkeji.xyz/gtmfmcxgpu.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtmtyolboe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtmaeruwvw.html

PHP:  // 手写递归函数
来源：http://hz.havefunace.top/gtzwxroqdu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtcsycgpfl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtipzadder.html

Java: // 手写递归
来源：http://hz.wangshuangyany.cn/gtziaxwusz.html


<!-- 参考信息 -->