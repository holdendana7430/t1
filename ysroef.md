代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.birdmap.top/gtbshdacsu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtjbxymfgi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtottqqcum.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.redwolf501.top/gtkmcredaa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gthbrptiva.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cqqwz.cn/gtvcqomppx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtgiaqpwmz.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuanzhike.top/gtdasvckfy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinghuilouyu.cn/gtdleijbmj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sxryk.cn/gtbfiqadgs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtwaodcedl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hfpthk.cn/gtdnxgnuav.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gthrsnxgor.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.meibo888.top/gtjougduga.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtbvjqhbki.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuetiantiany.cn/gtbqacghuk.html

================================================================================
来源：http://hz.dianchejie.cn/gtftgyfsda.html

K. JSON 与序列化
来源：http://hz.wangshuangyany.cn/gtyjbxejzd.html

================================================================================
来源：http://hz.0kj1m.cn/gttrvkfvmq.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinyuanbaomall.cn/gtmvhinqcz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gtlyxmfhsj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtxoehedak.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtsebhlizv.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtikqdlxcr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxinkj.top/gtkulbgcne.html

Go:   json.Marshal(obj)
来源：http://hz.ehwqpu.com/gtfcdimhng.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ywan-chungtsiang.top/gtflgpycpr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gtnlilvirf.html

[K02] JSON 字符串转对象
来源：http://hz.daxiang520.top/gtdybpcltt.html

Py:   json.loads(s)
来源：http://hz.9152youxi.cn/gtpadsjypi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtqrrqupqh.html

JS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtcqyequpi.html

TS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtqbquyuwg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xylfe.cn/gtqukczqaf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtysmnazhj.html

Ruby: JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtwisfnyfl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtzpcdqzgd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gzhubu.top/gtgaplnjny.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtjsvqofzz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtdqtbvqbp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtdbroytfh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtxrovanju.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daria6918.cn/gtbuyaijpv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigfzy.top/gtukhnnbxm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gthgnkrqnz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.meibo888.top/gtaoqxgekd.html

[K04] 读取 JSON 文件
来源：http://hz.hnxiangtu.top/gtrzvpeemf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yangfankeji.com/gtyyxjeehc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtbienfnog.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtintmdyoa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtgvkkqnnm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgufenzy.top/gtfytvrggi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtjroddcwm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.52xcode.cn/gtlwfawkno.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gtxkzehbah.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gttximrohu.html

Py:   copy.deepcopy(obj)
来源：http://hz.tanke756.top/gttobraicd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cdnleiting.top/gtclpvypgz.html

JS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtlhxlcexh.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtfdymwvgf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ppjwa.cn/gtglasnbqf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtehknygdc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtymnlcpim.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gteauxbwia.html

[K06] 解析 URL 查询串
来源：http://hz.tianlin.xyz/gtuxvdlmnx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtjjhormcr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tian-w.cn/gtopwyyxyi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtilhlqpsx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtsbtsexse.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cdnleiting.top/gtkmylgamk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtesijzici.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtnradjvfn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtehaqahlv.html

[K07] 进制转换
来源：http://hz.xinyue.icu/gtbbzrxsvf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jianghu66.top/gtmjiibxdg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dashuyun.cn/gtnnnboglw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtrealfjdn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtnfdgtsnx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtteckhzst.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tian-w.cn/gtvpzewggg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sweek.top/gtqzbqzwor.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yonumen.top/gtbqpzctei.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtoblmbgus.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtkuqkgwsx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daria6918.cn/gtucjfcdop.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtitfjwswx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtczqmzqfh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtkzdhizex.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtfkpubwgu.html

Ruby: Marshal.dump(obj)
来源：http://hz.shangyingyoupin.top/gtbljkwvoj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtlgsfdtwk.html

================================================================================
来源：http://hz.hammf.cn/gtjxcqxglp.html

L. 网络请求
来源：http://hz.zycfv.cn/gtzzmxeobu.html

================================================================================
来源：http://hz.chenlongwang.top/gtdltndsmz.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gtwosiwyuo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gtrmmktfhh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtwjyelymk.html

JS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtuyvjgbta.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtbbuvnhjd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.mhx1999.top/gtnytrlmwy.html

Go:   resp, err := http.Get(url)
来源：http://hz.vqdsnc.cn/gtahghlzxo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gthhoqjxfv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtdfjeduzb.html

[L02] 发送 POST JSON
来源：http://hz.mhx1999.top/gtmzonquqq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtzpxxtqvg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jiagoushi.top/gtyfbjucve.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtoggroiao.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtwsusqjzo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtrdovjmjm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.c1oappe.top/gtydtgswur.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtosnuwovc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jiagoushi.top/gtwtkhbxsk.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gttaqflakc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gthxavhjea.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtdawksalv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtcyzejrwp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtialamdib.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gtuuhppaht.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtuwncovlb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.svipenyu.cn/gteuivqepf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtaszcfxnl.html

[L04] 设置超时
来源：http://hz.cheryme.top/gtrooiyndn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhijiandao.cn/gthifgmzcj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ivvv.top/gtphkyedru.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtvjytarbb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtwxoauypa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtbvnmccwo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cashguo.top/gtgcyodzpv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtaidilvdw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xylfe.cn/gtcjkmuqvc.html

[L05] 上传文件（multipart）
来源：http://hz.aibaodan.cn/gtfmhyfosn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dianchejie.cn/gtmoqjtxwd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tianlin.xyz/gtlqunujdh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtbffhactw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtaqlvbwoy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zdqjudy.top/gtipuyphbz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ehwqpu.com/gtskvvemvn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gtarzjmqiy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangdashe.top/gtuctayknb.html

[L06] 解析响应为 JSON
来源：http://hz.wangdashe.top/gtzovngncz.html

Py:   resp.json()
来源：http://hz.guowangkeji.top/gtpylrzbdy.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gthqhaoyhf.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtwcchnkdc.html

TS:   await resp.json()
来源：http://hz.yangfankeji.com/gtdemadcfm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shangyingyoupin.top/gthpydwgxs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.svipenyu.cn/gtxaoodwbq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xinyue.icu/gtlfjaxclm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhengqikj.top/gtgxskbnop.html

[L07] 处理 HTTP 状态码
来源：http://hz.havefunace.top/gtlkfnfxbi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hammf.cn/gtaqulespi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gtnjuhyjbs.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtqbsxnmne.html

TS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtqcewsnry.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gttanzdsmz.html

Go:   resp.StatusCode
来源：http://hz.fengsongda.top/gtoljfosqe.html

Ruby: resp.code.to_i
来源：http://hz.tian-w.cn/gtkpheipym.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258888.top/gtqojcbmtr.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtmllipjlv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.haohaochexian.top/gtyrewqxop.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgufenzy.top/gtpisyowjo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtzpsfniye.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtjzjvbyvm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtzlroznks.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guannengcc.top/gtkdvwxrft.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.feifeiyinyue.top/gtcpgamynw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhaomingkeji.xyz/gtcicsncmt.html

================================================================================
来源：http://hz.tian-w.cn/gtmnactgfl.html

M. 命令行 / 进程 / 环境
来源：http://hz.guowangkeji.top/gtuxnwjwsd.html

================================================================================
来源：http://hz.chenlongwang.top/gtydprvuiv.html

[M01] 读取命令行参数
来源：http://hz.zhijiandao.cn/gtsmqwnsge.html

Py:   sys.argv[1:]
来源：http://hz.sufxvd.cn/gtgpqktybn.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258888.top/gtybysjciv.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtyotsjotn.html

TS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtyrmfdytg.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtncgckier.html

Go:   os.Args[1:]
来源：http://hz.hysaishi.cn/gtxufgtjfi.html

Ruby: ARGV
来源：http://hz.yvedp.cn/gtdsipjpfo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtpxppqapi.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtqlhvkith.html

Py:   os.environ.get("HOME")
来源：http://hz.zdqjudy.top/gthereruqc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtxailxgmj.html

JS:   process.env.HOME
来源：http://hz.haohaochexian.top/gtqmfkcnrb.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtpagppnyt.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gteksksdxv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtearhsols.html

Ruby: ENV["HOME"]
来源：http://hz.havefunace.top/gtzegisaqu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tianlin.xyz/gtjxkhnjnn.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtoohvixls.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtdoqvdagx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtfgdatebi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtzcfbqnjh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gttyvtohjz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtapqnikdb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtvvxsrjqe.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxuanxn.top/gtkejsdqlt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cashguo.top/gtznxkeaao.html

[M04] 获取当前工作目录
来源：http://hz.sysykeji.top/gtaltgtdwt.html

Py:   os.getcwd()
来源：http://hz.zhengqikj.top/gtgkcbltju.html

PHP:  getcwd();
来源：http://hz.nanxinkj.top/gthsravfky.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gtddemuoks.html

TS:   process.cwd()
来源：http://hz.andypj.xyz/gtbmikmpgv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuxming.cn/gtmoimnlkk.html

Go:   os.Getwd()
来源：http://hz.mhx1999.top/gtnjarspew.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gthepwnjys.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pengpengdd.cyou/gthynafjvd.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtxomquyfq.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtybleodsg.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtppdoezij.html

JS:   process.exit(1)
来源：http://hz.yj20258888.top/gtgolyvpda.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gthgzaubfc.html

Java: System.exit(1)
来源：http://hz.ehwqpu.com/gtcnswpvia.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtsolnooxj.html

Ruby: exit 1
来源：http://hz.daxiang520.top/gtpyclrvgs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtjexhyijs.html

[M06] 向标准错误输出
来源：http://hz.daria6918.cn/gtkmurtmqy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtlzwvaxvi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtgsdagfzo.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gteyxbtpqf.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtyoahqhak.html

Java: System.err.println("err")
来源：http://hz.316326.xyz/gtupixkwrm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zycfv.cn/gtgnhyskkv.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtullrkbwk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xinyue.icu/gtfkgpnura.html

[M07] 判断是否为主入口
来源：http://hz.aibaodan.cn/gtxmkysvfc.html

Py:   if __name__ == "__main__":
来源：http://hz.ydjk.org.cn/gtoallypbd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydjk.org.cn/gtigajrchx.html

JS:   require.main === module
来源：http://hz.sweek.top/gtyvdypsrt.html

TS:   require.main === module
来源：http://hz.chenzaomai.com/gtlmfjgziq.html

Java: public static void main(String[] args)
来源：http://hz.guowangkeji.top/gtnecxmueb.html

Go:   func main()
来源：http://hz.zdqjudy.top/gtnhimnfxl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gtzjgxaslj.html

C#:   static void Main(string[] args)
来源：http://hz.shzxlz.cn/gtfyljwohs.html

[M08] 获取系统与运行时信息
来源：http://hz.hongshengwenyu.top/gtnrlkqubj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtodxvynwt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.0kj1m.cn/gtcxbaaobm.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtwilllymu.html

TS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtslqxaalj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gaohongyu789.top/gtovtxrtnk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtneqqxomz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guowangkeji.top/gtunegziwd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtfmgsiphq.html

================================================================================
来源：http://hz.zhixingplan.top/gtcvtuumoc.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gtcrpysnol.html

================================================================================
来源：http://hz.gogol.net.cn/gtfgxqplpq.html

[N01] 二分查找（有序数组）
来源：http://hz.shuidangran.top/gtgmyerqec.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gtghocyiuu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gtuopwmwlw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtliwlacxd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtyiokijpg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shuidangran.top/gtdxfvvsvm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gtnaejfhhu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gtouagrajy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtdvxtlzvo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gtwwmxdsnx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtfsjuqfix.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.feifeiyinyue.top/gttceuixvl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtvulukbns.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtloeswrnq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnqzz.top/gtyhootkrx.html

Go:   slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtguphjlxe.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtpsqqbela.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gtdfzyvtml.html

[N03] 快速排序（分治示例）
来源：http://hz.hammf.cn/gtsvctkxbt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtjteqbgsx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtmskjasmb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtovyxmesb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtenzugqia.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.guowangkeji.top/gtdeivyetj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gaohongyu789.top/gtsaqigktu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xinyue.icu/gtpgjguqzv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hammf.cn/gtitephvhz.html

[N04] 斐波那契数列
来源：http://hz.andypj.xyz/gtpnmmdpma.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ppjwa.cn/gtpcwnbqpu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtcfycbiqp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtiegtmqnb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtjpqideeu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xziqi.cn/gtrexlzxfj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangtech.top/gtulyowyxs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtprtzpvaz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtjcasnglm.html

[N05] 最大公约数
来源：http://hz.zycfv.cn/gtctleqpdi.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtzywzrctp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.9152youxi.cn/gtbqpakswp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtsrnnrpqr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gttehocdpu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.snrcjt.cn/gtlcpthiwo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhixingplan.top/gtjkgplwkb.html

Ruby: a.gcd(b)
来源：http://hz.hywenlv.cn/gtfkqrbwwa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtvybfywef.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gtoqcivsmv.html

Py:   s == s[::-1]
来源：http://hz.tanke756.top/gtbddykboh.html

PHP:  $s === strrev($s);
来源：http://hz.jiagoushi.top/gttbsotgtv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtzgjrwfzl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtcryetyci.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinghuilouyu.cn/gtfrmciywo.html

Go:   // 双指针从两端比较
来源：http://hz.chenjidiqi.icu/gtdtrhghet.html

Ruby: s == s.reverse
来源：http://hz.hongshengwenyu.top/gtakogjqdg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gthookyojo.html

[N07] 两数之和（返回下标）
来源：http://hz.sweek.top/gtuxefmyee.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tianlin.xyz/gtfjygbygw.html


<!-- 参考信息 -->