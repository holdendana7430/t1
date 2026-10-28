代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gtlylghgcr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hfpthk.cn/gtlmbdlmln.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aibaodan.cn/gtvsycfxji.html

[J10] 取今天 / 本月第一天
来源：http://hz.jiagoushi.top/gtnpznrdjq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangtech.top/gtvneqeljw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtktaxnpwc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gtjffnzxct.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtvofvzxzd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtpwfqayqz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.svipenyu.cn/gtbzaeqoiz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtqxucasee.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.kuanghao11.cn/gtidltzfvy.html

================================================================================
来源：http://hz.jiagoushi.top/gtswjafuil.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gtctfolmtg.html

================================================================================
来源：http://hz.gotoacloud.top/gteddaqpyk.html

[K01] 对象转 JSON 字符串
来源：http://hz.feifeiyinyue.top/gtpaqylyjo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtckdpbbfa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtvgrdokad.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtnbccnmxd.html

TS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtllxrhtmc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtuvzluviw.html

Go:   json.Marshal(obj)
来源：http://hz.ywan-chungtsiang.top/gtqywaxkoe.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gaohongyu789.top/gtvtiatmrf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhiwuduotai.top/gtdussmjpk.html

[K02] JSON 字符串转对象
来源：http://hz.haohaochexian.top/gtcanqyaag.html

Py:   json.loads(s)
来源：http://hz.chenjidiqi.icu/gtmglrikce.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pengpengdd.cyou/gtgtdtnnev.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtxahknkhs.html

TS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtuvueaolq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtsirbjtmf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtygphaedo.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtlpoesumf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shangyingyoupin.top/gtobzgtoja.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gaohongyu789.top/gtvgqiwbbl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sxryk.cn/gttjsozsax.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtjwgesaaa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtfxwjbgum.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtsxwikozn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gtcmgfaiqn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xylfe.cn/gtlpltanqa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangdashe.top/gtmiwzagze.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gogol.net.cn/gtwzafjdsv.html

[K04] 读取 JSON 文件
来源：http://hz.shzxlz.cn/gtpmdmcflz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtndmiucac.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxinkj.top/gtsonmjipu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtcfjhaunn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtogrcuztv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hongshengwenyu.top/gtwpqhjsoi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tianlin.xyz/gthtdvnzps.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtxpsndabi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xylfe.cn/gtvxyflher.html

[K05] 深拷贝对象
来源：http://hz.xylfe.cn/gtcudkawyr.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgfzy.top/gtmkrgfbrh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gtnrinauhz.html

JS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtvimimnwp.html

TS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtrpjtggsh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.havefunace.top/gtfvrhzpsr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gzhubu.top/gtqpqnoqar.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.316326.xyz/gtrjcopxiy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtnxlotyua.html

[K06] 解析 URL 查询串
来源：http://hz.yueranfly.top/gtqqqcdscx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtciscftwl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtoapontwu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtmlpwdpnr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtprhyxpeo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtvrlzdovq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tian-w.cn/gtvvafbvpy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sweek.top/gttlendyvs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnqzz.top/gtfydtphqe.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtjzguuldf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gthbdvrnue.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtghovrune.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtegfckhsa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtihkcsoxk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtuqygsxky.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gtjnpnryhb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guowangkeji.top/gtngnezbml.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtjegalwjm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.havefunace.top/gtnparndam.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gtduqxvbrv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xingfuxueyuan.xyz/gtylzpjmpz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtmlmmgxay.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtwjwpwzlm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.svipenyu.cn/gtilmqulhl.html

Go:   encoding/gob
来源：http://hz.jinqigufen.top/gthlxcdhqe.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gttvsiwzsv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daria6918.cn/gtduojlljc.html

================================================================================
来源：http://hz.daxiang520.top/gturtcyruk.html

L. 网络请求
来源：http://hz.shanyushiyangtech.top/gtmiupgwgg.html

================================================================================
来源：http://hz.316326.xyz/gtocxyqzxr.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtyflzahfy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxuanxn.top/gtqhjgartg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenzaomai.com/gtxatlksgj.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtnircqeyv.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gtaxkgnfsp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtajtrmowv.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgufenzy.top/gtvomrhwph.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtslfwufgm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnqzz.top/gtdlqldyhg.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtewkwrdaa.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigufen.top/gtxnsnserz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinyuanbaomall.cn/gtcimcuqnw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtvpmzxhsb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtwteytptn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtwbhfubil.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gtnwvzbhzd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuanzhike.top/gtdkgfdoiv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhiwuduotai.top/gtkijzzkkv.html

[L03] 设置自定义请求头
来源：http://hz.shangyingyoupin.top/gtcmgxgidj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydzc1.top/gteyoxiqxw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.smart0.xyz/gtgdqtsxkq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gthcoajqhh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gttnwzhobh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yangfankeji.com/gtmrhodxnh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gthvtfgwwg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nwbrower.top/gtiwsorvoq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sufxvd.cn/gtmzdjjxvg.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtoaobwxgq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.quarkkingdee.top/gtbibhhlyn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yueranfly.top/gtvhraxxbe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtmgtyvdxq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtnnglagcf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gttfjnbfwc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yonumen.top/gtqocdabpp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtfuxizxca.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zdqjudy.top/gtkuykikfl.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gtxyspjkdz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dianchejie.cn/gtvpcoeots.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtdgtjpukh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtsruxqqxl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtciayykyh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.316326.xyz/gtloullcgb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtbyjujcgn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gtpiwfsmvj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hywenlv.cn/gtcpngkhnp.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gtwcnlxhpz.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtfiodxxub.html

PHP:  json_decode($body, true);
来源：http://hz.shangyingyoupin.top/gtdlqzkrgx.html

JS:   await resp.json()
来源：http://hz.cqqwz.cn/gtnqxvpjje.html

TS:   await resp.json()
来源：http://hz.dianchejie.cn/gtzlemmfic.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hywenlv.cn/gtlteqkfge.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gtchqfmncc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtylybsxff.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtgtqtncff.html

[L07] 处理 HTTP 状态码
来源：http://hz.hysaishi.cn/gtxwkareuf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.quarkkingdee.top/gtohbqlltq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aizwys.cn/gtulzspofm.html

JS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtsfnxejsr.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtkrqysasf.html

Java: resp.statusCode()
来源：http://hz.havefunace.top/gtgvojntau.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gtxpovxqrv.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtbbjoeiml.html

C#:   (int)resp.StatusCode
来源：http://hz.ivvv.top/gtzbklviin.html

[L08] 并发请求多个地址
来源：http://hz.guowangkeji.top/gtnaaivzcc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.redwolf501.top/gtkswornis.html

PHP:  curl_multi_init() 系列
来源：http://hz.ppjwa.cn/gtrkgkmhol.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtjnkfovxe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gthzpxashp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtpjzpbfdg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhengqikj.top/gtqzuhfkmh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jyoumei.cn/gtmbknzkfw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yanxiufei.cn/gtdsejkdxa.html

================================================================================
来源：http://hz.tian-w.cn/gtrzmbenbn.html

M. 命令行 / 进程 / 环境
来源：http://hz.316326.xyz/gtmibxxhld.html

================================================================================
来源：http://hz.jiagoushi.top/gtqdfmdgfj.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtnvmcowtv.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtriougtsj.html

PHP:  $argv;  $argc;
来源：http://hz.snrcjt.cn/gtexamjwpi.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtlqfzbxbo.html

TS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtchqnhwau.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtihfbplfm.html

Go:   os.Args[1:]
来源：http://hz.cdnleiting.top/gtnquhmuzr.html

Ruby: ARGV
来源：http://hz.chenjidiqi.icu/gtbvpziclh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.316326.xyz/gthfsttoja.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtjlbqxmug.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtfaxskpfs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuetiantiany.cn/gtdsmsxtjc.html

JS:   process.env.HOME
来源：http://hz.xuanzx.com/gtmidzvjye.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtgdwpcqpi.html

Java: System.getenv("HOME")
来源：http://hz.dianchejie.cn/gtiblqtvwd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fzhhl.top/gtljsbnjep.html

Ruby: ENV["HOME"]
来源：http://hz.xinyue.icu/gtjvwjihjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pycfn.com/gtmmftofkj.html

[M03] 执行外部命令
来源：http://hz.sweek.top/gtbhealyzy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtksuzpnny.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgfzy.top/gtnrkdfbti.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gttzzedpdy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gttzrupssx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxuanxn.top/gttyhcpsbv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gotoacloud.top/gtcnjczanx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtvjucejnc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dashuyun.cn/gtqlfllapx.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gtwezushou.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtiujtbrkk.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gtsgmvlixn.html

JS:   process.cwd()
来源：http://hz.dashuyun.cn/gtmezvljfp.html

TS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtmblrceqq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cqqwz.cn/gtpziwfeah.html

Go:   os.Getwd()
来源：http://hz.cqqwz.cn/gtdzwcyhgp.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangtech.top/gttfxxymsm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtdtyiupdh.html

[M05] 设置退出码
来源：http://hz.quarkkingdee.top/gtemubsood.html

Py:   sys.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtztqkwcef.html

PHP:  exit(1);
来源：http://hz.jinqigufen.top/gtovvarico.html

JS:   process.exit(1)
来源：http://hz.redwolf501.top/gtoonspugg.html

TS:   process.exit(1)
来源：http://hz.wangdashe.top/gtfqqgvgfi.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gtbueqdeay.html

Go:   os.Exit(1)
来源：http://hz.ehwqpu.com/gtglykutks.html

Ruby: exit 1
来源：http://hz.yj20258888.top/gtveiswwsa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnxiangtu.top/gtbiwohiqp.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtwlrvqpxx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gtdvyatcrm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtybnzykxt.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtjkrfzbak.html

TS:   console.error("err")
来源：http://hz.feifeiyinyue.top/gtknythuir.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtmhkwnrbp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtvixbkzry.html

Ruby: warn "err"
来源：http://hz.aibaodan.cn/gtocqduaqs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gttzfnmobg.html

[M07] 判断是否为主入口
来源：http://hz.tanke756.top/gtdiohsqgd.html

Py:   if __name__ == "__main__":
来源：http://hz.cashguo.top/gtyrhdvcfh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gzhubu.top/gtcdhyiwmf.html

JS:   require.main === module
来源：http://hz.fzhhl.top/gtwxeghnag.html

TS:   require.main === module
来源：http://hz.yonumen.top/gtegrwodqo.html

Java: public static void main(String[] args)
来源：http://hz.kuanghao11.cn/gtazomqdtt.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtowyyvwvb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gtcnphklos.html

C#:   static void Main(string[] args)
来源：http://hz.jqgfzy.top/gtxigvuofu.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gtnpggmhue.html

Py:   platform.system();  platform.python_version()
来源：http://hz.havefunace.top/gtbsnhtadr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnxiangtu.top/gtamnjfhvj.html

JS:   process.platform;  process.version
来源：http://hz.sufxvd.cn/gtlezuvxrr.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtmqapakrh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinghuilouyu.cn/gtcejglsan.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gtphxuwgle.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxinkj.top/gtsnmttpxh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gogol.net.cn/gtveyytkvv.html

================================================================================
来源：http://hz.gogol.net.cn/gtccwcujeg.html

N. 数据结构与算法
来源：http://hz.hongshengwenyu.top/gtaofhvlyi.html

================================================================================
来源：http://hz.tian-w.cn/gtzyaclvqv.html

[N01] 二分查找（有序数组）
来源：http://hz.yj202588.top/gtcgosuyjn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtivehblxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zdqjudy.top/gtdrysucbr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gthzjowjpg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtcogmhtsv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtdnbtdgdq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xuetiantiany.cn/gtqfnaylgd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gteuubiysu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtoodbspwo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gttqejdkau.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtndwfwtre.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.daria6918.cn/gtnzrwcmjq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtkrwftnlo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtejjxhmrf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxuanxn.top/gtpbjsuehj.html

Go:   slices.Sort(arr)
来源：http://hz.ivvv.top/gtfxigpfyy.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtbddlxyub.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxinkj.top/gtyqrnukhw.html

[N03] 快速排序（分治示例）
来源：http://hz.chenlongwang.top/gtoihkcdat.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guowangkeji.top/gtkwjnwexh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gttnfsduou.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gtttrpdckc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.quarkkingdee.top/gtcqufpkgj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cashguo.top/gtdnnzplmo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtdbldklox.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shangyingyoupin.top/gtvghkncax.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtnksmfumn.html

[N04] 斐波那契数列
来源：http://hz.wangshuangyany.cn/gtdnsrupdj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtucbkypme.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnxiangtu.top/gtakdghcfy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gthygynoui.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gttdazpxor.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cheryme.top/gteifogarh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgfzy.top/gtgolnhpdf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtpyymbwyg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtgiovbxha.html

[N05] 最大公约数
来源：http://hz.aibaodan.cn/gtotvuuhbp.html

Py:   math.gcd(a, b)
来源：http://hz.jinghuilouyu.cn/gtwlgeaday.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gtlszliyno.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gttyaauleg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gthrvwfuej.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuxming.cn/gtwjamfvyb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtaxsdzxqm.html

Ruby: a.gcd(b)
来源：http://hz.svipenyu.cn/gtauywuosy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgufenzy.top/gtfskpebuq.html

[N06] 判断回文字符串
来源：http://hz.ehwqpu.com/gtlgvbhhta.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtzlcbbmuf.html

PHP:  $s === strrev($s);
来源：http://hz.hnxiangtu.top/gtpuznsmke.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtvqwmtzbo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtztrievkm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gthlyywulk.html

Go:   // 双指针从两端比较
来源：http://hz.redwolf501.top/gtcdmjxdco.html

Ruby: s == s.reverse
来源：http://hz.hnqzz.top/gtjlpjwiel.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtosrcveef.html

[N07] 两数之和（返回下标）
来源：http://hz.vqdsnc.cn/gtdibmgixd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtladmncun.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shuidangran.top/gtnbgbkhbj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hysaishi.cn/gtgyepgvuy.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhongyouzk.top/gtjaawknmi.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gtovkyokjp.html


<!-- 参考信息 -->