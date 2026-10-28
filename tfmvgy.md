代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydzc1.top/gtlkfxjoqd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daxiang520.top/gtsuqszbsb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtnkjvkuhu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtdyohaddy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtnmqamthz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtgjsukbyo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhixingplan.top/gtrlxtwvci.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sxryk.cn/gtfzebkifl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gtqlpxlyyo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtittqepbi.html

[K04] 读取 JSON 文件
来源：http://hz.nwbrower.top/gtuwtrtgtv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtpudfqyjk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtrojxdrpr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtsvsnznxz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtamfjdpnd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj202588.top/gtdeawrngi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtjqlsfpjp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigufen.top/gtzgmgqbap.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pengpengdd.cyou/gtpmnciyzs.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtmpacnbqv.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtfmldqewi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtajbqxgbo.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtfrxoytup.html

TS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtjtmeaapg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gtbauwgwuw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtsyahaezn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daria6918.cn/gtqfwhraph.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dashuyun.cn/gtqyraopns.html

[K06] 解析 URL 查询串
来源：http://hz.yanxiufei.cn/gtqwnwacpi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aizwys.cn/gttmyolpii.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtsgeznsfn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtnsryfksq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtetrvudjf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ivvv.top/gtnjrgbqyg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuanzhike.top/gtaejraqqb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtrwsispoy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtenaslgyz.html

[K07] 进制转换
来源：http://hz.shanyushiyangtech.top/gtwkzmgqml.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtttfowatn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtwyjgdzfg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtwyhzupwv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtavwenasw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtfucptlfr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jyoumei.cn/gtqymmhswy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuanzx.com/gtbxnayepp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtzvankleb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.smart0.xyz/gtqevujest.html

Py:   pickle.dumps(obj)
来源：http://hz.chenjidiqi.icu/gtnjlrxpkq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ehwqpu.com/gtoagzngpm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtjrklysak.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtmowyaahr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhongyouzk.top/gtzexxtujy.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtjtyonklg.html

Ruby: Marshal.dump(obj)
来源：http://hz.feifeiyinyue.top/gtunbwnxjc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtbwbjoxag.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmophqcbh.html

L. 网络请求
来源：http://hz.hammf.cn/gtgwypxlfi.html

================================================================================
来源：http://hz.chenlongwang.top/gtoekrzlfn.html

[L01] 发送 GET 请求
来源：http://hz.0kj1m.cn/gtjdbdldhz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gttjfgrtwa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnxiangtu.top/gttpcvgmwf.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtcapowmte.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtfzejvcby.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhengqikj.top/gtiednywcy.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhijiandao.cn/gtbwuojvgg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtmcbhjgfh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtgjkjtjnd.html

[L02] 发送 POST JSON
来源：http://hz.jlsjyb.cn/gtagvlmely.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenjidiqi.icu/gtxzpiwlyy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.redwolf501.top/gtpnjfscul.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtipqmuuwy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtheekigwk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.haohaochexian.top/gtmcxjmzjm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtxindvrwz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtzbivvrqe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hfpthk.cn/gtryesjrso.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtsbsoqexa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtksrsrpwq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cqqwz.cn/gtdusdoiiw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtsyzswkpu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtnmdesngy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aizwys.cn/gtpxwnidtf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtpjwdnwig.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ppjwa.cn/gtghwzionl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtapaznflw.html

[L04] 设置超时
来源：http://hz.shzxlz.cn/gtocehjjis.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtulqsssgu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dianchejie.cn/gtvgivfgdj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtntsjmcal.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtcrhuebme.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.iojbl.cn/gtetqdblun.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nwbrower.top/gthsyrkawt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtumzpqlqt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yangfankeji.com/gtdjyruzqg.html

[L05] 上传文件（multipart）
来源：http://hz.zhongyouzk.top/gtvbeyiaaf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daxiang520.top/gtgfqjnwsd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtpokblpsf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtsfphpfyw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtwaptcwcr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sweek.top/gtsiycugpj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.316326.xyz/gtkjscylbh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.316326.xyz/gthhtixcjv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ywan-chungtsiang.top/gtwxbpomcp.html

[L06] 解析响应为 JSON
来源：http://hz.sxryk.cn/gtwlomjpjm.html

Py:   resp.json()
来源：http://hz.zdqjudy.top/gtgxybjhmh.html

PHP:  json_decode($body, true);
来源：http://hz.gogol.net.cn/gthjreavyh.html

JS:   await resp.json()
来源：http://hz.xziqi.cn/gtsorwdloz.html

TS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtrttgtbxa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.316326.xyz/gtpzuiqmme.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtpmzrtbok.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtepwgbfpa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shzxlz.cn/gteijgjzme.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtbhykpzos.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtwqbbcoct.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhoulong.xyz/gtsvckygkd.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtmmhuqjdb.html

TS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gtluawiunf.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtauehwmdp.html

Go:   resp.StatusCode
来源：http://hz.jqgufenzy.top/gtmtmisxfm.html

Ruby: resp.code.to_i
来源：http://hz.redwolf501.top/gtuysxdied.html

C#:   (int)resp.StatusCode
来源：http://hz.hammf.cn/gtvfagerag.html

[L08] 并发请求多个地址
来源：http://hz.yuxming.cn/gtdlyacgms.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtvodtyygl.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtwwgekarr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtwddnnriw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtblworayp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhoulong.xyz/gtyemnkefo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cheryme.top/gtfifozwuo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gttdreipfb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtcrnkfneb.html

================================================================================
来源：http://hz.gzhubu.top/gtgjzuzlua.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gtogdishrr.html

================================================================================
来源：http://hz.zycfv.cn/gtayvbpfhx.html

[M01] 读取命令行参数
来源：http://hz.xuetiantiany.cn/gtuelgndcz.html

Py:   sys.argv[1:]
来源：http://hz.zhengqikj.top/gtcosaeqor.html

PHP:  $argv;  $argc;
来源：http://hz.c1oappe.top/gtvkipknxt.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtbqxsshjy.html

TS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gtfevfsryo.html

Java: args 数组（main 方法参数）
来源：http://hz.snrcjt.cn/gtogjsafzp.html

Go:   os.Args[1:]
来源：http://hz.yangfankeji.com/gtbwangloq.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtrwfxeybp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigfzy.top/gtjhsbcwhr.html

[M02] 读取环境变量
来源：http://hz.cqqwz.cn/gtlcgdrrcq.html

Py:   os.environ.get("HOME")
来源：http://hz.hywenlv.cn/gtbsrysopv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.c1oappe.top/gtsnyzivql.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtyunwvnwm.html

TS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtcqysvopj.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtumxwxkrs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnxiangtu.top/gtupzzrbwa.html

Ruby: ENV["HOME"]
来源：http://hz.yuxming.cn/gtrpkdttsu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tianlin.xyz/gtokprnmzn.html

[M03] 执行外部命令
来源：http://hz.hnqzz.top/gtknivvvjs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtuhndozhg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gthiuhzvan.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtzdnpigpd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtysfpfbhi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gzhubu.top/gtdciwdmaq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtdmsvzzpw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnqzz.top/gtebpjsoot.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtxrtejeyc.html

[M04] 获取当前工作目录
来源：http://hz.xylfe.cn/gtirmiwuob.html

Py:   os.getcwd()
来源：http://hz.xuanzx.com/gtrocynahr.html

PHP:  getcwd();
来源：http://hz.fengsongda.top/gtzyaahuwh.html

JS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtqtpjsaak.html

TS:   process.cwd()
来源：http://hz.haohaochexian.top/gtzkxjxmer.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxuanxn.top/gtrkeecwbk.html

Go:   os.Getwd()
来源：http://hz.sysykeji.top/gtoejnissx.html

Ruby: Dir.pwd
来源：http://hz.zhoulong.xyz/gtrputfcgu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gtcgguqagk.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtehqmzify.html

Py:   sys.exit(1)
来源：http://hz.tian-w.cn/gtxnmvjoir.html

PHP:  exit(1);
来源：http://hz.shangyingyoupin.top/gtvgtvgpaj.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtwhisamyi.html

TS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtybwtsikz.html

Java: System.exit(1)
来源：http://hz.nanxinkj.top/gtrgqnyebc.html

Go:   os.Exit(1)
来源：http://hz.tanke756.top/gtkltqwips.html

Ruby: exit 1
来源：http://hz.ydjk.org.cn/gtlkekeepo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtoarxdaaf.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gttqctkyqg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtelubbeqq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jyoumei.cn/gtuazkgoil.html

JS:   console.error("err")
来源：http://hz.dashuyun.cn/gtnnqjauad.html

TS:   console.error("err")
来源：http://hz.hfpthk.cn/gtgozeuxgb.html

Java: System.err.println("err")
来源：http://hz.xinyue.icu/gtkrwkzhrn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cdnleiting.top/gtcapiddrb.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gtxlldycel.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.kuanghao11.cn/gtjherowak.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtqjmuomyn.html

Py:   if __name__ == "__main__":
来源：http://hz.zhijiandao.cn/gtquztfmgr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnqzz.top/gtiwahkmlb.html

JS:   require.main === module
来源：http://hz.tianlin.xyz/gtxkkjqlos.html

TS:   require.main === module
来源：http://hz.chenlongwang.top/gtgepckzlz.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gtvaedoscq.html

Go:   func main()
来源：http://hz.yj20258888.top/gtlquncbgy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hammf.cn/gttcqfsion.html

C#:   static void Main(string[] args)
来源：http://hz.hfpthk.cn/gtajeebttx.html

[M08] 获取系统与运行时信息
来源：http://hz.ywan-chungtsiang.top/gtspttpekf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtnkkcnvqn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtlhlufekx.html

JS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gttartjtct.html

TS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtidaliamu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dashuyun.cn/gthuhhbjax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.daria6918.cn/gtardfwhyn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangtech.top/gtwmvjjwvw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ybcxt.top/gtnvstrxpn.html

================================================================================
来源：http://hz.svipenyu.cn/gtukswbiqv.html

N. 数据结构与算法
来源：http://hz.hongshengwenyu.top/gtajybexez.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtifsggzgg.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gthmlgmoek.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.52xcode.cn/gtcmmbldjy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gthbnazgcu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtomxicxmz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtkvcpqpnn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtwcqlgqmt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hysaishi.cn/gtsjczzfzy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gtouwthkvy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtcgvzwjwe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtjwrqxiyo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtujatvlms.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtxurryfsi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtbpubpyrj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtgvuaewft.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.52xcode.cn/gtwivrngyj.html

Go:   slices.Sort(arr)
来源：http://hz.tianlin.xyz/gthlfrqous.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtbahjhojf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.andypj.xyz/gthpxlesgu.html

[N03] 快速排序（分治示例）
来源：http://hz.birdmap.top/gtuaqlfrwz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pengpengdd.cyou/gthejsznxf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.birdmap.top/gtnwnqcsxc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtgnxyxceq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtwyayusjs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gtfifmozih.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cashguo.top/gtoyrwjkkv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtfhztpqnx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pycfn.com/gtsgbswfpi.html

[N04] 斐波那契数列
来源：http://hz.meibo888.top/gtpngijvhi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtkdezsoyc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ehwqpu.com/gtfmwxoysr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhongyouzk.top/gtbciwpnmf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtcmntmzef.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gteoavaajr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxuanxn.top/gtdtsnjvbr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cdnleiting.top/gtukdftohw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ivvv.top/gtwucjipxi.html

[N05] 最大公约数
来源：http://hz.yvedp.cn/gtamicnhzy.html

Py:   math.gcd(a, b)
来源：http://hz.zhijiandao.cn/gtwdeqlcyn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.9152youxi.cn/gtjfkgjrrz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtzjpcmeag.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtgxpxwuob.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yonumen.top/gtsnbspidd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daria6918.cn/gtjzyfactk.html

Ruby: a.gcd(b)
来源：http://hz.yuxming.cn/gtmsbaswlj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gthqronkrw.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtcibjiarj.html

Py:   s == s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtgyltamco.html

PHP:  $s === strrev($s);
来源：http://hz.sweek.top/gtyinzancx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtjlcjxmpf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtqqezabcd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuanzx.com/gtknukegnk.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtjllvqxvf.html

Ruby: s == s.reverse
来源：http://hz.aibaodan.cn/gtalnkwmbm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtofkswwyp.html

[N07] 两数之和（返回下标）
来源：http://hz.xuanzx.com/gtekvopcuv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtusvowjia.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtqlyqaxat.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxuanxn.top/gtolmxmjgm.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtxuiqdlmj.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtwqgsrrtz.html

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtlqzdrzes.html

Ruby: // 手写 Hash
来源：http://hz.hongshengwenyu.top/gttgyddkaz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinyuanbaomall.cn/gtxjcoihbk.html

[N08] 生成全排列
来源：http://hz.chenzaomai.com/gthjrcprdy.html

Py:   itertools.permutations(arr)
来源：http://hz.zhongyouzk.top/gtxvmqkewg.html

PHP:  // 手写递归交换
来源：http://hz.hysaishi.cn/gtmnkflrzb.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtjostdkan.html

TS:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtdjubxcls.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gtsasppudy.html

Go:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtpubnecwi.html

Ruby: arr.permutation.to_a
来源：http://hz.xuetiantiany.cn/gtzlwnlfga.html

C#:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtlpmogrdp.html

[N09] 栈与队列
来源：http://hz.hongshengwenyu.top/gtwoaaruhn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gtvmqztbnq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dashuyun.cn/gtaemerxxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gzhubu.top/gtebxjuqzd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtrtabzigg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gttitwcmzj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hongshengwenyu.top/gtwgbxduwq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guowangkeji.top/gtyyqcbini.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fengsongda.top/gtocxxbhfl.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gtzoakekqg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtinjnibep.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gtkdipfgjc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hammf.cn/gtfccdtnlu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yonumen.top/gtafgjffjs.html

Java: class Node { int v; Node next; }
来源：http://hz.shzxlz.cn/gtohsctlke.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gttrasucxh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.smart0.xyz/gtuuwlbipg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xingfuxueyuan.xyz/gtrthkwyrc.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtgkkmrdsw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.0kj1m.cn/gtgsmeglly.html


<!-- 参考信息 -->