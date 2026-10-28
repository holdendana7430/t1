代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtnbtirpra.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtlnswtwag.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtwfixzeud.html

TS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtijmksufq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtyrdopcze.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gttttkrbfu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnxiangtu.top/gtpqjbkmhm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yanxiufei.cn/gtvtumozdi.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gtassselio.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtuvmxcmcm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sufxvd.cn/gtcooujtld.html

JS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtzjgrnexo.html

TS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtfehgtwum.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtfdwmzngy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtvrxlgybp.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtburlpfyt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangshuangyany.cn/gtkuoupyra.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jianghu66.top/gtpqhdpyow.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.316326.xyz/gtxbaunmhy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtwcdamvms.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtarlqdabf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtuqxlkcjb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinghuilouyu.cn/gtjsxmvvgh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sysykeji.top/gtvtibrnjm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hongshengwenyu.top/gtyxzujbff.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtlhohnkop.html

[K04] 读取 JSON 文件
来源：http://hz.cqqwz.cn/gtpvloatov.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ehwqpu.com/gttnyjfdtq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gttytbwuzu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtjwxkmxpw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtbsjrsvce.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtdjokuqpm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtrlfochhx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.iojbl.cn/gtboathhbr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtvwoilgvi.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtihtvabac.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gtkakbsnrj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuanzx.com/gtfingzbhm.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtpomijkxc.html

TS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtetdnbpyn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yanxiufei.cn/gtndzagpnw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cqqwz.cn/gtntjhdqtw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhongyouzk.top/gtiivnmabh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj202588.top/gtswioscfp.html

[K06] 解析 URL 查询串
来源：http://hz.cqqwz.cn/gtcaagnbxi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yongpay.top/gtpjmzglwd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ywan-chungtsiang.top/gthdonqcri.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtmrochdjb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtzwokhbbd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xylfe.cn/gtvmxbdrbs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fengsongda.top/gtjppildmf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtgtnfpqec.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gzhubu.top/gtemmslluo.html

[K07] 进制转换
来源：http://hz.haohaochexian.top/gtpjaxqaxq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtyywpprwh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuanzx.com/gttcchxzyy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtmrxwvqon.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtkcrulkoi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtobyjotcm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ybcxt.top/gtxaljjcby.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtxcckvdyo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxinkj.top/gtzdhdzfap.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gtjxmlpwgg.html

Py:   pickle.dumps(obj)
来源：http://hz.feifeiyinyue.top/gtiunofhxh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.aizwys.cn/gtnzenopbv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtlpuklyeb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtsqvegwmx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guowangkeji.top/gtepdqurem.html

Go:   encoding/gob
来源：http://hz.xingfuxueyuan.xyz/gtpyntnfid.html

Ruby: Marshal.dump(obj)
来源：http://hz.shuidangran.top/gtmuquvzva.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zycfv.cn/gtyigfhjef.html

================================================================================
来源：http://hz.cdnleiting.top/gtjaxcvigl.html

L. 网络请求
来源：http://hz.svipenyu.cn/gtcceopiao.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgpmbwqyg.html

[L01] 发送 GET 请求
来源：http://hz.aizwys.cn/gtiecnyton.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxinkj.top/gtbaxkvuwr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dianchejie.cn/gtqscwngoi.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtrrwaaqhp.html

TS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtyvivrckv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hywenlv.cn/gtkjukdxmc.html

Go:   resp, err := http.Get(url)
来源：http://hz.52xcode.cn/gtybebxadm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.redwolf501.top/gtrfwtffmu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtqvdukfey.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtohcaiywd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtotaaijwu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yonumen.top/gtuyccncuy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtoogxzdio.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtmyjwzitb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtjehtnedh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtgpobhdcd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.andypj.xyz/gtilmtncmq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gttczjwrwy.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtopxwtjup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtlestotoz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daria6918.cn/gttrunkpni.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtwqmuqwvj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtetulyols.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.9152youxi.cn/gtvjzwcput.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtzhwmgimp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gotoacloud.top/gtfurnxbqc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtgotfromq.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtvlvtjgro.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yanxiufei.cn/gtshwmmnix.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nwbrower.top/gtbngbxyql.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtyktenvvd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtinuuzpzg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yonumen.top/gtlqepffrz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cashguo.top/gttmqjtpiq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hongshengwenyu.top/gtssjltopk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jiagoushi.top/gtndxgklhr.html

[L05] 上传文件（multipart）
来源：http://hz.gzhubu.top/gtuicrzzvp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cheryme.top/gtyoblyvby.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shangyingyoupin.top/gtzfzflunc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtbyruouae.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtwruojlnb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gzhubu.top/gtrimesxol.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cucudq.cn/gtscxhebgu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gzhubu.top/gtjdiovwds.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgufenzy.top/gtyhctombh.html

[L06] 解析响应为 JSON
来源：http://hz.ivvv.top/gtmievvtvl.html

Py:   resp.json()
来源：http://hz.316326.xyz/gtgvftztuv.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gtdozolpqf.html

JS:   await resp.json()
来源：http://hz.havefunace.top/gtcasgjody.html

TS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtykphnemv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yongpay.top/gtailkblib.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tianlin.xyz/gtzluhlapn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zycfv.cn/gtispfendv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gaohongyu789.top/gtwzoxjpgt.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtmaqnmqbx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gtovqxiqig.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxuanxn.top/gtanqliifu.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtyqnuqugw.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtapugxzgb.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtygktohyl.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gtrurcejvf.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtciqrcrpo.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtfaqdymow.html

[L08] 并发请求多个地址
来源：http://hz.svipenyu.cn/gtaoknbiny.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.birdmap.top/gtrtmehgjp.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuanzx.com/gtkpfqnygs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtsrxsydsv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtbebxvwei.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tian-w.cn/gtuhmqduvk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sweek.top/gtvjwvywbg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtzqajgvzg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtvrjwjzuq.html

================================================================================
来源：http://hz.yj20258.top/gtdnwvdomz.html

M. 命令行 / 进程 / 环境
来源：http://hz.cheryme.top/gtmdklccvi.html

================================================================================
来源：http://hz.cqqwz.cn/gtyvweazil.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gtgozwgpgd.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtkmybrfbr.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtiatjxlgu.html

JS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gthlgjhuaq.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtuoxtpwlp.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtdaztzgsr.html

Go:   os.Args[1:]
来源：http://hz.jqgfzy.top/gtkqpzdeff.html

Ruby: ARGV
来源：http://hz.hysaishi.cn/gtjtfpsrqc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtebnernud.html

[M02] 读取环境变量
来源：http://hz.zdqjudy.top/gtyipzpocs.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gtrjnsjnan.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtyaoraojq.html

JS:   process.env.HOME
来源：http://hz.daria6918.cn/gtxcxtxlls.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtcduvgtty.html

Java: System.getenv("HOME")
来源：http://hz.nanxinkj.top/gtmvrxlhwm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigfzy.top/gtmiedjsoz.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gtehqespgz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtbynqlcwa.html

[M03] 执行外部命令
来源：http://hz.aibaodan.cn/gtsztcgboq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.bjfxy.top/gtpcunfwey.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtqslscfwk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtpkxqpozr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtaguepfao.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.andypj.xyz/gtreqyxwzo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtvqkvuyiz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtcdnhoiuh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gtjnqzrbiu.html

[M04] 获取当前工作目录
来源：http://hz.pycfn.com/gtlxlwirtt.html

Py:   os.getcwd()
来源：http://hz.sweek.top/gtkzjeoeli.html

PHP:  getcwd();
来源：http://hz.zhixingplan.top/gtjbfmhcmb.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gtikydmynl.html

TS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtuasllfni.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guowangkeji.top/gtjoqmfopo.html

Go:   os.Getwd()
来源：http://hz.yj202588.top/gthihwkloo.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gtjvepxdmz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.svipenyu.cn/gtdxajgvdg.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtdbrcovzs.html

Py:   sys.exit(1)
来源：http://hz.daxiang520.top/gtntswfgji.html

PHP:  exit(1);
来源：http://hz.sysykeji.top/gtcrihqjir.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gtsdxrxxzm.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtsuujspil.html

Java: System.exit(1)
来源：http://hz.nanxinkj.top/gtggeygtxn.html

Go:   os.Exit(1)
来源：http://hz.sweek.top/gtjsvfbxza.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gthixvjnmx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.vqdsnc.cn/gtyypkyfwy.html

[M06] 向标准错误输出
来源：http://hz.jinqigfzy.top/gtrrcsseia.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtgzoydlhg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gtbyrofcuh.html

JS:   console.error("err")
来源：http://hz.xuanzx.com/gtnrkenpez.html

TS:   console.error("err")
来源：http://hz.jinqigufen.top/gtyfxvlocy.html

Java: System.err.println("err")
来源：http://hz.guannengcc.top/gtktzfdryr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hywenlv.cn/gtztznwcda.html

Ruby: warn "err"
来源：http://hz.cheryme.top/gtwrlvfbtu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhongyouzk.top/gtxgibeuan.html

[M07] 判断是否为主入口
来源：http://hz.ybcxt.top/gtkzpvseou.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtjoghrydr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yueranfly.top/gtxjgzsjot.html

JS:   require.main === module
来源：http://hz.cheryme.top/gtkivvtgrm.html

TS:   require.main === module
来源：http://hz.tianlin.xyz/gtojrvtdxz.html

Java: public static void main(String[] args)
来源：http://hz.zhiwuduotai.top/gtskizratu.html

Go:   func main()
来源：http://hz.chenzaomai.com/gtrlwfxwse.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtcumwivml.html

C#:   static void Main(string[] args)
来源：http://hz.hfpthk.cn/gtjmdsdoaf.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gtekxwzhxj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.316326.xyz/gtjppgmkal.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cdnleiting.top/gtggdjbqwd.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtiwcdqkdx.html

TS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtwrcyezki.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gtombtamad.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtlshxocxy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hysaishi.cn/gtoxhtxqwy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhixingplan.top/gthkxfvint.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtcocuhgjr.html

N. 数据结构与算法
来源：http://hz.shuidangran.top/gttnuielow.html

================================================================================
来源：http://hz.316326.xyz/gtwiinylxd.html

[N01] 二分查找（有序数组）
来源：http://hz.cqqwz.cn/gtidzuvfmn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hongshengwenyu.top/gttaqhhxyn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gthbvcedkz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gteyyaaqsm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtflmhjkxy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtxcmwpdag.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jlsjyb.cn/gtzqqedrzq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cucudq.cn/gtcryuznbw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gteudqisvs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gtdbjnuqls.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtvjvqhklb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gtzxdiqibz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtqqnvtxek.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtaqxocrkt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gtammwhjff.html

Go:   slices.Sort(arr)
来源：http://hz.daria6918.cn/gtqmnfsoxf.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtdnbxqmuz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhoulong.xyz/gtlasxfjwn.html

[N03] 快速排序（分治示例）
来源：http://hz.yj202588.top/gtmiioshgl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtpmcjkvxd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtxkpjtaog.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtkmevklej.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtvrpestnx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gtiftcjhlz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.c1oappe.top/gtnumebedf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtabasjvwn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tian-w.cn/gtqmvqzyas.html

[N04] 斐波那契数列
来源：http://hz.zhoulong.xyz/gtykpuutiy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtmajzvsqz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenzaomai.com/gtnqiqqajl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.mhx1999.top/gtzwuswwjk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtdirqtxhu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtntghbyxe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xinyue.icu/gtxxafdgdy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtyhanlfmv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jqgufenzy.top/gtmureymsj.html

[N05] 最大公约数
来源：http://hz.haohaochexian.top/gttrqpsxcq.html

Py:   math.gcd(a, b)
来源：http://hz.kuanghao11.cn/gthgssdqvu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtogesburd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtuficbily.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtfyarhgtc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuetiantiany.cn/gtxbhtupwu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhixingplan.top/gtqtckaklk.html

Ruby: a.gcd(b)
来源：http://hz.yj20258.top/gtahrfuwwn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgufenzy.top/gtjsgeynrl.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtpgkrxsmz.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtjnwrbmgk.html

PHP:  $s === strrev($s);
来源：http://hz.feifeiyinyue.top/gtwbqtucnx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtmaflfhlg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtyaaerghl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gtbrulltsp.html

Go:   // 双指针从两端比较
来源：http://hz.jqgfzy.top/gtbdbpbasm.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtyidbrits.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtapdhaugk.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtnggdnpsw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yanxiufei.cn/gtwwhiszgv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhixingplan.top/gtdaoyaqfq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xinyue.icu/gtylsufeud.html

TS:   // 手写 Map<string, number>
来源：http://hz.quarkkingdee.top/gtuwcyxnnn.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtnidxeisv.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gtaxzcnoyb.html

Ruby: // 手写 Hash
来源：http://hz.wangshuangyany.cn/gtcwtclkuv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.snrcjt.cn/gtqbgxwywg.html

[N08] 生成全排列
来源：http://hz.gotoacloud.top/gtnenaywkv.html

Py:   itertools.permutations(arr)
来源：http://hz.shuidangran.top/gtnpzwegla.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtlbpahkbe.html

JS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtezvtomxr.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtjtfvxcjx.html

Java: // 手写回溯递归
来源：http://hz.yongpay.top/gtlqkrwonu.html

Go:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtbyypzyre.html

Ruby: arr.permutation.to_a
来源：http://hz.yongpay.top/gtlhdumbcb.html

C#:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtmvyzmwwl.html

[N09] 栈与队列
来源：http://hz.tanke756.top/gthaymudii.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhixingplan.top/gttzhlybjj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.meibo888.top/gtvsdbqtoy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aibaodan.cn/gtjfizjspk.html


<!-- 参考信息 -->