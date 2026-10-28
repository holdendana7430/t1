代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yueranfly.top/gtghauqnxe.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtoemktzqm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.birdmap.top/gtrmyitlkn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtbhhxjrrw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gttrfchgrd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtggcywxvz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ybcxt.top/gtdzerqdts.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gteudbcwnx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.0kj1m.cn/gtitdxrlpm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gtlmuawbaq.html

[K04] 读取 JSON 文件
来源：http://hz.hnqzz.top/gtxwetttnt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jianghu66.top/gtfghfzyyh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hysaishi.cn/gtxkyaddlz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtkypwsnbb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtsetmzark.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.mhx1999.top/gtzcvfjfuv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtzkjiwfas.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuanzx.com/gtvvvhllao.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtokskzpcb.html

[K05] 深拷贝对象
来源：http://hz.yuanzhike.top/gtluwdoykw.html

Py:   copy.deepcopy(obj)
来源：http://hz.jyoumei.cn/gtaueaotea.html

PHP:  unserialize(serialize($obj));
来源：http://hz.9152youxi.cn/gtofrjwjoy.html

JS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtamwjfioq.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtlpfyxury.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtukrdlugs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtczkxbxqi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtrugfzbai.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtszuyvfch.html

[K06] 解析 URL 查询串
来源：http://hz.zhaomingkeji.xyz/gtzjlodzdr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ehwqpu.com/gthglxecdf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ybcxt.top/gtbixeygrd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtdppgenqk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtjqityszf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gthndzgnww.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtjwbwhiar.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtmwyecrgx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gtvujzofyd.html

[K07] 进制转换
来源：http://hz.aizwys.cn/gtuhjgalro.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtoguccxdw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ehwqpu.com/gthgfkzjgj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtkwkeynjj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gttxzybosi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ivvv.top/gtukgqxgic.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tanke756.top/gtaqthdimm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhiwuduotai.top/gtlmieskvp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.snrcjt.cn/gtxpdbpoxl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gtmtsjcmlm.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gtwmikzbdb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yongpay.top/gtldotyqek.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gthvbueoyx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtxfbqcypy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtzavgbaim.html

Go:   encoding/gob
来源：http://hz.ywan-chungtsiang.top/gtdjodknrd.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangkeji.top/gtoqvbfeew.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zycfv.cn/gtsbbrmthw.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtnqlpvpag.html

L. 网络请求
来源：http://hz.havefunace.top/gtfakxlhod.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqwflbjod.html

[L01] 发送 GET 请求
来源：http://hz.aizwys.cn/gtetbphyyt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gthlaqrvlc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtororhlpi.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtqvruodju.html

TS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtkdrwhluy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtvtttqyej.html

Go:   resp, err := http.Get(url)
来源：http://hz.hammf.cn/gtlhesrhyv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yongpay.top/gtyclkbqhe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtamnyrxxz.html

[L02] 发送 POST JSON
来源：http://hz.quarkkingdee.top/gtfkkhhnfh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.havefunace.top/gtdykhgzdf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gttfdxqwzj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtakzynahq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtrijcjdat.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtoglrorjh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtvklfzzxf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.andypj.xyz/gtzyvgrros.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hywenlv.cn/gtuqierksw.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtazgvsnzu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtmabagzfx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.9152youxi.cn/gtavfwjnko.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gttclmwvch.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtjxoumfwy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yanxiufei.cn/gttaqkmtgb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtzjrjunpr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dianchejie.cn/gthzfdehzs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gtzououena.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gtexfblcui.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gtjijyasog.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gttbpvovio.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gtzetcfsee.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gtrbwtzdzm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangshuangyany.cn/gtwxiqappu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuanzx.com/gtkznwyhlo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenjidiqi.icu/gtivhawoha.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hywenlv.cn/gtojvouhup.html

[L05] 上传文件（multipart）
来源：http://hz.ehwqpu.com/gtkzmlbojt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuanzx.com/gtuskotgiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.bjfxy.top/gtkgdkymld.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gttzggnkrf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtfpientif.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtbtnrwjay.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxinkj.top/gtnddpzdjb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cheryme.top/gtvfljjvdp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dashuyun.cn/gtaeydwnuv.html

[L06] 解析响应为 JSON
来源：http://hz.tianlin.xyz/gtqmhkvgzm.html

Py:   resp.json()
来源：http://hz.xuetiantiany.cn/gtkwzuyawq.html

PHP:  json_decode($body, true);
来源：http://hz.ehwqpu.com/gtnhhnnhaf.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtyvqwaddl.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtsojlqgyt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangdashe.top/gtjweeived.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhengqikj.top/gtsrpdnstw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhaomingkeji.xyz/gtvoelfozm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.redwolf501.top/gtogrwbapb.html

[L07] 处理 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtidtclcbl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtdspsvogf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnxiangtu.top/gtdmxrkbmb.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtbuaqikle.html

TS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtbdnxbczj.html

Java: resp.statusCode()
来源：http://hz.wangdashe.top/gtutolrclv.html

Go:   resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtooviilkh.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gtetlhaqzl.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gtxzwpywno.html

[L08] 并发请求多个地址
来源：http://hz.gogol.net.cn/gthnttisif.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gogol.net.cn/gtfcgiosfd.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtjegidvss.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtzodftuzq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtbvbpgitj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydzc1.top/gtmrrutxgv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtksxpntqm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258888.top/gtajsdwdcw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sufxvd.cn/gtcumqxmqt.html

================================================================================
来源：http://hz.nanxuanxn.top/gtectfdszc.html

M. 命令行 / 进程 / 环境
来源：http://hz.quarkkingdee.top/gtpdlkovdw.html

================================================================================
来源：http://hz.ehwqpu.com/gthisdsirk.html

[M01] 读取命令行参数
来源：http://hz.redwolf501.top/gtlpakgstm.html

Py:   sys.argv[1:]
来源：http://hz.chenjidiqi.icu/gteocndeta.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtlnzvwfsc.html

JS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtusxiisfu.html

TS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtpbheqslu.html

Java: args 数组（main 方法参数）
来源：http://hz.gzhubu.top/gthbzcojqi.html

Go:   os.Args[1:]
来源：http://hz.shuidangran.top/gtdmkgbkyi.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtyqjzzetw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guannengcc.top/gttpdqcxyv.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtjsujhenb.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gturdzqywl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigfzy.top/gtqvxwdjlo.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtkbxnydts.html

TS:   process.env.HOME
来源：http://hz.yongpay.top/gtwcgtnnly.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtcitjuihu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtckykqlll.html

Ruby: ENV["HOME"]
来源：http://hz.hywenlv.cn/gtwwqiztik.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtgukrtzug.html

[M03] 执行外部命令
来源：http://hz.316326.xyz/gtxoquagvw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangshuangyany.cn/gtwfhzxefz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dashuyun.cn/gtznsmpzcs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtmzhaxaod.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtxssfoeis.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangdashe.top/gtxxqqoemz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtazsrjuqc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pycfn.com/gthtckyjod.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtqpzbocbz.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangtech.top/gtntpnbbod.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtkfqnxdhe.html

PHP:  getcwd();
来源：http://hz.xziqi.cn/gtsegehmrn.html

JS:   process.cwd()
来源：http://hz.birdmap.top/gttbrrfzqw.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtscknvjjh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.havefunace.top/gtmlwrmumg.html

Go:   os.Getwd()
来源：http://hz.sweek.top/gteommmoqp.html

Ruby: Dir.pwd
来源：http://hz.zycfv.cn/gtywmxazyk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tianlin.xyz/gtmynincqi.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtukbhnqeo.html

Py:   sys.exit(1)
来源：http://hz.iojbl.cn/gtxlocccfg.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtijbydmrw.html

JS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtyaqfftkb.html

TS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtyzpxfxjv.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gtxuxbtkfd.html

Go:   os.Exit(1)
来源：http://hz.zhongyouzk.top/gtkzcxzgve.html

Ruby: exit 1
来源：http://hz.cucudq.cn/gtsengbufq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guowangkeji.top/gtscrnqpxh.html

[M06] 向标准错误输出
来源：http://hz.jianghu66.top/gtpmnpmxbi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtdhnqiqgw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtezwzgihv.html

JS:   console.error("err")
来源：http://hz.jqgfzy.top/gtdzxspavx.html

TS:   console.error("err")
来源：http://hz.yueranfly.top/gtyiqapchu.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtunghzncx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhixingplan.top/gtexhdxmhm.html

Ruby: warn "err"
来源：http://hz.nanxinkj.top/gtvkkbrqut.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nwbrower.top/gtzrbkunow.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtwzaiygru.html

Py:   if __name__ == "__main__":
来源：http://hz.zhoulong.xyz/gttuxvtkvw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtqzodwjdd.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtwboiomdq.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtwofddazk.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangtech.top/gthkkwmydj.html

Go:   func main()
来源：http://hz.xziqi.cn/gtudtzgzro.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hammf.cn/gtcvybjkpa.html

C#:   static void Main(string[] args)
来源：http://hz.sufxvd.cn/gtzxcqiryl.html

[M08] 获取系统与运行时信息
来源：http://hz.haohaochexian.top/gtymlevgts.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yongpay.top/gtwdtjrhhk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtelgaadtg.html

JS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtzelrvqez.html

TS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtptsfavdh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.haohaochexian.top/gtfoxlktod.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtysvbgbhu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pycfn.com/gtaqfidkvh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gthhxzabwr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gttbhzjmcx.html

N. 数据结构与算法
来源：http://hz.ivvv.top/gtxmddkqzz.html

================================================================================
来源：http://hz.ivvv.top/gtinwlxnyp.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtoqhawnby.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ehwqpu.com/gtsmnbmawe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtbjogwzpp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtahthasob.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtacugyjbo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aizwys.cn/gtomjboreo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ehwqpu.com/gtsqjavybp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtazlrelhw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtuomhkqxt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cheryme.top/gtvxuzcris.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtrtaqycer.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dianchejie.cn/gttegapygz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gttieneqae.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtkopatpra.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hfpthk.cn/gtlegnnrwr.html

Go:   slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtlrrqgaxq.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtupcdlmvn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tianlin.xyz/gtknbfcdax.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtkvmheroh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shuidangran.top/gtrkjgutto.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yangfankeji.com/gtombcelmc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtowwrraxy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gttvkxhqlf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aizwys.cn/gtoldfkluq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtfddyiair.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gtmavkqkvk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gtijqoytya.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtciafnexd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jyoumei.cn/gtjjcadipi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gttcctbjyh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtowxzqfqh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtyqwseavj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtfoeketxk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinghuilouyu.cn/gtijapyibg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtgxfuplnt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenlongwang.top/gtadepgjms.html

[N05] 最大公约数
来源：http://hz.ppjwa.cn/gtimjfvixm.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtlhhvpijb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.0kj1m.cn/gtudaynwwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtyiavalsb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtpcdnkzol.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aibaodan.cn/gtrumwdizw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtvtukfxyj.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gtkopoekmg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hongshengwenyu.top/gtyocrngus.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtzdgshbkc.html

Py:   s == s[::-1]
来源：http://hz.yj202588.top/gtnxjajwgc.html

PHP:  $s === strrev($s);
来源：http://hz.c1oappe.top/gtudlcyiul.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtlucnsops.html

TS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtuntbbycq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gtdybqayor.html

Go:   // 双指针从两端比较
来源：http://hz.jianghu66.top/gtqaimzgjd.html

Ruby: s == s.reverse
来源：http://hz.c1oappe.top/gtuwzaguks.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtscxvnzht.html

[N07] 两数之和（返回下标）
来源：http://hz.xziqi.cn/gtcryhyytq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtfueizwid.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guannengcc.top/gtvfgkkwnp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtnvxlssjk.html

TS:   // 手写 Map<string, number>
来源：http://hz.fzhhl.top/gttgahgxkb.html

Java: // 手写 HashMap
来源：http://hz.shzxlz.cn/gtmnnidhkj.html

Go:   // 手写 map[int]int
来源：http://hz.ybcxt.top/gtnkvmsruc.html

Ruby: // 手写 Hash
来源：http://hz.wangdashe.top/gtarpzjqid.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.snrcjt.cn/gtcmhobmej.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gtkgdqldzj.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxinkj.top/gtaxbigtcd.html

PHP:  // 手写递归交换
来源：http://hz.tanke756.top/gtxsjgpjsg.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtqchgetuz.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtirmoggfl.html

Java: // 手写回溯递归
来源：http://hz.nwbrower.top/gtviktheeg.html

Go:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtnqnzvlmq.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtccoixerq.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtpmywmirj.html

[N09] 栈与队列
来源：http://hz.fengsongda.top/gtsgpvbuci.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtzgfmtiqy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258.top/gtywaotefk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtlobprvih.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ybcxt.top/gtoruhpopz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guowangkeji.top/gtihtdkkib.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangshuangyany.cn/gtvyiiouok.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gtlkkypkym.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daria6918.cn/gtwvvdaqwc.html

[N10] 链表节点定义
来源：http://hz.yj20258888.top/gtxqcpgmxk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.quarkkingdee.top/gtljjgkbxn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gtqxlnllqq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shanyushiyangtech.top/gtznnmggnx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.bjfxy.top/gtxtdaeony.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtiazaybyd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xinyue.icu/gtuzngoles.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gthdhuvrny.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gtnffkpuld.html

[N11] 二叉树中序遍历
来源：http://hz.cashguo.top/gtjneflmtp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinghuilouyu.cn/gthpvhaipj.html


<!-- 参考信息 -->