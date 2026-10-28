代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aizwys.cn/gtqcpqebah.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtupmiunim.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.kuanghao11.cn/gtzbuhqzkr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtszpxhbjy.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtowhqdrvb.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtallbukdc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yangfankeji.com/gtapdabenz.html

JS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtswgpvfbx.html

TS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtdwamisip.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tian-w.cn/gtlrcnctsk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtpbfdxayc.html

Ruby: JSON.parse(s)
来源：http://hz.cqqwz.cn/gtrvkjfmdq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ehwqpu.com/gtaxobcmnm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yvedp.cn/gtzsnnufnu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gthyirtzwj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtnlbkyxvl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtkheseliq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtflggzhyn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gtbylyplkn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtkazjpbiw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sysykeji.top/gtfsksaajr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gtbkkcbicn.html

[K04] 读取 JSON 文件
来源：http://hz.zhaomingkeji.xyz/gtsdvokxvi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gttqaxlrce.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.9152youxi.cn/gtlelhidiv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtvahoqvcl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtpkinybzk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xylfe.cn/gtsbebcffl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtasmuuxjf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtxaefkmlx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gteozebruv.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtxlydwqup.html

Py:   copy.deepcopy(obj)
来源：http://hz.gaohongyu789.top/gtmulsmryi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gttayycvbw.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtcafmxqda.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtrybiwhyv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dashuyun.cn/gtqxwbtrno.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtfxltxber.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gthkzrpisg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtmimhzwlc.html

[K06] 解析 URL 查询串
来源：http://hz.snrcjt.cn/gtdlqrplrw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yongpay.top/gtzpkxduns.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yanxiufei.cn/gtfzwdiigz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtguelrqjt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtjonykcft.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gthqrmahep.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hysaishi.cn/gtonybfbwu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xziqi.cn/gttpbzpeqn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xziqi.cn/gtkopwhbvz.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtleiewmik.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgfzy.top/gtjqtvjcac.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuxming.cn/gtgjlvachu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtgungsyxj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtwrsrsmpl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtazslsuho.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sxryk.cn/gtqjtcqtxa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gtraghraho.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hongshengwenyu.top/gtdfydqnpy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtplbzyvqg.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtuyqfxfsy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtliilwehl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtfdaqgemp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gthbavbepp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gtrrhctrye.html

Go:   encoding/gob
来源：http://hz.wangshuangyany.cn/gtxqgqntik.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenlongwang.top/gtuoxzizah.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtlvsmujov.html

================================================================================
来源：http://hz.hywenlv.cn/gtnnnqfexh.html

L. 网络请求
来源：http://hz.zdqjudy.top/gtxfnscazv.html

================================================================================
来源：http://hz.sxryk.cn/gtnrgkvymq.html

[L01] 发送 GET 请求
来源：http://hz.zdqjudy.top/gtlqaswpwo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.kuanghao11.cn/gtmqbhcacz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gtofpydhyr.html

JS:   await fetch(url)
来源：http://hz.ydzc1.top/gttuvqpltn.html

TS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtwquoedvg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtsztzddtx.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtmsthtnvx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtcjishpci.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daxiang520.top/gtyppntfmh.html

[L02] 发送 POST JSON
来源：http://hz.havefunace.top/gtwyfejgli.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sxryk.cn/gtfmsrrxgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cheryme.top/gtcezylpcz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtehjlutka.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtddnrmxsz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xingfuxueyuan.xyz/gtgyohpizn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtwwdugcqq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtbpeskwfb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtxoitidkq.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtlegbjsul.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenzaomai.com/gteycwtpso.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cucudq.cn/gtvqohmqez.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtadzdxfsc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtgtzvhggt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigufen.top/gtnzqudylj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtcvpvlryj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yangfankeji.com/gtvvdhbqmz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtosmkiqdi.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtvouqyheu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hfpthk.cn/gteztnobux.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tianlin.xyz/gteaddnhec.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtxrmyarjn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtkzflxezw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sweek.top/gtttnhbzrw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hfpthk.cn/gtkcyszzxe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtblpaqgwg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yongpay.top/gtqeljumrt.html

[L05] 上传文件（multipart）
来源：http://hz.xylfe.cn/gtkrfzaumo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuanzhike.top/gtgkrndtnv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sxryk.cn/gtwclolijq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtaowdjfpb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtghajgxki.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gtqdederax.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ppjwa.cn/gtoyrlamng.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sweek.top/gtfgcbtrsa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ivvv.top/gttoeksegf.html

[L06] 解析响应为 JSON
来源：http://hz.sysykeji.top/gtngbxokxk.html

Py:   resp.json()
来源：http://hz.pycfn.com/gtwrhgbgkk.html

PHP:  json_decode($body, true);
来源：http://hz.cashguo.top/gtlcklmsgc.html

JS:   await resp.json()
来源：http://hz.wangdashe.top/gtssdpgtge.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gtvpyevvja.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jianghu66.top/gtkpiudytl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fzhhl.top/gtzcebqvra.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtzlbynvps.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtoqcqmeme.html

[L07] 处理 HTTP 状态码
来源：http://hz.sweek.top/gtlvuhznmp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinghuilouyu.cn/gtdtaigurv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.mhx1999.top/gtgimgmfgt.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtzkkatamj.html

TS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtwfrocplb.html

Java: resp.statusCode()
来源：http://hz.sysykeji.top/gtzklvvrfj.html

Go:   resp.StatusCode
来源：http://hz.jqgufenzy.top/gtmwptgpvq.html

Ruby: resp.code.to_i
来源：http://hz.zhijiandao.cn/gtsmofbdag.html

C#:   (int)resp.StatusCode
来源：http://hz.shuidangran.top/gtltzgulgf.html

[L08] 并发请求多个地址
来源：http://hz.cashguo.top/gtmjgmofmr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuanzx.com/gtaydhllpt.html

PHP:  curl_multi_init() 系列
来源：http://hz.feifeiyinyue.top/gtdnnmiwbq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtpmhwpujw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtxncgyymu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.havefunace.top/gtqbbrbrgi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgufenzy.top/gtxjtqieec.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.52xcode.cn/gtpmizczgr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtnhklxhgq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtinkkylfp.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtvxajxdrb.html

================================================================================
来源：http://hz.sufxvd.cn/gttgarrchk.html

[M01] 读取命令行参数
来源：http://hz.jinghuilouyu.cn/gtjukvjfwq.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtdfumtosv.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtiffiwdqf.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtacxmuxxi.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtsswvljsw.html

Java: args 数组（main 方法参数）
来源：http://hz.xinyue.icu/gttnhfbpoo.html

Go:   os.Args[1:]
来源：http://hz.xinyue.icu/gthioyzvui.html

Ruby: ARGV
来源：http://hz.yuanzhike.top/gthhkbtgat.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgfzy.top/gtadgwajrv.html

[M02] 读取环境变量
来源：http://hz.feifeiyinyue.top/gtxxorsxhk.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gtlujaiqga.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.c1oappe.top/gtwkonrksf.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtdmvzpznt.html

TS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtmpzfmuod.html

Java: System.getenv("HOME")
来源：http://hz.gzhubu.top/gtxvccuota.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtyyjqiuyb.html

Ruby: ENV["HOME"]
来源：http://hz.zhixingplan.top/gtykzhzour.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258.top/gtdvynnidv.html

[M03] 执行外部命令
来源：http://hz.wangdashe.top/gtorctpfvr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xziqi.cn/gtobhiieqx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgfzy.top/gtftkozpmt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gteflcgein.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtkfwgzwkw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fengsongda.top/gtodajmafc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gtfazgfeye.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gtmktsreky.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtabahkyyq.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtzqdhvdor.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtwlaakcqt.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtjezpyonz.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtuakabeau.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gtnvzqtwvq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fengsongda.top/gtkdcepunt.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtwwszreag.html

Ruby: Dir.pwd
来源：http://hz.tanke756.top/gtxwecpbui.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gtbxrgbved.html

[M05] 设置退出码
来源：http://hz.jyoumei.cn/gtulyomnhc.html

Py:   sys.exit(1)
来源：http://hz.xuanzx.com/gtwmlnnbwm.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtfucgtlmg.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtxonkogew.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtglwkzjpr.html

Java: System.exit(1)
来源：http://hz.fzhhl.top/gtxmucmmaj.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtibhuedhm.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtjyiwuhrn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtlrjeebgo.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gttrwofqll.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtdjcouacb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigfzy.top/gtvhtymazx.html

JS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gthqnubuns.html

TS:   console.error("err")
来源：http://hz.aibaodan.cn/gttilxgjor.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtfkrecjme.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtysrrfoni.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtvnujhqxz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yanxiufei.cn/gtamsvymss.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtbvywxgmw.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gteseroqdt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinyuanbaomall.cn/gtnlettejn.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtprrsckza.html

TS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtnrwhxbyt.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtclusmwiu.html

Go:   func main()
来源：http://hz.ivvv.top/gtgfaqrhny.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gtzudefcpt.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gthngirqsg.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtnweefvtu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hongshengwenyu.top/gtssedutcy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtfllislkn.html

JS:   process.platform;  process.version
来源：http://hz.yuxming.cn/gtcwcwllls.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtoddbtbvl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258888.top/gtdaynvfxt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangtech.top/gtkileaoqd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tian-w.cn/gtudolhhwb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gthsxkasjy.html

================================================================================
来源：http://hz.wangdashe.top/gtcljrpagu.html

N. 数据结构与算法
来源：http://hz.ywan-chungtsiang.top/gtbgpkxlst.html

================================================================================
来源：http://hz.jqgfzy.top/gtgpmrwbbi.html

[N01] 二分查找（有序数组）
来源：http://hz.c1oappe.top/gtdedxsgzm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guannengcc.top/gtlzrlnaxm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtolvxeiqf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtdascstbl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtpjmzdysh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shuidangran.top/gtpjpmniaj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigufen.top/gtxonxwxdt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ywan-chungtsiang.top/gtykdwhhcu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fengsongda.top/gtfweclypm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gtgabseaah.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtbyheyfng.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtqwvunsxc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtvfthwehx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtqlikrvzi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xylfe.cn/gtwdzbwdnj.html

Go:   slices.Sort(arr)
来源：http://hz.yongpay.top/gtgtnzwwyb.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gttgwujhzp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtgoeqpewz.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258.top/gtjgsfjnlj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zycfv.cn/gtiudvyfwa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.52xcode.cn/gtbjfhakdm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtuyscbvnn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtaywjuahd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtqybttabz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zycfv.cn/gtgmugjppa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gaohongyu789.top/gtkxmdfusx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.daxiang520.top/gtjyojcinn.html

[N04] 斐波那契数列
来源：http://hz.sufxvd.cn/gtgeqxuafk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtfrrgyzgc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shangyingyoupin.top/gtlbugtexm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtfikmwwbf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtxpivjyae.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ehwqpu.com/gtoyakhubh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shzxlz.cn/gtddzixpwl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtqyumckje.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zycfv.cn/gtqcvtpzwq.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtrhulrehz.html

Py:   math.gcd(a, b)
来源：http://hz.jyoumei.cn/gtaqftrxos.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yongpay.top/gtlhvgxzci.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtlwysyydw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtnekovnsf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cheryme.top/gthrurlgmz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtzjmgpxjm.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtocddimaa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gtzzppgcfe.html

[N06] 判断回文字符串
来源：http://hz.cashguo.top/gtgptrbmzo.html

Py:   s == s[::-1]
来源：http://hz.snrcjt.cn/gttsxuqrpl.html

PHP:  $s === strrev($s);
来源：http://hz.pengpengdd.cyou/gtytkbtbmx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtkebqitwp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtfbmfhuxp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgufenzy.top/gtwwqkoikr.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtlaiqflgy.html

Ruby: s == s.reverse
来源：http://hz.andypj.xyz/gtcnnhlbqm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangkeji.top/gtmvawiaty.html

[N07] 两数之和（返回下标）
来源：http://hz.xuetiantiany.cn/gtmlaplmzd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hywenlv.cn/gtlzowwvac.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.andypj.xyz/gtbjervkjn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shuidangran.top/gttzswywln.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangshuangyany.cn/gtaruopsex.html

Java: // 手写 HashMap
来源：http://hz.feifeiyinyue.top/gtjaukczcw.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtvnbuvthr.html

Ruby: // 手写 Hash
来源：http://hz.zhijiandao.cn/gtjrkebylt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gogol.net.cn/gtmqcveuxo.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtqotlslmy.html

Py:   itertools.permutations(arr)
来源：http://hz.yangfankeji.com/gtrcydydqj.html

PHP:  // 手写递归交换
来源：http://hz.andypj.xyz/gtacumqoed.html

JS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtjukmcesj.html

TS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtuwntepks.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gthtyhqsfu.html

Go:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtwoslccec.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtmdrblpve.html

C#:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtjxgcidia.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gthedvkmwa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.pengpengdd.cyou/gtckopvtkc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.c1oappe.top/gtjrwglgfm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtuqhfoixz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ywan-chungtsiang.top/gtbzxbypxg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangdashe.top/gtjutpamfa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.kuanghao11.cn/gtricccxlb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.havefunace.top/gtavqcvrxy.html


<!-- 参考信息 -->