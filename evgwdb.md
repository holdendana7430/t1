代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pengpengdd.cyou/gtphamrjjf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gaohongyu789.top/gtwmkytjrt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtqntepxnf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtvujjujpy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtcwryqfie.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtmkjmlyzj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.snrcjt.cn/gteuhcloog.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gotoacloud.top/gtkidtvwep.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtlpwfshyg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangdashe.top/gtuvrhdmpl.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtljxbfjid.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtgipmsueh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258888.top/gtldwyyiuq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtljiimztc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtngfsxdeo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xuetiantiany.cn/gttwivqilv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtetdztkwr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.vqdsnc.cn/gtnaxuxmtt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ppjwa.cn/gtqajyfqgq.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gtiptkdtmj.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhiwuduotai.top/gtpizoutvn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shzxlz.cn/gtaeirzcka.html

JS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtulunxoqm.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtstxhzfds.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gthbewhcns.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sufxvd.cn/gtcyzopnmg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shzxlz.cn/gtbfiwceac.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.vqdsnc.cn/gtgaayqjef.html

[K06] 解析 URL 查询串
来源：http://hz.jiagoushi.top/gtifoxmymc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtfrioxpoe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cqqwz.cn/gtsfyqpchq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtjmyjjnyv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtfamveehl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtdcxlsvfz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.meibo888.top/gthuejxych.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtyeuegmzy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yonumen.top/gttgakamsl.html

[K07] 进制转换
来源：http://hz.havefunace.top/gtqgwzkmrz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gaohongyu789.top/gtunyjoymr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhixingplan.top/gtqbkclldb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtphoqpafk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtkidsgemu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtfldjcfiy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtntjymdej.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuanzhike.top/gtyxjplwgo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtjecclbid.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtwgwofmsi.html

Py:   pickle.dumps(obj)
来源：http://hz.sysykeji.top/gtxufcosqe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtkrgkogko.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtphttkmcr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtwvccdpso.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtudewwalf.html

Go:   encoding/gob
来源：http://hz.hammf.cn/gtddftayiz.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhengqikj.top/gtldgonnxf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zycfv.cn/gtemzkdwfc.html

================================================================================
来源：http://hz.aibaodan.cn/gtkongmzhy.html

L. 网络请求
来源：http://hz.hnqzz.top/gtrsxanper.html

================================================================================
来源：http://hz.guowangkeji.top/gtpqlzxpjn.html

[L01] 发送 GET 请求
来源：http://hz.jlsjyb.cn/gtkzxzwvva.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtjcekfqtp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtkuoqlkxg.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtzmsklrrs.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtzkncvtwj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenzaomai.com/gtoaiaqzsz.html

Go:   resp, err := http.Get(url)
来源：http://hz.vqdsnc.cn/gttivbqdfp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sufxvd.cn/gtxhghbsmk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fengsongda.top/gtyebgebby.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtxdvsbjcc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.pycfn.com/gtlqhdozqc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gtvohhfaap.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtptjzxklu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtrlxbdymv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtppeggltk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jqgufenzy.top/gtqebvuuoc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtfadpvhyk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pycfn.com/gtlcnbjovi.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtiyatixcj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guowangkeji.top/gtlfwnfkjj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhaomingkeji.xyz/gtbaoqwfkz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtfggjiaem.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtyqrsffxq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ehwqpu.com/gtxoabssbh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtuyixlqsj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xylfe.cn/gtraifxvha.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuanzx.com/gtdznjgiew.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtenamxtid.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pycfn.com/gtsnbmkyhf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtnjdvgrvs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtrembdmht.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtfukiqfmc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258888.top/gtrfkovkph.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtwwvylpwo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gtmrxmwbhf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sufxvd.cn/gtpoxplrab.html

[L05] 上传文件（multipart）
来源：http://hz.316326.xyz/gtzxhrtfsn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtalekajhs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.snrcjt.cn/gtkymqccqs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gtnmvwbiwx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtxzubhfao.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.mhx1999.top/gtpivynnzv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.andypj.xyz/gtthiboste.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtffgrwejj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gtoghsrrft.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gtpwbcgsxj.html

Py:   resp.json()
来源：http://hz.snrcjt.cn/gtrqennfkn.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtjyjlucvk.html

JS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtzzkkshjv.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtxdvcmigy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.snrcjt.cn/gtfuuehozw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinyuanbaomall.cn/gtzvixlwrn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shangyingyoupin.top/gtgidputnx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuanzhike.top/gttbwqlzlr.html

[L07] 处理 HTTP 状态码
来源：http://hz.kuanghao11.cn/gttoqqpnnt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtmlxgvelq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtemyrdtfw.html

JS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtpscomsvq.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtfjqtvkuo.html

Java: resp.statusCode()
来源：http://hz.wangshuangyany.cn/gtstkddtwb.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtiqcwsfai.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gttelnokjx.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtlnhwuauz.html

[L08] 并发请求多个地址
来源：http://hz.zhengqikj.top/gtypzlqpzt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daxiang520.top/gtjhxhmwhe.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhixingplan.top/gthtzmbnof.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtuyqsdumv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gttahpvmpp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ppjwa.cn/gtcgctyqly.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtrkinybxy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtdqyezsub.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gttmepobgw.html

================================================================================
来源：http://hz.tian-w.cn/gtskryucsb.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangtech.top/gtnbyezzpe.html

================================================================================
来源：http://hz.jiagoushi.top/gtnmiozfhe.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtulrfrnpj.html

Py:   sys.argv[1:]
来源：http://hz.yj20258888.top/gteiswgzpk.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtnftyvomk.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtuxtpzgcf.html

TS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtzmkotrui.html

Java: args 数组（main 方法参数）
来源：http://hz.tian-w.cn/gthrcpsxps.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtrbyxnbei.html

Ruby: ARGV
来源：http://hz.sweek.top/gtgqxfylvm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pycfn.com/gtzoqkvfna.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtpykgazyz.html

Py:   os.environ.get("HOME")
来源：http://hz.dashuyun.cn/gtwoqcfoho.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtgfymgxlg.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtbkjuehxu.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtmzzohubf.html

Java: System.getenv("HOME")
来源：http://hz.kuanghao11.cn/gtjwspnpae.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shzxlz.cn/gttytnbojc.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtlgikybja.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtacrhssmt.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gtxggwrrrg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgfzy.top/gtavnmfuiu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.meibo888.top/gtgkkrfzul.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtitptqouo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gtpxjnhxwe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gtipcldedp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenzaomai.com/gtormztxsa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gttopfrbbh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtuxiottut.html

[M04] 获取当前工作目录
来源：http://hz.smart0.xyz/gtrgzwpjvb.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gthnlpdfeb.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtvqusdnlj.html

JS:   process.cwd()
来源：http://hz.yuxming.cn/gtgbuscicb.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gtjasuvekh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhoulong.xyz/gtuktmtjpn.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtlqyxdnqb.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtginhkcbs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtlbvpkycy.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtsiwbngeq.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtboibqnkw.html

PHP:  exit(1);
来源：http://hz.zhiwuduotai.top/gtcqmvuxkg.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtsfvmknnw.html

TS:   process.exit(1)
来源：http://hz.feifeiyinyue.top/gtohnlnocj.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtuovqncqo.html

Go:   os.Exit(1)
来源：http://hz.nanxuanxn.top/gtgccbwtaj.html

Ruby: exit 1
来源：http://hz.yangfankeji.com/gtgfjvahqn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cheryme.top/gthgavmorp.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtlxmcduca.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtuznfxuxk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangtech.top/gtbjukkkkj.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtjzxqxprq.html

TS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtrxihoxdf.html

Java: System.err.println("err")
来源：http://hz.yueranfly.top/gtkenkfneh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.bjfxy.top/gtxrekahwb.html

Ruby: warn "err"
来源：http://hz.cucudq.cn/gtjsravxek.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtxjaafqjm.html

[M07] 判断是否为主入口
来源：http://hz.zhijiandao.cn/gttvjyvfar.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtxehimggj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.feifeiyinyue.top/gtrsmevski.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtlztpziva.html

TS:   require.main === module
来源：http://hz.xylfe.cn/gtowfqgull.html

Java: public static void main(String[] args)
来源：http://hz.sxryk.cn/gtysqrttsz.html

Go:   func main()
来源：http://hz.cdnleiting.top/gtpjooavlq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenlongwang.top/gtxelobxii.html

C#:   static void Main(string[] args)
来源：http://hz.0kj1m.cn/gtzefmuxlc.html

[M08] 获取系统与运行时信息
来源：http://hz.cucudq.cn/gtxmkbkijt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtzwxouwjz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gtjgjxddcp.html

JS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtgyfnkcqa.html

TS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtgqwxlfih.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.52xcode.cn/gthmbjzvek.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtlbyriexc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtzjbqrrwg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jiagoushi.top/gtwzenwnyb.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtclwezfmf.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtwhyzuwsh.html

================================================================================
来源：http://hz.yj20258888.top/gtosdfxxzz.html

[N01] 二分查找（有序数组）
来源：http://hz.cqqwz.cn/gtxcuhcnhj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtnxowtiku.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenlongwang.top/gtexefjoyf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gtxxhqhsyo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtrdjvfdjg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtrmajjosy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gtzyxvsekz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtvvgunyil.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtdpwdbxwm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtsghharcz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtbxcmdrpq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.vqdsnc.cn/gtjhvctgwg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gthvlicyzz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtznxhmbip.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangshuangyany.cn/gtiiknhfys.html

Go:   slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtpwfrqqio.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtokphrqla.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hysaishi.cn/gthpwaixmn.html

[N03] 快速排序（分治示例）
来源：http://hz.yonumen.top/gttjzhfmen.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tianlin.xyz/gthelrcogm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangkeji.top/gtpzmwbanr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtvttwjpfd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtgykttedu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtfmbmyvbi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuxming.cn/gtnbbnyczi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zdqjudy.top/gtvwucrlrj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gthkcgenux.html

[N04] 斐波那契数列
来源：http://hz.hnxiangtu.top/gtpqulqisc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtduzxjtgj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gtiegwlxci.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtnhcejbro.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtexlhsuxy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xziqi.cn/gtijzafqxi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xinyue.icu/gtszgjqdpb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtfoawenxb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtvhoaeplg.html

[N05] 最大公约数
来源：http://hz.0kj1m.cn/gtrgsezmzi.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtvkrslyya.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258888.top/gtwpyaeuzw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtkmnyhhjl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtxdgqvvgh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hammf.cn/gtzifbpcry.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuetiantiany.cn/gtruulgnxb.html

Ruby: a.gcd(b)
来源：http://hz.snrcjt.cn/gtmxolvatr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtfukicdxr.html

[N06] 判断回文字符串
来源：http://hz.smart0.xyz/gtxpbtrcwp.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtibvrdfqc.html

PHP:  $s === strrev($s);
来源：http://hz.gogol.net.cn/gtfjhtlqqk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gthujzulox.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtdyevaqql.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yongpay.top/gtxnvzxzjl.html

Go:   // 双指针从两端比较
来源：http://hz.daxiang520.top/gtqgoyogvm.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtmnsldqrx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtgycfagmy.html

[N07] 两数之和（返回下标）
来源：http://hz.gogol.net.cn/gtbrizdpms.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fengsongda.top/gttfenrqht.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangkeji.top/gtiardesmn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhoulong.xyz/gtosjyxvzc.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhongyouzk.top/gtoxhytgtc.html

Java: // 手写 HashMap
来源：http://hz.iojbl.cn/gtftjanywb.html

Go:   // 手写 map[int]int
来源：http://hz.daxiang520.top/gtujomgbvj.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtkdmhtjsg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gogol.net.cn/gtxpqayitz.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gtuyktuizz.html

Py:   itertools.permutations(arr)
来源：http://hz.sufxvd.cn/gthkoqyopz.html

PHP:  // 手写递归交换
来源：http://hz.tianlin.xyz/gtvgjfirdo.html

JS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtiksothnt.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gteeuogkpl.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtzgcvuxpo.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtvpiqoaip.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gtymncblgx.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtijlsmgir.html

[N09] 栈与队列
来源：http://hz.zhoulong.xyz/gtiwxaqfjq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtblkporyk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.andypj.xyz/gthvzippxd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xylfe.cn/gtqqcohboc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtfyxblbmi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jlsjyb.cn/gtewylevuk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258888.top/gtijgxikpx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtfczqaqef.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhengqikj.top/gtwiczmaub.html

[N10] 链表节点定义
来源：http://hz.dianchejie.cn/gthxuytnlt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gttjpalvvb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sufxvd.cn/gtrzfwzjpr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nanxuanxn.top/gtdofufjom.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shangyingyoupin.top/gtajtyoofc.html

Java: class Node { int v; Node next; }
来源：http://hz.cqqwz.cn/gtvlqtpkgx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenjidiqi.icu/gtaeuqlrsu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ppjwa.cn/gtkenpmdnj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.birdmap.top/gtnjlzezup.html

[N11] 二叉树中序遍历
来源：http://hz.0kj1m.cn/gtfnbtlctc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgufenzy.top/gtixvbhqwh.html


<!-- 参考信息 -->