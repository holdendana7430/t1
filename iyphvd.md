代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shzxlz.cn/gtteylwskt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtoawfinyv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtvthvihae.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtzzzuafdi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtbkpvccoh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.snrcjt.cn/gtasynvoeu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jyoumei.cn/gthuswllbq.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtcmkbdqno.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pengpengdd.cyou/gtuyzszpph.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ehwqpu.com/gtubzhqzpe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gotoacloud.top/gtlzzkpqmt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.daxiang520.top/gtttdwozah.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xylfe.cn/gtbdcdmfpi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aibaodan.cn/gtvsxwlnyb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.0kj1m.cn/gtsjiqwtvt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtwsvikakk.html

================================================================================
来源：http://hz.sxryk.cn/gtwizwjkdr.html

K. JSON 与序列化
来源：http://hz.ehwqpu.com/gtwthlvpty.html

================================================================================
来源：http://hz.redwolf501.top/gtsjyxhzgv.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtsjooaizb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtpwemzrle.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtrsarutee.html

JS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtifoayfvq.html

TS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtglyjeltv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fzhhl.top/gtdgxtexbr.html

Go:   json.Marshal(obj)
来源：http://hz.9152youxi.cn/gtfdlshheg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gzhubu.top/gtxdbjodfj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gzhubu.top/gtkuhlimkr.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtjrzrfksc.html

Py:   json.loads(s)
来源：http://hz.chenjidiqi.icu/gtadajezih.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gtmzqolifk.html

JS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtrdrezsrj.html

TS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtoedzqanf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gtgeilhjmq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gttjmqdphl.html

Ruby: JSON.parse(s)
来源：http://hz.jiagoushi.top/gtytitzwez.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtbcxwzmkp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.havefunace.top/gtoikjzalw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtjnsaaapn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtvuyznncy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtssxnhtnq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtwyfvybxv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtnheasyec.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhongyouzk.top/gthmjdttre.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.bjfxy.top/gtkcnttizg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.316326.xyz/gtntwwpcvb.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtzovqxhwj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.andypj.xyz/gtxabkfvgg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gtlffemjvv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gthnqthhir.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtijzkvgyy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtifetfdqb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtksquhdvl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hywenlv.cn/gtplltygus.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gthmlmioep.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtoaitoraw.html

Py:   copy.deepcopy(obj)
来源：http://hz.iojbl.cn/gtmzgzhbtb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangkeji.top/gtitgvalmz.html

JS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtfoxiainn.html

TS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtmlnimdwz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtxrgmgjgu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dianchejie.cn/gtmkwlmmee.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhijiandao.cn/gtrgezxmaa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sweek.top/gthrposwzy.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtsfzwqhbw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtdscungwb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.haohaochexian.top/gtzdprtmjp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtugwvfxga.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtnhpvnirg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtfxtzoevy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yueranfly.top/gttspslmbj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtjrmxyzii.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gtyyuhghvy.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtndmjxtrz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtudwkcssy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gtxenvemfe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gthfsfbpmr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtblsiwonp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtbglvhqpu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtlgqgawjx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gtfjfbwswu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xziqi.cn/gtnqmhgrmx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtfvlfrzie.html

Py:   pickle.dumps(obj)
来源：http://hz.wangdashe.top/gtnnsaluhe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sxryk.cn/gtzlgbtsph.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtnlivcjvb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtrtrmngor.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aizwys.cn/gtacmwbbsw.html

Go:   encoding/gob
来源：http://hz.chenzaomai.com/gtidzgmfuj.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtjpmgqwvn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtxqhomgeg.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkqrojhjf.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gtfrgjmaif.html

================================================================================
来源：http://hz.hysaishi.cn/gtzqdeqjnc.html

[L01] 发送 GET 请求
来源：http://hz.jinghuilouyu.cn/gtnityolqk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtidqfgdji.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhengqikj.top/gtqkvqbjng.html

JS:   await fetch(url)
来源：http://hz.daria6918.cn/gtunoawrdb.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtacicdcoh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daxiang520.top/gtgdbhlveh.html

Go:   resp, err := http.Get(url)
来源：http://hz.hywenlv.cn/gtqfnggilo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtdburohwu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gzhubu.top/gtcygtrfys.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gtffufrwiz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhongyouzk.top/gtidvgdlok.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.316326.xyz/gtuwvqyxjd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtfvmighsh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtpflroogr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtxvzhmnwa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.c1oappe.top/gtdhyffpbk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jiagoushi.top/gtcdonjdhf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhaomingkeji.xyz/gtwgyvzube.html

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gtmogjakva.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtvgloxaxp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtmruwoeqc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xingfuxueyuan.xyz/gtilljaziw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtljywrjmo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtumedqwsh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtqkcsyaep.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydzc1.top/gtbeqlnygb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtckvtenyk.html

[L04] 设置超时
来源：http://hz.316326.xyz/gtavtyzvvt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.smart0.xyz/gtmbhalvpf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yangfankeji.com/gtfhqfesrg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtsbknywri.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtugjakmyf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtxggxujwa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pengpengdd.cyou/gtlbtqxxfc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gtwzahrfdo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cqqwz.cn/gtcibajusj.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtbnthofdp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtsdugybdr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zdqjudy.top/gtwdaiwijc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtnhpyrosy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtrphtjptc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tanke756.top/gtrpskfuku.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pycfn.com/gtngmwaaob.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtkrueinpy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj202588.top/gtiwdxevsu.html

[L06] 解析响应为 JSON
来源：http://hz.c1oappe.top/gtnafqbaar.html

Py:   resp.json()
来源：http://hz.gzhubu.top/gtqrdtyotw.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtvgzskuuw.html

JS:   await resp.json()
来源：http://hz.pycfn.com/gtgpaviirm.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtblmqvtyc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.meibo888.top/gtfkkffetv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtntjohdag.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangshuangyany.cn/gtfupmnrdr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sweek.top/gtglbpwuxv.html

[L07] 处理 HTTP 状态码
来源：http://hz.jyoumei.cn/gtmyyrfqpy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.c1oappe.top/gtkrpognkn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258.top/gtyjqnnofs.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtljamgzxe.html

TS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtbvlnsdxl.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gtiymxewdo.html

Go:   resp.StatusCode
来源：http://hz.sufxvd.cn/gtistvshyr.html

Ruby: resp.code.to_i
来源：http://hz.hnqzz.top/gtkrsiggia.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gttkaknsmp.html

[L08] 并发请求多个地址
来源：http://hz.9152youxi.cn/gtnpsvodpf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gtugbnfqdt.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtkvtjbljy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtdcvdfzxe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtddporyrg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtuugfwutg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cheryme.top/gtedwkpysy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtmzyprcqh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gotoacloud.top/gtnjsjspzq.html

================================================================================
来源：http://hz.xinyue.icu/gtwbdnwein.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtmygobzot.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdcuspcqq.html

[M01] 读取命令行参数
来源：http://hz.gogol.net.cn/gtjpzfbpca.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtqojjhikq.html

PHP:  $argv;  $argc;
来源：http://hz.shuidangran.top/gtljbuugay.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtrnynafdb.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gttghtsepw.html

Java: args 数组（main 方法参数）
来源：http://hz.meibo888.top/gtweevsepx.html

Go:   os.Args[1:]
来源：http://hz.haohaochexian.top/gtwdoxlprs.html

Ruby: ARGV
来源：http://hz.jinyuanbaomall.cn/gtitpkjgwt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtdaiedvvh.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtjvrwpqpc.html

Py:   os.environ.get("HOME")
来源：http://hz.mhx1999.top/gtlqjlhfxt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxinkj.top/gtomqaaydh.html

JS:   process.env.HOME
来源：http://hz.cucudq.cn/gtlbefivnb.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtmmwihdfi.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtfwbwzxjm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yangfankeji.com/gtgaozcbnk.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtxqkykpne.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fengsongda.top/gtmtfduvkh.html

[M03] 执行外部命令
来源：http://hz.ybcxt.top/gttszexduj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtiiwvnbik.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgufenzy.top/gtgtkbqumw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtmhhpladp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtblxdxoyy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.9152youxi.cn/gtikewhgdq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zdqjudy.top/gtmygwjihu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtboavbmxj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhixingplan.top/gtmhtquxuf.html

[M04] 获取当前工作目录
来源：http://hz.chenzaomai.com/gtujqdradl.html

Py:   os.getcwd()
来源：http://hz.ydjk.org.cn/gtmckpxjfu.html

PHP:  getcwd();
来源：http://hz.nanxinkj.top/gtgfbcgcxl.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtkffmywal.html

TS:   process.cwd()
来源：http://hz.hywenlv.cn/gtvowelskz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jianghu66.top/gtctknebah.html

Go:   os.Getwd()
来源：http://hz.pycfn.com/gtzxeazkiy.html

Ruby: Dir.pwd
来源：http://hz.quarkkingdee.top/gtxcbcmuai.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xingfuxueyuan.xyz/gtekxiozsv.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtfebualsk.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtdcuttqqg.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gtnpslbpwc.html

JS:   process.exit(1)
来源：http://hz.bjfxy.top/gtddkbarrf.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gtdipwkkha.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtspjgquve.html

Go:   os.Exit(1)
来源：http://hz.gotoacloud.top/gtxtunevcc.html

Ruby: exit 1
来源：http://hz.sweek.top/gtflrisoov.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenlongwang.top/gtcrdhjfbt.html

[M06] 向标准错误输出
来源：http://hz.hnqzz.top/gtenrctfai.html

Py:   print("err", file=sys.stderr)
来源：http://hz.9152youxi.cn/gtwyufjenq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daria6918.cn/gtvqkgyrzu.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtufztsmkn.html

TS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtaxdynjtx.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtoykjmkba.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jianghu66.top/gtmjtukokn.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtcynuymkd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258888.top/gtnnlqobls.html

[M07] 判断是否为主入口
来源：http://hz.andypj.xyz/gtdbucvaln.html

Py:   if __name__ == "__main__":
来源：http://hz.jiagoushi.top/gtioatchgu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj202588.top/gthirbixvq.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtyumlgksj.html

TS:   require.main === module
来源：http://hz.tian-w.cn/gtnuizobmp.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gtvwtpcawd.html

Go:   func main()
来源：http://hz.yuxming.cn/gttlnillfj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtbaenbfew.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtpkzzvcbt.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gthcyfqvtn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtyhfzertr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtfxmozkbx.html

JS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtmgnvmjnf.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtoqhwyfbq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.kuanghao11.cn/gtwlutkozn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtgiqcimme.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gtgkaxdvin.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydzc1.top/gtceklnstq.html

================================================================================
来源：http://hz.yuxming.cn/gtlgguqbyd.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtjidcqiep.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlsuqgouw.html

[N01] 二分查找（有序数组）
来源：http://hz.guannengcc.top/gtaqipsmzm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guowangkeji.top/gtynithtbr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtdwjyghkj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tanke756.top/gtnqagsckb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtoqelbuxb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtlrsuxkvf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jyoumei.cn/gtjibayaot.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daria6918.cn/gtswjjgvga.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtstzcpzid.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gtdgdvohna.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtlkefspop.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ehwqpu.com/gtuoubfshy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtvujjcrxv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtvafqozgq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtysgihqpr.html

Go:   slices.Sort(arr)
来源：http://hz.hnqzz.top/gtlmcuquja.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtmqjovoyz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxinkj.top/gthfvpzfjp.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gtwaizphza.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhijiandao.cn/gtbbkfozvw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ydjk.org.cn/gtaoatnhqj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtzkcoaxmj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtdmofvyfh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hysaishi.cn/gtfgqqcslj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hongshengwenyu.top/gtxmcjibke.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shuidangran.top/gteuqraksm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yanxiufei.cn/gtwpxugklx.html

[N04] 斐波那契数列
来源：http://hz.wangdashe.top/gtvakefxza.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gteegytyjm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtncftmrnh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jiagoushi.top/gtazkqabzv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtyvvhnbkb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuanzx.com/gtabdxnscw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhoulong.xyz/gtjljevogs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gtbdrvpvxm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jianghu66.top/gtzabccpln.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gthhakeuka.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtzgjcgsbd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daria6918.cn/gtelkwlsnn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtoxdtugrk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtalxxgsfl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yonumen.top/gtejylphmu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.52xcode.cn/gtrnhyeudd.html

Ruby: a.gcd(b)
来源：http://hz.jyoumei.cn/gtiahbwivf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.meibo888.top/gtvgxejefu.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtyqmytude.html

Py:   s == s[::-1]
来源：http://hz.ybcxt.top/gtxcprqiat.html

PHP:  $s === strrev($s);
来源：http://hz.guannengcc.top/gtmtplhers.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtzmfncyhn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtcxytweux.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258.top/gtuxexdgfl.html

Go:   // 双指针从两端比较
来源：http://hz.wangdashe.top/gtpalarupf.html

Ruby: s == s.reverse
来源：http://hz.9152youxi.cn/gtylwmuunp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtktnjufxz.html

[N07] 两数之和（返回下标）
来源：http://hz.daria6918.cn/gtdbxnvlpn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guannengcc.top/gtoaliwlok.html


<!-- 参考信息 -->