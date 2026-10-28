代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtutbkhncn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtkcqffibg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtchirklcn.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxuanxn.top/gtfwgglyla.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hongshengwenyu.top/gtabayolxn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cucudq.cn/gtllkvlzwh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xziqi.cn/gtvivgxfcu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gtoastgqpz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.smart0.xyz/gtlwoajpls.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangdashe.top/gtffnntfai.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.quarkkingdee.top/gtowkvhvvz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtbfqtxrxv.html

================================================================================
来源：http://hz.jianghu66.top/gtkztrathe.html

K. JSON 与序列化
来源：http://hz.shanyushiyangkeji.top/gtwninlvhb.html

================================================================================
来源：http://hz.snrcjt.cn/gtibbbxify.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtdyqfeywt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtwmozrgcf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtjixpiutt.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtvfatzjry.html

TS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtsiscagrj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtcmfevymy.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gttmicbjsw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtlidonjzl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gteudkyppg.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gtrtndjpnz.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtfqjhqwrx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigufen.top/gtkvbpctff.html

JS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtkebuucbh.html

TS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtytydygum.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhoulong.xyz/gtjikjygtj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gttuoafwod.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gtzufyujib.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gtccpzmpnj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xylfe.cn/gtktmjvgdt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtylrpykbj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtvmhxbqcg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtnfhdeozf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtmvhbdfjm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.c1oappe.top/gtatroaqiu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhixingplan.top/gtejlrcaoo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gtxvdrpdhp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258888.top/gtgzdvkabj.html

[K04] 读取 JSON 文件
来源：http://hz.hnxiangtu.top/gtfbjyldra.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gttohatdgv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hammf.cn/gtokztxdaz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtxnvckuae.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtpsueoide.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hysaishi.cn/gtjnhnrloy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtbeuxtdqe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtwasrnvkm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gtytwcgdgk.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gthxizikon.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtlcwlleox.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhixingplan.top/gtzwoerihj.html

JS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtveldoadp.html

TS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtnciuorom.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtjtrwtrqc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtlgbamprz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ivvv.top/gtuavmndzy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhaomingkeji.xyz/gtlixjeuxf.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gthxmftkas.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sufxvd.cn/gtcfejffnv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cdnleiting.top/gtaardtbld.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtmgqejpcy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtndtfdknp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258888.top/gtiiqxcice.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gthwhjgtqm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigfzy.top/gttzxjprly.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.iojbl.cn/gtiptpymto.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtjokpnirk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daxiang520.top/gttfisghqv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtoeipcgbj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtzvdfcdjk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtykxfqvym.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtsntgpofw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yvedp.cn/gtycsmirrp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sufxvd.cn/gtmedoudlz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gtaouhaabu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtdkjvybjb.html

Py:   pickle.dumps(obj)
来源：http://hz.ydjk.org.cn/gtpyyuzany.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ywan-chungtsiang.top/gtszbojsof.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtevvogjjv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtbrxjyibn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gthfgkejje.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gttntlevfk.html

Ruby: Marshal.dump(obj)
来源：http://hz.meibo888.top/gthzquhdfk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zdqjudy.top/gtnwqgtjin.html

================================================================================
来源：http://hz.jlsjyb.cn/gtsidskwza.html

L. 网络请求
来源：http://hz.aizwys.cn/gtuftagstc.html

================================================================================
来源：http://hz.hnxiangtu.top/gtkrrwirty.html

[L01] 发送 GET 请求
来源：http://hz.pycfn.com/gtzqjslycn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydzc1.top/gturektpqy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gtvgowaboq.html

JS:   await fetch(url)
来源：http://hz.daria6918.cn/gtnaqtbjkj.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtoakyjwzr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sufxvd.cn/gtdyxiabbs.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gthxljiymy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tianlin.xyz/gttgjnoudn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yueranfly.top/gtlxrowlop.html

[L02] 发送 POST JSON
来源：http://hz.smart0.xyz/gtcmqcjhei.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtlikjpmti.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gthbnmruki.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jianghu66.top/gterhogquc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtargbbeog.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gtbwnzlddh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtmtnshjea.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jyoumei.cn/gtedjjvlrz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtmmirgeor.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtvrzlzlmo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinyuanbaomall.cn/gtsaotqydo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtilulixss.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtqhewuqce.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtrarvxwcw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tianlin.xyz/gtjnriextf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtcyyamyhj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ivvv.top/gtlzpeddxb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtmjdohaye.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtsbpqlswr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xylfe.cn/gteqyvduur.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hywenlv.cn/gttswztawp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtnwhqyvjk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtbolrmfbx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ppjwa.cn/gtpzvzuxww.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gtkmkohkit.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtmnztzzpa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gotoacloud.top/gtxxehizss.html

[L05] 上传文件（multipart）
来源：http://hz.gogol.net.cn/gtwyatguwv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guannengcc.top/gtjmbhhuox.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ydzc1.top/gtcncmcnsx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtvkqupboy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtsfecknbz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxuanxn.top/gtjsmcaide.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fengsongda.top/gtflbdmvcp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtolffccmq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jiagoushi.top/gtegusiadv.html

[L06] 解析响应为 JSON
来源：http://hz.yueranfly.top/gtcqwdupnl.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtyyyrdoev.html

PHP:  json_decode($body, true);
来源：http://hz.bjfxy.top/gthimbfctb.html

JS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtsgsfujlu.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gtcbjtpoth.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangshuangyany.cn/gtipnvblql.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtdqdvbkyp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gttepsmqsz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinghuilouyu.cn/gtnqstmwiy.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtfiynvvkb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinyuanbaomall.cn/gtemubyzxq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangkeji.top/gtpmucpjit.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtmcxjfbtz.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtzcxoprqb.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtsgrtmrbn.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtixbmnoxl.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtojvvsujo.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gtbntizqrl.html

[L08] 并发请求多个地址
来源：http://hz.dashuyun.cn/gthkrgsbkr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhiwuduotai.top/gtmfwxvmmx.html

PHP:  curl_multi_init() 系列
来源：http://hz.nwbrower.top/gtdqvmiqjv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtmckqslrg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtoqjbncph.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuanzx.com/gtlixlhirx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yanxiufei.cn/gtrrunzuse.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhengqikj.top/gtrfgfnliw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yongpay.top/gtxrsjuvcd.html

================================================================================
来源：http://hz.havefunace.top/gtkjgnebeq.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtsklzjniy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkgnfglhv.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtzdwpxewn.html

Py:   sys.argv[1:]
来源：http://hz.jianghu66.top/gthbyiiuss.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtcbeuwulp.html

JS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtqogqbfqn.html

TS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtbbxqubws.html

Java: args 数组（main 方法参数）
来源：http://hz.yj20258888.top/gtxonfcvll.html

Go:   os.Args[1:]
来源：http://hz.shzxlz.cn/gtgmwmarkl.html

Ruby: ARGV
来源：http://hz.xuanzx.com/gtqbifqkfe.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ivvv.top/gtvudpncjc.html

[M02] 读取环境变量
来源：http://hz.jiagoushi.top/gtajmlzuxr.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtyjmcdfbj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtsybbuiib.html

JS:   process.env.HOME
来源：http://hz.zycfv.cn/gtqrqpbvic.html

TS:   process.env.HOME
来源：http://hz.c1oappe.top/gtijhuqiks.html

Java: System.getenv("HOME")
来源：http://hz.jinqigfzy.top/gtvhdwftmq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhoulong.xyz/gtyqldkppr.html

Ruby: ENV["HOME"]
来源：http://hz.haohaochexian.top/gtberavcoq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ehwqpu.com/gtvzxwqhkv.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gteienzflu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtntstnvly.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuetiantiany.cn/gtivlknnyv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtnshnptux.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gttsspthtt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gtcczuflyi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gtlvlmqtyg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sxryk.cn/gtaerthhbg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtmnnyxvmr.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtrbglfmgm.html

Py:   os.getcwd()
来源：http://hz.c1oappe.top/gtzocqtitw.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtmbqomicd.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtohhcfwzw.html

TS:   process.cwd()
来源：http://hz.cucudq.cn/gtcndgmxsv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cucudq.cn/gtvkwustko.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gtfxanxize.html

Ruby: Dir.pwd
来源：http://hz.cucudq.cn/gtwbkenaly.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jlsjyb.cn/gtxwbzljxk.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gthhzbxzxo.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtkkhksrbu.html

PHP:  exit(1);
来源：http://hz.xuanzx.com/gtwjrhcuia.html

JS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtdbdkagyi.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtaoyoxvbb.html

Java: System.exit(1)
来源：http://hz.shzxlz.cn/gtghzgluyy.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gttesnvuvb.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtilzxchua.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenlongwang.top/gtudlrmeli.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtfbufxgtz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtcxdseski.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtsapawmde.html

JS:   console.error("err")
来源：http://hz.zycfv.cn/gtvfgkibjq.html

TS:   console.error("err")
来源：http://hz.hysaishi.cn/gtyjhivkgj.html

Java: System.err.println("err")
来源：http://hz.tian-w.cn/gtbakzvrfj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtmlswyjmx.html

Ruby: warn "err"
来源：http://hz.yuanzhike.top/gtgzgstchf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtcpnxuwox.html

[M07] 判断是否为主入口
来源：http://hz.dianchejie.cn/gtydhzhvdc.html

Py:   if __name__ == "__main__":
来源：http://hz.jyoumei.cn/gtdukphaeb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yvedp.cn/gtajshdent.html

JS:   require.main === module
来源：http://hz.jinqigufen.top/gtxvfsmtwx.html

TS:   require.main === module
来源：http://hz.hysaishi.cn/gtwzbipomt.html

Java: public static void main(String[] args)
来源：http://hz.mhx1999.top/gtnqvzzeel.html

Go:   func main()
来源：http://hz.zhixingplan.top/gtwuumagqc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gtelspqbuq.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gtqhwcvoif.html

[M08] 获取系统与运行时信息
来源：http://hz.zhongyouzk.top/gtflkkdgxn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258.top/gtxicitcal.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.kuanghao11.cn/gtydikisab.html

JS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gteekgttgt.html

TS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtnzkhzcpd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.snrcjt.cn/gtwwuglmcn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gtryysyngu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gtvnxhtxlw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ppjwa.cn/gtpbjntgvp.html

================================================================================
来源：http://hz.52xcode.cn/gtfwzediyb.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gtzxddcmpe.html

================================================================================
来源：http://hz.smart0.xyz/gtijeggubv.html

[N01] 二分查找（有序数组）
来源：http://hz.jinghuilouyu.cn/gtcdqgimgt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtcfoavcat.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nwbrower.top/gtjflzjuqa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtjthbcwaa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtpuvsgmqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtsryjzbqx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxuanxn.top/gtdghenwdt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gthedjynqx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fzhhl.top/gtuzrzksna.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.birdmap.top/gtvzwqwcfn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtixycuxja.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fzhhl.top/gtgbdpxqyb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtdwsxgkjl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtfllspuko.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sxryk.cn/gtvugolwxx.html

Go:   slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gttqtvovnp.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtsodzbplr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yonumen.top/gtxcatvyrv.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtbmpdigpr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gthczpodjs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtnxxjvyii.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtlndftqsa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtjhpbiwdt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cashguo.top/gtltdxlbfd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.meibo888.top/gttaoprvmu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jiagoushi.top/gtlydtechr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtgmuwmcfv.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtrksmssti.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtenixwfrb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gthbgjubhh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtvsgjukop.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gtejddmxpr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtzblxukha.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sysykeji.top/gtipdkobmn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtuwyvcsoq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dianchejie.cn/gtkcolaftz.html

[N05] 最大公约数
来源：http://hz.zhaomingkeji.xyz/gtwmejkvmu.html

Py:   math.gcd(a, b)
来源：http://hz.iojbl.cn/gtjkadvlex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xylfe.cn/gtupqeoyzs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtdmntccms.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gttinzxyac.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuanzx.com/gtcyyusako.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gtdbyrbzxp.html

Ruby: a.gcd(b)
来源：http://hz.birdmap.top/gthzsmsxuq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xziqi.cn/gtuhsurusr.html

[N06] 判断回文字符串
来源：http://hz.jlsjyb.cn/gtlvbrtkvq.html

Py:   s == s[::-1]
来源：http://hz.xylfe.cn/gtmcqmjnak.html

PHP:  $s === strrev($s);
来源：http://hz.sufxvd.cn/gtaxecxiii.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtouuctmlr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtpqyiohtz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtlqeufpzt.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtameozxpq.html

Ruby: s == s.reverse
来源：http://hz.zdqjudy.top/gtsywfyrgr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhijiandao.cn/gtxsjcqpfe.html

[N07] 两数之和（返回下标）
来源：http://hz.shzxlz.cn/gtpksqjkij.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuanzx.com/gtefvnlwmc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gtkujklszc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jianghu66.top/gtemfytbkj.html

TS:   // 手写 Map<string, number>
来源：http://hz.nwbrower.top/gtvevrxdvr.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtgjuellub.html


<!-- 参考信息 -->