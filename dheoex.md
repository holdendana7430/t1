代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.c1oappe.top/gthcyxyzxt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtzqcjugdy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gtxdqgsfeq.html

[J10] 取今天 / 本月第一天
来源：http://hz.aibaodan.cn/gtxhzmntgn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydzc1.top/gtbtxvaufe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtjwnuvzws.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtkrolbmsu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ybcxt.top/gtepiuwtau.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258888.top/gtdplzutsp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jianghu66.top/gtojayjnit.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.quarkkingdee.top/gtrnfhdvnw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gtdcgqthkc.html

================================================================================
来源：http://hz.tianlin.xyz/gtkczryemj.html

K. JSON 与序列化
来源：http://hz.dianchejie.cn/gtkbnafocw.html

================================================================================
来源：http://hz.fengsongda.top/gtbstvahjf.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigfzy.top/gtcqppxlbo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gthglzlumu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gtrpcpmaqu.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtkfxcuqta.html

TS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtfwroockq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258888.top/gtqnahaazw.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gteiyrnjwx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtwsawdrwr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgufenzy.top/gtbkvtjnan.html

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gtutfbouph.html

Py:   json.loads(s)
来源：http://hz.cheryme.top/gtyxbsgahm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinyuanbaomall.cn/gtokachrvl.html

JS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtyvhjdlfc.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtiomdxrea.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yanxiufei.cn/gtnxmvkytt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtetyxhrmq.html

Ruby: JSON.parse(s)
来源：http://hz.gogol.net.cn/gtjyiunzmc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pengpengdd.cyou/gtiztjexed.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aibaodan.cn/gtyrybduoa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.birdmap.top/gtptgovnmp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtqaucwfhz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ivvv.top/gtxldffymi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtlkeaefda.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhijiandao.cn/gtdqcpqxfm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gtuzyvffpt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgufenzy.top/gtmzepgcyx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gtvirursnd.html

[K04] 读取 JSON 文件
来源：http://hz.iojbl.cn/gtfazyistp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ybcxt.top/gtnjpkoixu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.havefunace.top/gtboepeeqa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtqnjrbgpf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtyqgztjiu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtqfahgemo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtnjyzuuxe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pycfn.com/gtokqlxmds.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gtbdbtlwrx.html

[K05] 深拷贝对象
来源：http://hz.xingfuxueyuan.xyz/gtsqeeqzpw.html

Py:   copy.deepcopy(obj)
来源：http://hz.redwolf501.top/gtobtvkqrp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtllqokmjb.html

JS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtnfhkmtob.html

TS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtuelrhvjz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj20258888.top/gtkorgodob.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sweek.top/gtsslwrjfu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtvkkzweds.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtoswebyvu.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtoblqgmcb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtbtgqltnp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhaomingkeji.xyz/gtzrwcqfin.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtknmafpnw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtttvcfopm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtqrtcvkwq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtsuqjtmwa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgfzy.top/gtkvmsnvqe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtsmwurwtp.html

[K07] 进制转换
来源：http://hz.cdnleiting.top/gtytdvsxba.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtclwemxoa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtvhxbaupw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtkmeksfnu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtwgsilyns.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtcqzbiykp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtnijoayju.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sweek.top/gtgppcshsx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gttlnuwfvw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtjiwejczy.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtqrgjudwl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtiqmlipqg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtmlshxybr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtbrcbitjb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtjkwwbgpr.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtiflayvqn.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangtech.top/gtkyepbppf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jiagoushi.top/gtyjktcjvm.html

================================================================================
来源：http://hz.tianlin.xyz/gtharvxceq.html

L. 网络请求
来源：http://hz.bjfxy.top/gtpqzjtkol.html

================================================================================
来源：http://hz.sufxvd.cn/gtmqysfrez.html

[L01] 发送 GET 请求
来源：http://hz.yangfankeji.com/gtohfthmkj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gthnhqmliw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnxiangtu.top/gtznwxbrcf.html

JS:   await fetch(url)
来源：http://hz.nanxinkj.top/gthstuswuz.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtqotbfmle.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xylfe.cn/gtsrmxahpy.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenjidiqi.icu/gtedbnraqf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jiagoushi.top/gtreuxpyiu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtnddcxqku.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtbxxnpdii.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigufen.top/gtfcegvvrx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nwbrower.top/gtmhbgqkmt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtadmkytsj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtwwnjpxeh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daxiang520.top/gtjmcmfkhv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtohggzsgx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.0kj1m.cn/gtpxhrjakr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ybcxt.top/gtezosocwc.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtygwdegql.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ywan-chungtsiang.top/gtzjyjhjfq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258.top/gtqsduwocq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtnddaimec.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtfyanyckj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.52xcode.cn/gtanhymeic.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtgnoraeeu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.c1oappe.top/gtlgjjyzda.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtspwdegvb.html

[L04] 设置超时
来源：http://hz.tian-w.cn/gtkpoclmah.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hongshengwenyu.top/gtoxkljwyf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ybcxt.top/gtpxuhoxlw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtriyfqlcv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtaagiltls.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj202588.top/gtoecgxkxf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pengpengdd.cyou/gtfttqsyug.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.redwolf501.top/gtazacuzkt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuxming.cn/gtglebtvrw.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtcaokwfkh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yangfankeji.com/gtmiaqvvpx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dianchejie.cn/gtzfdxaenz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gthaaovbjt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtwxbikbfg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gthbtsxopw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.birdmap.top/gtvisjvgdi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yvedp.cn/gtelqttbiu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gtfahffpzu.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigufen.top/gteitkcqjn.html

Py:   resp.json()
来源：http://hz.yj202588.top/gteengorpl.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtkyjdztjw.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtpptzvidj.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtlcvidmaq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.meibo888.top/gtczkmygxu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ppjwa.cn/gtgjowmeod.html

Ruby: JSON.parse(resp.body)
来源：http://hz.snrcjt.cn/gtcuacfxtz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtkhonfcgl.html

[L07] 处理 HTTP 状态码
来源：http://hz.tanke756.top/gtincvngok.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jiagoushi.top/gtlqolcvkm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtzswdpsjy.html

JS:   resp.ok;  resp.status
来源：http://hz.shzxlz.cn/gtcfmrdqgw.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtvtkzypil.html

Java: resp.statusCode()
来源：http://hz.nanxuanxn.top/gtqmggazfl.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtnpdocosj.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtebbfjjxw.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtwbuxbqkw.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtchfxrham.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sysykeji.top/gtojsladjl.html

PHP:  curl_multi_init() 系列
来源：http://hz.zdqjudy.top/gtlxvxxsgm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtpzoilvhh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtzxfisbev.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jyoumei.cn/gtmlbejnky.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtsgwyldth.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtzboyzmpj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gtyzoqxznl.html

================================================================================
来源：http://hz.daria6918.cn/gtfnjqnkyr.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangdashe.top/gtfioftfrx.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrfnonabb.html

[M01] 读取命令行参数
来源：http://hz.ppjwa.cn/gtmhefgiex.html

Py:   sys.argv[1:]
来源：http://hz.tianlin.xyz/gtyifxiphd.html

PHP:  $argv;  $argc;
来源：http://hz.daria6918.cn/gtbtnbulql.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtueanitvf.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtcminkffp.html

Java: args 数组（main 方法参数）
来源：http://hz.fengsongda.top/gthggfggwq.html

Go:   os.Args[1:]
来源：http://hz.hnxiangtu.top/gtrgzelolt.html

Ruby: ARGV
来源：http://hz.vqdsnc.cn/gtjvsbwnnp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hfpthk.cn/gtqmnfyvsw.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtkeztccgp.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtluknmtqu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydzc1.top/gtbzyubgnj.html

JS:   process.env.HOME
来源：http://hz.tanke756.top/gtomhcbbxa.html

TS:   process.env.HOME
来源：http://hz.9152youxi.cn/gtaybbyevf.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gtmjojllty.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zycfv.cn/gtxbfrzzym.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtacbnqyia.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtlfdfazrl.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gtwqarexxe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtdjbimetm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuanzx.com/gtbvrylbom.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtclaommpm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtaxjenouj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtvempmqji.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtajuaqxqz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtsabyqzde.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gtgmpbwvxz.html

[M04] 获取当前工作目录
来源：http://hz.kuanghao11.cn/gtogjepwta.html

Py:   os.getcwd()
来源：http://hz.zycfv.cn/gtvnlxltpu.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtteprvefm.html

JS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gteochcljq.html

TS:   process.cwd()
来源：http://hz.smart0.xyz/gtvigehcte.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gthspykmmf.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtckdkinnu.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gtmtznneti.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigufen.top/gtvkboeghx.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtclovncfj.html

Py:   sys.exit(1)
来源：http://hz.shzxlz.cn/gtaolqhfiy.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtdomaagzz.html

JS:   process.exit(1)
来源：http://hz.daria6918.cn/gtzvqohosk.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtecahzzjo.html

Java: System.exit(1)
来源：http://hz.svipenyu.cn/gthbfyxtto.html

Go:   os.Exit(1)
来源：http://hz.wangdashe.top/gtitycrbnf.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtlpxnvhji.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gtssdewjiw.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtyzgusvjn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hysaishi.cn/gteonoypsa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtmxsyfpmp.html

JS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtlvkzgiou.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtchtjzjsq.html

Java: System.err.println("err")
来源：http://hz.snrcjt.cn/gtbyubgjel.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtrwvnneoi.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtwxtimxiz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zycfv.cn/gtmvkgkplm.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtsdpcvaxn.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gthhvjgjtl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtzwrpnnnc.html

JS:   require.main === module
来源：http://hz.andypj.xyz/gtivjjzsqr.html

TS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtvsykcxdj.html

Java: public static void main(String[] args)
来源：http://hz.zhongyouzk.top/gtvuxcbjyx.html

Go:   func main()
来源：http://hz.shuidangran.top/gtxvhreaml.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtwtfgzlck.html

C#:   static void Main(string[] args)
来源：http://hz.shuidangran.top/gtfwnmgzhp.html

[M08] 获取系统与运行时信息
来源：http://hz.hfpthk.cn/gtouszqmaj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangdashe.top/gtbivmvnoq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxuanxn.top/gtbdpolusn.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gteosztbxc.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtnczrollv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.52xcode.cn/gtapwjjuym.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenlongwang.top/gtpifmnsle.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ppjwa.cn/gtxcfizhlv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxuanxn.top/gtlkeywxsm.html

================================================================================
来源：http://hz.zhijiandao.cn/gteusbnxzn.html

N. 数据结构与算法
来源：http://hz.shanyushiyangtech.top/gtjzsvungw.html

================================================================================
来源：http://hz.svipenyu.cn/gtxdepgjsx.html

[N01] 二分查找（有序数组）
来源：http://hz.hnqzz.top/gtkbunphey.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtkifjapsf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.316326.xyz/gtqwreburu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtmebkgalw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtiyvukpbk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pycfn.com/gtnbmtvsxg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtcqwejbjg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zycfv.cn/gtirmknmjt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gthfktuhlp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zdqjudy.top/gtdlawzeff.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtqekwhfxz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gtywlufsmt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtihltchgf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtbbypixdd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gteyjuefth.html

Go:   slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtuamfcvqp.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtuyouslgl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gogol.net.cn/gtvpeqseoh.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gtvjhiwcjw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gotoacloud.top/gtreklpnic.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtqgmthsvc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtfwuxsomb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtndwsplkt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ydjk.org.cn/gtnjxmlupv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.9152youxi.cn/gtkluhwzkp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnqzz.top/gtvmvajbch.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gotoacloud.top/gtyovhurec.html

[N04] 斐波那契数列
来源：http://hz.hnxiangtu.top/gtryoomnij.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtgpokmrqk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ivvv.top/gtqxihqczj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtbrtlnvag.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtbwbrhngp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtuuzvhddj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhengqikj.top/gtmshlbkzp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtuoschkch.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tianlin.xyz/gtgfgfnbkc.html

[N05] 最大公约数
来源：http://hz.zhixingplan.top/gtqxkhmagz.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gttvelvygd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtofmkvnfc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtaqbhkgno.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtnyswqkbv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangkeji.top/gtuuvxfzjv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.aizwys.cn/gtjuettjhe.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtqrccqsqz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gogol.net.cn/gtsihyqgnb.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gtdxplljje.html

Py:   s == s[::-1]
来源：http://hz.zhongyouzk.top/gtkenkvwcc.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtaodtexeh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtyhhuwjzt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtvvczcvsa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yueranfly.top/gtybghwiww.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gtimjeohae.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtrmudosyg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtqitjidwa.html

[N07] 两数之和（返回下标）
来源：http://hz.cheryme.top/gtwzfzmcgm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jianghu66.top/gtpcstpfki.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gtgrddgmnb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.havefunace.top/gtbdrkuajq.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gtyuhxrggm.html

Java: // 手写 HashMap
来源：http://hz.birdmap.top/gtavykvydj.html


<!-- 参考信息 -->