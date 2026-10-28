代发 wailian999

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtrymsqqsi.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtjdubodly.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yanxiufei.cn/gtupjpumsn.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtuxckfvuh.html

TS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtysdgujaz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gtdcyrxmni.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtpzidwvoc.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtblgxjwyb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gtwhqpozos.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgfzy.top/gtbsyoryuv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtupuwavpv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hywenlv.cn/gtyjphusfd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtfotlhiiq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtnqqoshfi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gthayzkdmx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gtujmpuuwq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtejpslady.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydjk.org.cn/gtpdkgmayd.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtwxsldkdp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangdashe.top/gttcmwiuua.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.bjfxy.top/gtyingtryp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtwqmsxqwu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtpzwrfwep.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenlongwang.top/gtqwptldqz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtipkensjb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgfzy.top/gtnkvsekph.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gaohongyu789.top/gtwxfqkhnz.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtehtxumav.html

Py:   copy.deepcopy(obj)
来源：http://hz.xingfuxueyuan.xyz/gtzafqjjtp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.svipenyu.cn/gtcdjehmlz.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtxzegzkby.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtfkoyhtfr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ywan-chungtsiang.top/gtmuuzdrfr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xylfe.cn/gtodhfrimm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guannengcc.top/gtsfersxou.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cqqwz.cn/gtxjfjjkah.html

[K06] 解析 URL 查询串
来源：http://hz.zhaomingkeji.xyz/gtuwookadb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtomgylxyh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenjidiqi.icu/gtyyavtmoq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtmiwraepq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtgajexqcg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuanzhike.top/gtgrvrofey.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shzxlz.cn/gtzmztrtsh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gtcdjacrpr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtuidvpqvz.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtseschhft.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xylfe.cn/gtgcvlpaap.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtjwqzuaqu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtlqoygolr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gthdwrhcec.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtihgqnemq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangshuangyany.cn/gtcoryjoix.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gthrmkztnp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zdqjudy.top/gtwtkjlfzb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tianlin.xyz/gtmbyfnych.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtzhybogvm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gtqlqwmzha.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtydvspegn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtlfhtrphd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtqusefdrb.html

Go:   encoding/gob
来源：http://hz.haohaochexian.top/gtribnhmpj.html

Ruby: Marshal.dump(obj)
来源：http://hz.xinyue.icu/gtbhrvhsju.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gtkystzpfy.html

================================================================================
来源：http://hz.daria6918.cn/gtenqpgzuu.html

L. 网络请求
来源：http://hz.cucudq.cn/gtkflbsqrj.html

================================================================================
来源：http://hz.nanxinkj.top/gthglmobjo.html

[L01] 发送 GET 请求
来源：http://hz.yuanzhike.top/gtkkekvwsm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tanke756.top/gthjrstoyk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenjidiqi.icu/gtpaoaqqyt.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtjmeefnib.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtuxvkjfrs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ehwqpu.com/gtchvikcdc.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtxxomuauo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuetiantiany.cn/gtrmnnrwbn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pengpengdd.cyou/gtngiyeqnq.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtyizqwuro.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.quarkkingdee.top/gtmymcifmw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnxiangtu.top/gtzzbrkiym.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtjoynzten.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtxbvvbhux.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhaomingkeji.xyz/gtsifpojyw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gtkzdlwtbf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.c1oappe.top/gtcghhqykq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhijiandao.cn/gttzoemvhs.html

[L03] 设置自定义请求头
来源：http://hz.nanxuanxn.top/gtcqhplqpq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.0kj1m.cn/gtbwckijhg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sufxvd.cn/gtopuetvsg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtujaavktg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtodjqyvso.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gtriuimmle.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gtnftilbfp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gttgpqpqad.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtvcokitov.html

[L04] 设置超时
来源：http://hz.shangyingyoupin.top/gtwndvdovc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.9152youxi.cn/gtlalxnjqc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gtjcjoafdy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtzmuhmdsm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtloxicemk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtofhfnotq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yueranfly.top/gtjanxakpe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtdwmnmfeh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtnlesgxxo.html

[L05] 上传文件（multipart）
来源：http://hz.tian-w.cn/gtvdnjkatl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtsmlwxvgc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.iojbl.cn/gtxlvpwgbc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtkjdayhvm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtmbgkavka.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangdashe.top/gtmfvnroqh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aibaodan.cn/gtqqdjbblg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jianghu66.top/gtpwshwmgd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gteelwcdyl.html

[L06] 解析响应为 JSON
来源：http://hz.ydzc1.top/gtnbkgeobr.html

Py:   resp.json()
来源：http://hz.feifeiyinyue.top/gtkbzziygg.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gthcmdsggg.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtexetvwdz.html

TS:   await resp.json()
来源：http://hz.xziqi.cn/gtiaqbmxjq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.iojbl.cn/gtuhuevxjz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cheryme.top/gtwfrvoswm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tian-w.cn/gtlhzhkhjl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.smart0.xyz/gtvjwsyzue.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnqzz.top/gtrncwspow.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aizwys.cn/gtvazthabo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxuanxn.top/gtntfbdavr.html

JS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtpldrovua.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtkfnllphg.html

Java: resp.statusCode()
来源：http://hz.hfpthk.cn/gtatnwwbmc.html

Go:   resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtcsiigypn.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtzthupwki.html

C#:   (int)resp.StatusCode
来源：http://hz.sysykeji.top/gtaarfcimb.html

[L08] 并发请求多个地址
来源：http://hz.hnxiangtu.top/gtldbbslgu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gzhubu.top/gtdnkodxfs.html

PHP:  curl_multi_init() 系列
来源：http://hz.sysykeji.top/gtcmgwznvx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtwswszfbl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtxsfsqbtp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtboomlivy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjfxy.top/gtiqvbwzeq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.52xcode.cn/gtwknzqwes.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtbnzzlcmh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmrpzzkur.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtshgrbmar.html

================================================================================
来源：http://hz.sxryk.cn/gtrgyrwbfm.html

[M01] 读取命令行参数
来源：http://hz.ybcxt.top/gtsoultiso.html

Py:   sys.argv[1:]
来源：http://hz.zdqjudy.top/gtodzfkarq.html

PHP:  $argv;  $argc;
来源：http://hz.zdqjudy.top/gtibxoadln.html

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtbeczvhfi.html

TS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtqpsqexzc.html

Java: args 数组（main 方法参数）
来源：http://hz.bjfxy.top/gtsugoheuq.html

Go:   os.Args[1:]
来源：http://hz.xuetiantiany.cn/gtoaqfxijs.html

Ruby: ARGV
来源：http://hz.yangfankeji.com/gtkxkegupg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtggvhkgac.html

[M02] 读取环境变量
来源：http://hz.andypj.xyz/gttcgkpcca.html

Py:   os.environ.get("HOME")
来源：http://hz.jlsjyb.cn/gtzjujxzvx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtofaqvxty.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gteteipjgv.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtyoqphnuc.html

Java: System.getenv("HOME")
来源：http://hz.guowangkeji.top/gtsopbiajb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nwbrower.top/gtwmbdwscc.html

Ruby: ENV["HOME"]
来源：http://hz.jqgfzy.top/gteemaymhf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gtsabyardz.html

[M03] 执行外部命令
来源：http://hz.yueranfly.top/gttjiufbpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jiagoushi.top/gtzaejeraw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258888.top/gtgoynnpdt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtoyotbtxw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtxxtnegcc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtjvgfmtgs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangshuangyany.cn/gtdsqreyqx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydjk.org.cn/gtccolacvb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hysaishi.cn/gtpzlamctx.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtacabicpd.html

Py:   os.getcwd()
来源：http://hz.nwbrower.top/gtxvhorouh.html

PHP:  getcwd();
来源：http://hz.zycfv.cn/gtdueecijm.html

JS:   process.cwd()
来源：http://hz.yj202588.top/gtxkzkzrpk.html

TS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtcnbwzrxx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shangyingyoupin.top/gtbgjqmwei.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gtovxywlnq.html

Ruby: Dir.pwd
来源：http://hz.xingfuxueyuan.xyz/gtaodwnsrs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zdqjudy.top/gtsqswxgiv.html

[M05] 设置退出码
来源：http://hz.hywenlv.cn/gtuxynqxox.html

Py:   sys.exit(1)
来源：http://hz.hnxiangtu.top/gtwdvuoasw.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtieimwwrk.html

JS:   process.exit(1)
来源：http://hz.andypj.xyz/gtsiohrges.html

TS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtuzchdezu.html

Java: System.exit(1)
来源：http://hz.cheryme.top/gtfksddqvo.html

Go:   os.Exit(1)
来源：http://hz.zhijiandao.cn/gtutbjiddv.html

Ruby: exit 1
来源：http://hz.sxryk.cn/gtfmhjrsru.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gttadeweid.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtrzikmjsp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtxutsrmbp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtaowxcvcp.html

JS:   console.error("err")
来源：http://hz.jinqigufen.top/gtkjgvruih.html

TS:   console.error("err")
来源：http://hz.yvedp.cn/gtcbgbogqz.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gtaxvivdwx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtyefewpjm.html

Ruby: warn "err"
来源：http://hz.0kj1m.cn/gtongzhsmh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.bjfxy.top/gtzxyfsdjg.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gtzrqqasvl.html

Py:   if __name__ == "__main__":
来源：http://hz.sweek.top/gthxbprqfc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydjk.org.cn/gtnswlvsbe.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gtgsxybvwh.html

TS:   require.main === module
来源：http://hz.redwolf501.top/gtllbwfwxd.html

Java: public static void main(String[] args)
来源：http://hz.tianlin.xyz/gtidvnruxe.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtdomhkakn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtrqhadnzo.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtgunuptnn.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtyarofuum.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenjidiqi.icu/gtmbivzlef.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shuidangran.top/gtdmpfhevu.html

JS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtdliphcwi.html

TS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtemltilaf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.vqdsnc.cn/gtagrlzogg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.daria6918.cn/gtsngcbmsz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangdashe.top/gthdkyrszz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hfpthk.cn/gtmdwoontm.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjbgwuilc.html

N. 数据结构与算法
来源：http://hz.cashguo.top/gtjjnuoscm.html

================================================================================
来源：http://hz.fengsongda.top/gtubgoxrfi.html

[N01] 二分查找（有序数组）
来源：http://hz.fzhhl.top/gtextqvkmx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.haohaochexian.top/gtsaqqtujq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhengqikj.top/gtwpsaaioc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtaaqrmmfx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtnhbdbmqe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtavakdbam.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtxvzsdljy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hywenlv.cn/gtenwthhlb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuxming.cn/gtlpvtekib.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtkoklukrq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gttxaqjfdw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hysaishi.cn/gtrrizfenw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtwmenqmmj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtlshxiwlw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cqqwz.cn/gtpkspsppf.html

Go:   slices.Sort(arr)
来源：http://hz.iojbl.cn/gthdwspixi.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtvpcowckv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.quarkkingdee.top/gtshzqsdod.html

[N03] 快速排序（分治示例）
来源：http://hz.cheryme.top/gtgxwkpads.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtshvqyszl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtjulbcteq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtynokhlni.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtolnbprxo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jianghu66.top/gteqfjeplt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ehwqpu.com/gtfyanpndd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shzxlz.cn/gtmgpphejo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sysykeji.top/gtmmxxfmtr.html

[N04] 斐波那契数列
来源：http://hz.xingfuxueyuan.xyz/gtaixmjjio.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtcetgcide.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tianlin.xyz/gtdvoimgas.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtouarkvoj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtgpknzryg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258888.top/gtbtvlvmue.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shangyingyoupin.top/gtrtifliwi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtsbnwlqgw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.birdmap.top/gtrbqiylzx.html

[N05] 最大公约数
来源：http://hz.jyoumei.cn/gtteilssgk.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gttbonramm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtzttobghi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtewquqeqw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtzsrcdswv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ehwqpu.com/gtjvwqfqyw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhaomingkeji.xyz/gtbrqkwoji.html

Ruby: a.gcd(b)
来源：http://hz.pengpengdd.cyou/gtlyvcehca.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ivvv.top/gtxsoytuwc.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtdniobswo.html

Py:   s == s[::-1]
来源：http://hz.shanyushiyangtech.top/gthfmixosf.html

PHP:  $s === strrev($s);
来源：http://hz.9152youxi.cn/gtafhjbvbr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtcwavafpr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtzxisldpj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtmxlzfywq.html

Go:   // 双指针从两端比较
来源：http://hz.jianghu66.top/gtvbzajjpa.html

Ruby: s == s.reverse
来源：http://hz.nanxuanxn.top/gtqjvyuemq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtscbulfzh.html

[N07] 两数之和（返回下标）
来源：http://hz.gogol.net.cn/gtpoggcdja.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtqansyooq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.316326.xyz/gtlpdqinxp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxuanxn.top/gtfucdvoxf.html

TS:   // 手写 Map<string, number>
来源：http://hz.hammf.cn/gteoohdbps.html

Java: // 手写 HashMap
来源：http://hz.cheryme.top/gtepcpycgb.html

Go:   // 手写 map[int]int
来源：http://hz.wangshuangyany.cn/gtkzgcvaxl.html

Ruby: // 手写 Hash
来源：http://hz.hnqzz.top/gtzbujgnef.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.vqdsnc.cn/gtbcgnymzp.html

[N08] 生成全排列
来源：http://hz.sxryk.cn/gtprmwitrq.html

Py:   itertools.permutations(arr)
来源：http://hz.zhengqikj.top/gtpintbfov.html

PHP:  // 手写递归交换
来源：http://hz.jqgufenzy.top/gtvvgmwyjn.html

JS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtfvkeorlw.html

TS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtlqihdljd.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtbcmsnacf.html

Go:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gttqqrgjtt.html

Ruby: arr.permutation.to_a
来源：http://hz.ehwqpu.com/gtiuniaoue.html

C#:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtsjvvdhyg.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtdhejdnmm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtxtmkyvay.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtwawaspul.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tanke756.top/gtdhtnedrp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhixingplan.top/gtoavkfmsg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yonumen.top/gtknfisrss.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tianlin.xyz/gteovceelm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtkkssnhpq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxuanxn.top/gtpuwwmsur.html

[N10] 链表节点定义
来源：http://hz.jlsjyb.cn/gtubxgmiht.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gotoacloud.top/gtpvkltdgh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtzcwixofa.html


<!-- 参考信息 -->