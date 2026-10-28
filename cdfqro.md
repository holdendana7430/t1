代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtlvonecby.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtbmycmidp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtevwohiko.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.0kj1m.cn/gtryjobepj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.smart0.xyz/gtkhmanfet.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtlxewwhgn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtuqslemhy.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtuqgcyvzs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtngwmodxe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhiwuduotai.top/gtojbccfkd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yanxiufei.cn/gthwpkmxtc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cashguo.top/gtedgrfduq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtmzuyqhsl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.snrcjt.cn/gtwqglnqjs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhixingplan.top/gtozefijbl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtuvtbtqov.html

================================================================================
来源：http://hz.zhixingplan.top/gtrrpnweej.html

K. JSON 与序列化
来源：http://hz.hfpthk.cn/gtdvttccyq.html

================================================================================
来源：http://hz.yj20258.top/gtnksprqwp.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtgzistulm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtueojthob.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gttwzczjak.html

JS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtolfihawc.html

TS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtwhtrxwjk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fzhhl.top/gtlvjrkcps.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtnhdneqjv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenzaomai.com/gtezvqiubv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtrrdlartu.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gtfwagxtxp.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtxqbxviyp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtmfykqeuc.html

JS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtdicekidj.html

TS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtcsluzjqj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.aizwys.cn/gtwufurhvl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtnrtbhuba.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtqctlzbhy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtpnnusgaz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gteuvhzuqx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtoatohveb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtzxjvbwym.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtngaaoqqc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtwgnkutcy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.redwolf501.top/gtlcvzmubl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtrjpunybe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtfjjlovui.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.mhx1999.top/gtcxdkpozf.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtmdrcfeik.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258.top/gtodrvyzyr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtckcryaic.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtqppfgiyx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtqybidpns.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daria6918.cn/gtgrehevpt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtiwdryypk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtnvlenuch.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tanke756.top/gtwsmwpyor.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtocpdherj.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtoiwtpnmx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtllvwdhwr.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtyescetht.html

TS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtuszwqttl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtcbqwesfa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.andypj.xyz/gtchqlyucv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtqngmnfuy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtmcrizalt.html

[K06] 解析 URL 查询串
来源：http://hz.pengpengdd.cyou/gtgvqodwex.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jlsjyb.cn/gtlxpmwngw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhijiandao.cn/gtrtwhkqbn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtxuwnqztw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtydwvdfpy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtejvnrncf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtepabbhfv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gtaejkslue.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtpomtjyff.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtoqshycrk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gtkmbifaiv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtxsfhfwhp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtvovkcpjb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtaxfdyvsi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtbxxlmllv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtmdwwatge.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gterehafwe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aibaodan.cn/gtfaeuecjq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.9152youxi.cn/gtpbeyedui.html

Py:   pickle.dumps(obj)
来源：http://hz.daxiang520.top/gtkfuhobik.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.c1oappe.top/gtutmmonnr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtkusobfqo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtfazxlvbn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtezvgsvnr.html

Go:   encoding/gob
来源：http://hz.fengsongda.top/gtwfhdkioy.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtwrttluvb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.smart0.xyz/gtmcwgwhhh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthjwmaodc.html

L. 网络请求
来源：http://hz.yuanzhike.top/gtssncvsem.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtybgxrxik.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtdtufydvs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydzc1.top/gtpeudbqsz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnxiangtu.top/gtbbqchpxt.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtewxnknjb.html

TS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtxpinkckx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.birdmap.top/gtuhuyldyt.html

Go:   resp, err := http.Get(url)
来源：http://hz.aizwys.cn/gthtnwgiye.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gthaocqdhr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnqzz.top/gtgatbqgkv.html

[L02] 发送 POST JSON
来源：http://hz.ppjwa.cn/gtwsnyvssm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aibaodan.cn/gtekenfqwf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtqqucgnqw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtquiavior.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtlswpgfij.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtsdvvoyrm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtvrwgvycc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtjawhhmtl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guannengcc.top/gthdfhzjkm.html

[L03] 设置自定义请求头
来源：http://hz.hywenlv.cn/gtteghtouu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gtwnfkqccc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ivvv.top/gtbitemvxn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtrliopnco.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtwhwqhcjn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gtfbbmodui.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yvedp.cn/gterdvkhnh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gthenkkzbw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.redwolf501.top/gtyputekvu.html

[L04] 设置超时
来源：http://hz.jiagoushi.top/gtfmnofxbw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shzxlz.cn/gtxtojrgzw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.mhx1999.top/gtfseyryvm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtapqowdgm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtjjlxtuvy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangshuangyany.cn/gtmzxjhqes.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ehwqpu.com/gtwklsnbyq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtbimbvhrx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gtetogqzli.html

[L05] 上传文件（multipart）
来源：http://hz.daria6918.cn/gtyxhryojp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hysaishi.cn/gtrdmwjaah.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ehwqpu.com/gtioootpsu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.52xcode.cn/gtjrglyaer.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtlopletzv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgufenzy.top/gtxjiioaou.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.iojbl.cn/gtfbvgxdwe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gogol.net.cn/gtfrbozteb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jyoumei.cn/gtuzaphasb.html

[L06] 解析响应为 JSON
来源：http://hz.zhiwuduotai.top/gtchhgmggg.html

Py:   resp.json()
来源：http://hz.hnxiangtu.top/gtvhfvyuxd.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gtmqdvovil.html

JS:   await resp.json()
来源：http://hz.9152youxi.cn/gtllzlnhaq.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtiiorhnng.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xylfe.cn/gtmjsbbywe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.quarkkingdee.top/gtcyfayhrj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtwrcywzfj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jianghu66.top/gtpdssttsu.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtikylirpq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gttytzwepr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gtkjgtwosf.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtwgvwwkfs.html

TS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtunojaalz.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtuqavbhbr.html

Go:   resp.StatusCode
来源：http://hz.cashguo.top/gtxzcjrlpw.html

Ruby: resp.code.to_i
来源：http://hz.redwolf501.top/gtcpjofdtt.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtdsonvtab.html

[L08] 并发请求多个地址
来源：http://hz.hongshengwenyu.top/gtezdvxrfc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ywan-chungtsiang.top/gtfbhcntxx.html

PHP:  curl_multi_init() 系列
来源：http://hz.snrcjt.cn/gttihppkri.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtvhasdhxx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtvxdqcnyv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydzc1.top/gtxiglahur.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtzdgjpbgj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydzc1.top/gtmtjrasvo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuetiantiany.cn/gtfnymrbxn.html

================================================================================
来源：http://hz.nanxinkj.top/gtaiczhamz.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258888.top/gtslsdxcie.html

================================================================================
来源：http://hz.shuidangran.top/gtbhdkghjs.html

[M01] 读取命令行参数
来源：http://hz.pengpengdd.cyou/gtpwjluekd.html

Py:   sys.argv[1:]
来源：http://hz.shzxlz.cn/gtjcgsmmwk.html

PHP:  $argv;  $argc;
来源：http://hz.yj202588.top/gtkmniosbu.html

JS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtubonguft.html

TS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtuagkkbhq.html

Java: args 数组（main 方法参数）
来源：http://hz.aibaodan.cn/gtxnqfqdzv.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gtuzxlcrtf.html

Ruby: ARGV
来源：http://hz.52xcode.cn/gtqdafvibc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gtcjqzhltl.html

[M02] 读取环境变量
来源：http://hz.chenjidiqi.icu/gtxyvepmju.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtgmpvegdr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtbvzqcvad.html

JS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtldqebuhj.html

TS:   process.env.HOME
来源：http://hz.tanke756.top/gtaktylizg.html

Java: System.getenv("HOME")
来源：http://hz.ivvv.top/gtrevegkim.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hfpthk.cn/gtmbrakvoq.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangkeji.top/gtnxhjysav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtwxwrbmdw.html

[M03] 执行外部命令
来源：http://hz.kuanghao11.cn/gtwzmeabwx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtfgvxbgxu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtjpuvmcqe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtaavyjviz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtoitvaexw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtfudzepqz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtugchrtxa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtjajstend.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shangyingyoupin.top/gtwyqtqbtg.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtunloxinl.html

Py:   os.getcwd()
来源：http://hz.bjfxy.top/gtifthsoev.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gttkcmmnjh.html

JS:   process.cwd()
来源：http://hz.zdqjudy.top/gtdsstecgd.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gtzgedpply.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxuanxn.top/gtsktqvyub.html

Go:   os.Getwd()
来源：http://hz.jianghu66.top/gthvdjyedj.html

Ruby: Dir.pwd
来源：http://hz.yonumen.top/gtrvyrgsjk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nwbrower.top/gthrabkhze.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtwevkmcfl.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtmwqukoof.html

PHP:  exit(1);
来源：http://hz.vqdsnc.cn/gtjmgbleoa.html

JS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtmzhkiwec.html

TS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtudjvfdlu.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtalxafkee.html

Go:   os.Exit(1)
来源：http://hz.jyoumei.cn/gtjvssvgwx.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gtherfcbfy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgufenzy.top/gthzcwhfvt.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtfhicrray.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtbobruzfd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hfpthk.cn/gtebavngos.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtkazqydmm.html

TS:   console.error("err")
来源：http://hz.nwbrower.top/gtirnmmvix.html

Java: System.err.println("err")
来源：http://hz.ydjk.org.cn/gtlstcqtmy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtnydquxdh.html

Ruby: warn "err"
来源：http://hz.xuanzx.com/gtwjozcdgk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtlnavshlj.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtmpbfleur.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtoalxqeer.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.birdmap.top/gtojamjowi.html

JS:   require.main === module
来源：http://hz.dianchejie.cn/gtuxkhsvwd.html

TS:   require.main === module
来源：http://hz.tianlin.xyz/gtvogiijkr.html

Java: public static void main(String[] args)
来源：http://hz.hnxiangtu.top/gtpndglgib.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtpgaftniq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuanzx.com/gthtzxbnld.html

C#:   static void Main(string[] args)
来源：http://hz.shuidangran.top/gtfegwvgkq.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtjocychcq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.meibo888.top/gtaikmuetb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgfzy.top/gtmvecyqlt.html

JS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtjpgwhrnc.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtlmdkdduo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sufxvd.cn/gtozvmfpqt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.wangshuangyany.cn/gtbbslkpyg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.quarkkingdee.top/gtelyzenep.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtupjfudug.html

================================================================================
来源：http://hz.chenlongwang.top/gtrjwlsfax.html

N. 数据结构与算法
来源：http://hz.hongshengwenyu.top/gtjlhbwkuk.html

================================================================================
来源：http://hz.yangfankeji.com/gtspwzlqiv.html

[N01] 二分查找（有序数组）
来源：http://hz.hysaishi.cn/gtxaxpfweo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtyvctxzgl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zycfv.cn/gtjnuzrhll.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtvtdfyvav.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtlrbbgnbd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sysykeji.top/gtfzaemjyp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtnzsxqcme.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtbxrpuufl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtmxscasok.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ywan-chungtsiang.top/gtsnhoanrr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtjpuqzpmc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangdashe.top/gtindmtsbm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtwbroozup.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtjmjcufjw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cqqwz.cn/gtvmggswml.html

Go:   slices.Sort(arr)
来源：http://hz.daxiang520.top/gtdcygullc.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtkftywjqz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ybcxt.top/gtffuemiyp.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gtxggrvgak.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtqjtkuaas.html

PHP:  // 递归实现，或用 usort
来源：http://hz.kuanghao11.cn/gtbfkrcqvy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtaskkjzez.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gthkhfawwl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtsmyqfkla.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gtktleurxn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gzhubu.top/gtmyqhjkie.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sysykeji.top/gtadmufmzm.html

[N04] 斐波那契数列
来源：http://hz.jqgfzy.top/gtggpsolvo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtczwliokd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtrwjaeaju.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtrwjstthx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtegbrqrch.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jlsjyb.cn/gtfrltcmqm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cdnleiting.top/gtpdohlwfc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtjeqeofhr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtgxluejzb.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gtssjfmkhs.html

Py:   math.gcd(a, b)
来源：http://hz.yangfankeji.com/gtfujoiwmp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxinkj.top/gtzscietkz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtmjdhioog.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtpcvmfsud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zycfv.cn/gtohyerffa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cdnleiting.top/gtxdtpdkol.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gtrjgipjne.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gtccyczfte.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gtbsbvqbcz.html

Py:   s == s[::-1]
来源：http://hz.zhixingplan.top/gtqgdcdlbf.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtwupcpvnl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtdongiawa.html

TS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtyswvfguw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yongpay.top/gtmafacgui.html

Go:   // 双指针从两端比较
来源：http://hz.smart0.xyz/gtgtvureke.html

Ruby: s == s.reverse
来源：http://hz.dashuyun.cn/gtbnsxnjwn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtlfjvytvc.html

[N07] 两数之和（返回下标）
来源：http://hz.cheryme.top/gtlangdrod.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtdfjkelna.html


<!-- 参考信息 -->