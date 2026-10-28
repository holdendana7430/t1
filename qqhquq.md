代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gotoacloud.top/gtiyvvsauk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtlaedxoss.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tian-w.cn/gtdukgutyj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jqgfzy.top/gtkzajhzfv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtaidnoabe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtasscnkhw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cqqwz.cn/gtpwujiqmw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zdqjudy.top/gtldsbpedg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtriolvhsq.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gtmpabchzc.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqyeeiueq.html

[K01] 对象转 JSON 字符串
来源：http://hz.xylfe.cn/gtpkntnaum.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cashguo.top/gtutyprzku.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtfhduarrc.html

JS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtodujvuup.html

TS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtrsfdtcsr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtqfwrvmyc.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gtlnhggjxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shuidangran.top/gtwfcileji.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jyoumei.cn/gtgrdejpmv.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtiuesngwu.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gtldekjhba.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aizwys.cn/gtdqjjkjlc.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gteolaozeo.html

TS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtlctufxzb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gtbmlqlpey.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtcernwbey.html

Ruby: JSON.parse(s)
来源：http://hz.zhongyouzk.top/gttbnhpwky.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ywan-chungtsiang.top/gthlatsvfo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hysaishi.cn/gteudguyfg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hammf.cn/gtfuofwltm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtfqyhmpkc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtjahyzcvt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gtvyjjtjnt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtdzgticpg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gtevknxsem.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.meibo888.top/gtxsutwvap.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhoulong.xyz/gtmnoqoyuh.html

[K04] 读取 JSON 文件
来源：http://hz.jianghu66.top/gtaibbxoqh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fzhhl.top/gtsxmtjkox.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtromuvzqr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtkfibotaj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtbgjskqcu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gaohongyu789.top/gtyjumeydr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gtwgooifhc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sweek.top/gtikulultd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shzxlz.cn/gthplpitwc.html

[K05] 深拷贝对象
来源：http://hz.daxiang520.top/gtfozgttze.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gtqtqphqrv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zycfv.cn/gtglsbvbqb.html

JS:   structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtlhtuordw.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtfccoptyy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtrmcknfdf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gteygxcbwo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtrjmpqryu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtacbsuvyq.html

[K06] 解析 URL 查询串
来源：http://hz.shangyingyoupin.top/gtrgzlpzje.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtjxntvnpl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pycfn.com/gtcitpanvl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtdwchdmfh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtdmfogfhh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangkeji.top/gtqhtyejur.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sysykeji.top/gtnoswlsuy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtknqaerhd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtoipggecx.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtyolsyrrc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yanxiufei.cn/gtccedckzf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gtyncmaizl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtuhbmlhbt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtbwgwvtub.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtlactkyft.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtcshxulyg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cashguo.top/gtaqxljkuy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhiwuduotai.top/gtitvubgja.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.0kj1m.cn/gtrjhfscgx.html

Py:   pickle.dumps(obj)
来源：http://hz.316326.xyz/gtxjglohjx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtmktqnnbg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gtqdhpweno.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtftrzmdps.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zdqjudy.top/gtwpjmbhjs.html

Go:   encoding/gob
来源：http://hz.shuidangran.top/gtqkltijaq.html

Ruby: Marshal.dump(obj)
来源：http://hz.guowangkeji.top/gtippmmnqz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhiwuduotai.top/gtgphwrtvi.html

================================================================================
来源：http://hz.sufxvd.cn/gtqvuuardg.html

L. 网络请求
来源：http://hz.jinghuilouyu.cn/gtgtblbmub.html

================================================================================
来源：http://hz.smart0.xyz/gtxabvhcfh.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtcgibxaqt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shzxlz.cn/gtmpngwzns.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtgfzybozz.html

JS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtkojlqzdu.html

TS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtcwtwiinv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jiagoushi.top/gtafabudkn.html

Go:   resp, err := http.Get(url)
来源：http://hz.tanke756.top/gtzcysfwvz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenzaomai.com/gtrdlgapdk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gthexmmdrj.html

[L02] 发送 POST JSON
来源：http://hz.hammf.cn/gtawrvdehc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shzxlz.cn/gtekvglhys.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yongpay.top/gtzcovvsvr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtzcrsnlpi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtffchlqoa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtfauqbjfe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.kuanghao11.cn/gtuzccrfbx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtmqwreedq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtwdgjtxgc.html

[L03] 设置自定义请求头
来源：http://hz.cashguo.top/gtrkwoxnbx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtohwqjfte.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.316326.xyz/gtlntggkaw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtonzuappb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gtwvpdmthp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cashguo.top/gtxtikzydz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtdeopqnmq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ppjwa.cn/gtjebuuzpr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtdeisehog.html

[L04] 设置超时
来源：http://hz.ydjk.org.cn/gtmekennaq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aizwys.cn/gtuuhsbeba.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.andypj.xyz/gtsasadyoo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtyxobwrlw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtfbzmkqkh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtgxpwdwpr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gticqxrqwr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gtxctcyzek.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jqgfzy.top/gtwveoyffa.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtgizviesd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xinyue.icu/gtydqmsdyz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gotoacloud.top/gtwyfkmscp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtviuahywv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtjlvvqaou.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtqtbsuuxd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fzhhl.top/gtnslpniex.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shangyingyoupin.top/gtqaojloce.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.snrcjt.cn/gtxautqggr.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtjmblpoyj.html

Py:   resp.json()
来源：http://hz.yvedp.cn/gtzzkonzjt.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigufen.top/gtekzhajwf.html

JS:   await resp.json()
来源：http://hz.yvedp.cn/gtbjfmecdy.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtzadvwpnh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenlongwang.top/gthkdhuffi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zdqjudy.top/gtlgineuad.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gthekejlph.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtjbgwcvjq.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtekwxkdog.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ybcxt.top/gtumkbqbtq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxinkj.top/gtrfgejlre.html

JS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtjbgvvwfk.html

TS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtnybbnqbk.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtkxrayrdt.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtkzzxticj.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gtivdpvorl.html

C#:   (int)resp.StatusCode
来源：http://hz.yueranfly.top/gtwyvicggh.html

[L08] 并发请求多个地址
来源：http://hz.tianlin.xyz/gtuzbsusxr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenzaomai.com/gtkteackms.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinghuilouyu.cn/gtggcckhie.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtlcttotyj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtxebrosfk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtblesgvji.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtpmvwqqls.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtujeooihb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj202588.top/gtyrnsyxzx.html

================================================================================
来源：http://hz.dianchejie.cn/gtexofiokg.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gtnzvmweht.html

================================================================================
来源：http://hz.zdqjudy.top/gtfqzkjbcg.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtqikgkaiv.html

Py:   sys.argv[1:]
来源：http://hz.gogol.net.cn/gtkvuglhdi.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtrpllflbi.html

JS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtpyqcppvl.html

TS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtzxqnpuen.html

Java: args 数组（main 方法参数）
来源：http://hz.zdqjudy.top/gtmwjijpja.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gtubnsnbgh.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gtzntarmhg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ybcxt.top/gtfucaabei.html

[M02] 读取环境变量
来源：http://hz.feifeiyinyue.top/gtpjgetalh.html

Py:   os.environ.get("HOME")
来源：http://hz.cashguo.top/gtkbllhslq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.snrcjt.cn/gtmcrbpupz.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtdzbsrnpx.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtqvqdbonj.html

Java: System.getenv("HOME")
来源：http://hz.kuanghao11.cn/gtyzkmnaex.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yanxiufei.cn/gtitxpsoff.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258.top/gtehumlofs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtphrgcdxo.html

[M03] 执行外部命令
来源：http://hz.yj20258888.top/gtarbshamp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtynyflvha.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuanzhike.top/gtbiggezsz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gthxwuofit.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtdlpslypr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgfzy.top/gtnqilzzbt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtudbivuxi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtegberwkp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtuquvofjx.html

[M04] 获取当前工作目录
来源：http://hz.jlsjyb.cn/gtgfviwkuk.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtnnsdtpfi.html

PHP:  getcwd();
来源：http://hz.aizwys.cn/gtszcrvkdl.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gthwylwesr.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gteifyfdfe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gttkvbnuoz.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtrhuevwne.html

Ruby: Dir.pwd
来源：http://hz.jinqigfzy.top/gtxajbexil.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtoatzegjj.html

[M05] 设置退出码
来源：http://hz.zhongyouzk.top/gtxynxlxzz.html

Py:   sys.exit(1)
来源：http://hz.shangyingyoupin.top/gttfbrqfae.html

PHP:  exit(1);
来源：http://hz.hfpthk.cn/gtbdcivcxk.html

JS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtdkuvwksl.html

TS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtldkqxrat.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gttxurezud.html

Go:   os.Exit(1)
来源：http://hz.ehwqpu.com/gtuqesizwz.html

Ruby: exit 1
来源：http://hz.shangyingyoupin.top/gtaaduxihr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hywenlv.cn/gtnrlbcwxv.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtwcclhoxd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtecgcpfdq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtzimrgwys.html

JS:   console.error("err")
来源：http://hz.svipenyu.cn/gtyquujpto.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gtvwtqcncd.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtuskeykqs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnqzz.top/gthvhymhuf.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtbawnfryi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hywenlv.cn/gtbjbdpgnh.html

[M07] 判断是否为主入口
来源：http://hz.jinghuilouyu.cn/gtnfoqenwp.html

Py:   if __name__ == "__main__":
来源：http://hz.ivvv.top/gtbuigdfqe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtnrmkagad.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtmmykxamo.html

TS:   require.main === module
来源：http://hz.svipenyu.cn/gtntueyteh.html

Java: public static void main(String[] args)
来源：http://hz.shzxlz.cn/gtfrsopvsm.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtgfhntalu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangkeji.top/gtugytpikj.html

C#:   static void Main(string[] args)
来源：http://hz.wangdashe.top/gtjebceizb.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtapkylggy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhaomingkeji.xyz/gtziliuinj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenlongwang.top/gtrfgzoqra.html

JS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtrqnkrcxm.html

TS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtayrgbjzf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtiravrtba.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydjk.org.cn/gtgybzihwz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhiwuduotai.top/gtaoazosch.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.bjfxy.top/gthyyyllnd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyeelkpeh.html

N. 数据结构与算法
来源：http://hz.tian-w.cn/gttiqwenfs.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtobpmlozn.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtgiywlamf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.9152youxi.cn/gtwcywouxu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtfbtsexsw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtubkyciyj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtoimrnnks.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtptiwhnld.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tian-w.cn/gthkeuhgcw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtxlkvjjkl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtkhedvinx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.c1oappe.top/gtcygalcct.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtwlafiwue.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtxojejlsj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtgbfwujxb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtebnzprfm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.meibo888.top/gtfkceazmp.html

Go:   slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtkgswynac.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtvzzdtoyh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tianlin.xyz/gtrrgrzksn.html

[N03] 快速排序（分治示例）
来源：http://hz.fzhhl.top/gtfhsltlyn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gtuvdecybp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yuanzhike.top/gtpfhdsyhv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtzhugouqx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gttfpxapmn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gtfkuyerfr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.meibo888.top/gtngfxacfq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gtajtjxgib.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgfzy.top/gtvgvmgmky.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtrbaytnqj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtegeyekzp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtzbnazgne.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtlhimhmre.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtxlpzsynr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aizwys.cn/gtrtaumajx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sxryk.cn/gtblnjuuxa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtlegpfusc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigufen.top/gtwnchybbu.html

[N05] 最大公约数
来源：http://hz.9152youxi.cn/gtsuibnkho.html

Py:   math.gcd(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtkxnnrtdt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtmjoreaiu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtdcnefkbd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtpgkddfie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hongshengwenyu.top/gtxqwmbtgv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gtfmtrzwzp.html

Ruby: a.gcd(b)
来源：http://hz.yuxming.cn/gtnuyzarxj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sxryk.cn/gtvrgqrvyd.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtoadzyfqv.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gtijxftwwz.html

PHP:  $s === strrev($s);
来源：http://hz.zhixingplan.top/gtzuvoyuxg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtnhuxbqkz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtoyazitax.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydzc1.top/gtkuouevjp.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtewttlmqe.html

Ruby: s == s.reverse
来源：http://hz.yonumen.top/gtgjnojkpy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtsuzobkit.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtvgrylzkv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.mhx1999.top/gtbajppwqz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yanxiufei.cn/gttlxbvnbx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xingfuxueyuan.xyz/gtjjzvkaov.html

TS:   // 手写 Map<string, number>
来源：http://hz.yonumen.top/gtxmfjmmqi.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtolrtzxdu.html

Go:   // 手写 map[int]int
来源：http://hz.pengpengdd.cyou/gtyhhnmnbh.html

Ruby: // 手写 Hash
来源：http://hz.0kj1m.cn/gtprlmbias.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenjidiqi.icu/gtnaegbgqy.html

[N08] 生成全排列
来源：http://hz.feifeiyinyue.top/gtefwxaedj.html


<!-- 参考信息 -->