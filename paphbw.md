代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuetiantiany.cn/gtspshqior.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtcqowtlwc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhoulong.xyz/gttgmmtres.html

[J10] 取今天 / 本月第一天
来源：http://hz.ivvv.top/gtdcjzdvpf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gtezassqho.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shuidangran.top/gtinrelwmf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ivvv.top/gtilxkybha.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sweek.top/gtervfkzco.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shuidangran.top/gtkpewitbq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtjumjfxxh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258.top/gtbnakjwhu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jiagoushi.top/gtwewvtflb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtubsvxcns.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gtggwjdmev.html

================================================================================
来源：http://hz.hnqzz.top/gtsggmgnfr.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtnwpqjqwr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtehrtsvdm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtqfqgosfm.html

JS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtjrgkjwnz.html

TS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtuncdrzuv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hfpthk.cn/gtylfwwnxq.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtebhllivp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fzhhl.top/gtahsijgmd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtvcaxqdtl.html

[K02] JSON 字符串转对象
来源：http://hz.hnqzz.top/gtcdxmhfoz.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtwudaimhl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenjidiqi.icu/gthsivsnlh.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtrzjuiyfb.html

TS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtakqpgkvd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xziqi.cn/gtcbwdfgnz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtfjpyucuq.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtqeoxuzen.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.haohaochexian.top/gtnjgnowfg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuanzhike.top/gtbyslnimk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtyzuyvqdz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtbcvvkokk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtipiepwqe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtsmclhtjg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258.top/gtadgpowau.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangshuangyany.cn/gtnrbsgxjy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenlongwang.top/gtpmeliwyc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gtpoevvgxr.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtnpoftgwq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gotoacloud.top/gtfydhttzx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnqzz.top/gtitjsktrc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gthkmtskrm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtewsfriuw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhijiandao.cn/gtsstktvor.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtmrxnojlb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gtkocsavqu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yueranfly.top/gtghwcbexq.html

[K05] 深拷贝对象
来源：http://hz.dianchejie.cn/gtbjnrlbtr.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangkeji.top/gtykzsklct.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinyuanbaomall.cn/gtynozmjex.html

JS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gttgaxdbcy.html

TS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtgdxpuerb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigufen.top/gtahtxawlh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yongpay.top/gtlcarbipd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtngapalgr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuxming.cn/gtqvjtlhrg.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gtmvgdwccc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtrbfcftmb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtvjqxqmje.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtmsdlilfk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtpysagrih.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gttpzxkojf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuanzhike.top/gttyzmpjfm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtcdeewhus.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtmehaqqls.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gtgyvjapqj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigfzy.top/gtxcggzlyo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtgzcqkvxs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtehtaaymw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtabfmozpe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtqoyfnkta.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangtech.top/gtftbbmwzn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xylfe.cn/gtpkoxfcfl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daria6918.cn/gtaoztqpul.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtdudzvpuk.html

Py:   pickle.dumps(obj)
来源：http://hz.daxiang520.top/gtdxxmwrse.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xziqi.cn/gteseiwpen.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtanhacwmp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtgflwlmyj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtibrpzpji.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtihpoaeuc.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtmenhrgxs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gtsfkkptjy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfhlctisd.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtfbkkldfi.html

================================================================================
来源：http://hz.hnqzz.top/gtuszylzhb.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtmxaoopqc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guannengcc.top/gtktbznhal.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gtriavfrdf.html

JS:   await fetch(url)
来源：http://hz.zycfv.cn/gtiqtkefll.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtoazyfhbj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtgindnbqa.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenzaomai.com/gtkedfyget.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gtovdcywfx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gzhubu.top/gtvsnbcwhl.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gtlbatgbde.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.iojbl.cn/gtlyrbzvsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.guannengcc.top/gtnqfhkwag.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtczsqapeo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtdrscfdsc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ppjwa.cn/gtdljjwsjg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.andypj.xyz/gtktankrxw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ppjwa.cn/gtsfopvhxl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtplsgglht.html

[L03] 设置自定义请求头
来源：http://hz.yanxiufei.cn/gtlrxkcuqw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gtsbzdoqgv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.c1oappe.top/gtkapktewn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gteyihgkdu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtnldpplof.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shzxlz.cn/gtfuyufotd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hammf.cn/gtmvwjsrdy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtykbvuaiw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtmxjhwyzz.html

[L04] 设置超时
来源：http://hz.sxryk.cn/gtdbnvkkkm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cucudq.cn/gtkntavpgw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xinyue.icu/gtxfhtdben.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtmhfczbdx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtnhlmpzyr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tian-w.cn/gtdxcdoxgj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtkxfxoeoe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nwbrower.top/gtukpzddid.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aizwys.cn/gtcwsdexnd.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gttlkirdtx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aibaodan.cn/gtnkfhqjgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jianghu66.top/gtgpjxaplu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtdgrxqcxr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtuucjeide.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gtkximkhdl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gthlcgrggf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnxiangtu.top/gtgjxmezpj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hammf.cn/gtigssnlgt.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gtuvwgpqyn.html

Py:   resp.json()
来源：http://hz.mhx1999.top/gttkmspwmg.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtjjmmxfzr.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtexqsaght.html

TS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtopbdmyrz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tian-w.cn/gtkkgzvpnw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtsqevbfgy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.iojbl.cn/gthizxpzyg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangkeji.top/gtiwehlhjl.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258888.top/gtmcgntqpj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sxryk.cn/gtgwljzqiv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tianlin.xyz/gtfnkewwht.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtfcveehol.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gticmekvre.html

Java: resp.statusCode()
来源：http://hz.feifeiyinyue.top/gttxjsisrv.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtpfrzisig.html

Ruby: resp.code.to_i
来源：http://hz.andypj.xyz/gtiynldrka.html

C#:   (int)resp.StatusCode
来源：http://hz.meibo888.top/gtenfugucb.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtshamhtys.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhoulong.xyz/gtohvenrnk.html

PHP:  curl_multi_init() 系列
来源：http://hz.mhx1999.top/gtfwerfayr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtzbtptppe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gthrsjxkqj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gtrzxwartb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtuzqauynd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtgcfeercj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sxryk.cn/gttagbgjxo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmidqnsbz.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gturlsniwm.html

================================================================================
来源：http://hz.c1oappe.top/gtcviwyrmn.html

[M01] 读取命令行参数
来源：http://hz.nanxinkj.top/gtiaxbhlyl.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gtshilmnnd.html

PHP:  $argv;  $argc;
来源：http://hz.jqgufenzy.top/gtfhiswowv.html

JS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtcgphrxgc.html

TS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtmjenanuf.html

Java: args 数组（main 方法参数）
来源：http://hz.zhoulong.xyz/gtehpfyprh.html

Go:   os.Args[1:]
来源：http://hz.nanxuanxn.top/gtpdzelrye.html

Ruby: ARGV
来源：http://hz.gotoacloud.top/gttrqntrtg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tanke756.top/gtpzcnjcmn.html

[M02] 读取环境变量
来源：http://hz.gogol.net.cn/gtbzthxteo.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gtbtudilfa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtpxgikkbh.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtakzijqld.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtczhyxbbz.html

Java: System.getenv("HOME")
来源：http://hz.iojbl.cn/gttdqhwstw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tanke756.top/gtxuudjsjt.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtklkhzewv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydzc1.top/gtuncdwkoe.html

[M03] 执行外部命令
来源：http://hz.9152youxi.cn/gtkcdxvfaf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtynrbsscd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gttylxjrhx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtntxmrgza.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtptzoeweo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yongpay.top/gttrkdszlu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtfjhdzvsn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhijiandao.cn/gtfeqphmhw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtwsfmefaw.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangkeji.top/gtfkgzpaha.html

Py:   os.getcwd()
来源：http://hz.nanxinkj.top/gtugismdid.html

PHP:  getcwd();
来源：http://hz.sufxvd.cn/gtqlgblvlo.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtyqcsisuh.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gthylsyqlx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yueranfly.top/gtwsnimroc.html

Go:   os.Getwd()
来源：http://hz.jinqigufen.top/gtyutaciic.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtdjqvuoar.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtlbaqxtzs.html

[M05] 设置退出码
来源：http://hz.0kj1m.cn/gtbleioaay.html

Py:   sys.exit(1)
来源：http://hz.yuxming.cn/gtzcovfrpf.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtpicgghhu.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtuivbfdxl.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtaolvssoy.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtzchzouja.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangtech.top/gtgevocpzc.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtkzhxngab.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gogol.net.cn/gtsisjwgfv.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtoxjzvezn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtbjatbote.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jyoumei.cn/gtnjzinsks.html

JS:   console.error("err")
来源：http://hz.xylfe.cn/gtcroeakuu.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtnbxnprxs.html

Java: System.err.println("err")
来源：http://hz.yonumen.top/gtyrezztba.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtygmzeurm.html

Ruby: warn "err"
来源：http://hz.sweek.top/gtwybjvges.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gotoacloud.top/gtxvddffbu.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtcluugkvm.html

Py:   if __name__ == "__main__":
来源：http://hz.dashuyun.cn/gttxedqyuz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtqzdfnckw.html

JS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtsoqbrnpz.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtpaeakxzr.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtxssmtwsz.html

Go:   func main()
来源：http://hz.jinghuilouyu.cn/gtwujeorsj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtebginsww.html

C#:   static void Main(string[] args)
来源：http://hz.jinghuilouyu.cn/gtkaiiqtqc.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtllpeusnt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jqgufenzy.top/gtqmkirypr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gtwkgafqts.html

JS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtqgxyxden.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtewnbesiw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.svipenyu.cn/gtzqyuglks.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhijiandao.cn/gtguvsanfs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xingfuxueyuan.xyz/gttgykxqvz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.havefunace.top/gtfblfxkwr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtkyxcmhuj.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gttnlezinr.html

================================================================================
来源：http://hz.yonumen.top/gtrucziadv.html

[N01] 二分查找（有序数组）
来源：http://hz.meibo888.top/gtvdvbiqun.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gtuclxsykq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hammf.cn/gtejrrelzw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtzoliewmf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtvrbbanim.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtophzgnnb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtsrpkeari.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtzlwwwdyd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtyvwmvucr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.feifeiyinyue.top/gtlkhehcfe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtmyetyemw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.c1oappe.top/gtnbqbzxko.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtxxzqtocv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtkkqbxdsp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj202588.top/gtelqaeuvz.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtpcikanem.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtugsvrsxn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cashguo.top/gtisxiqepa.html

[N03] 快速排序（分治示例）
来源：http://hz.gaohongyu789.top/gtdeejptkc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shangyingyoupin.top/gtzrxbxgld.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daria6918.cn/gttbugvgef.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtrudhkwqp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gtbtcuctzz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gtnjkxttxj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtkydrioqx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gttyeuftst.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hysaishi.cn/gtfqiiiwki.html

[N04] 斐波那契数列
来源：http://hz.9152youxi.cn/gtekaksvou.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtxjqagvme.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gtpncezdet.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gtpfumzaju.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtsqlzfybt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jyoumei.cn/gteyuljmuv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gttgxfxvbh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtyggkkgwg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.316326.xyz/gtkguidwif.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtzzehqyic.html

Py:   math.gcd(a, b)
来源：http://hz.xylfe.cn/gtgbsvlaoe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtbshtwmma.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtkmgenrcs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtdbowdlns.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtyicpcaeu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hammf.cn/gtpzrzwduz.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtoljgqrty.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dashuyun.cn/gteqreozgy.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtrscunkpd.html

Py:   s == s[::-1]
来源：http://hz.ydzc1.top/gtjldwwctv.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtwlwqsvbb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtfxlsptxs.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtayrwhhqd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cheryme.top/gtrpodopin.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtxikqwrmz.html

Ruby: s == s.reverse
来源：http://hz.quarkkingdee.top/gttbcjrtce.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.quarkkingdee.top/gttxvjasjz.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtoatsaxhy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtnrnjurpu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gogol.net.cn/gtfyiksbid.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhoulong.xyz/gtyhhcgiep.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtmzfaejyp.html

Java: // 手写 HashMap
来源：http://hz.daria6918.cn/gtrwxfzsvm.html


<!-- 参考信息 -->