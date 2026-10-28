代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jlsjyb.cn/gthagsxjds.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shzxlz.cn/gtgepvyquq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhengqikj.top/gtwffwrxgc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinyuanbaomall.cn/gtbwnjqoqp.html

================================================================================
来源：http://hz.yj20258.top/gtxrftiggl.html

K. JSON 与序列化
来源：http://hz.sysykeji.top/gtevilfmrb.html

================================================================================
来源：http://hz.sysykeji.top/gtmhncmdut.html

[K01] 对象转 JSON 字符串
来源：http://hz.jyoumei.cn/gtrnkixfyu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtacwrdeib.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtpnufmksq.html

JS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtqhzqfojq.html

TS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gttbyojnje.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangshuangyany.cn/gtvnexyibl.html

Go:   json.Marshal(obj)
来源：http://hz.snrcjt.cn/gtuzrjfdir.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhoulong.xyz/gtjegbmakw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgufenzy.top/gtqunlquss.html

[K02] JSON 字符串转对象
来源：http://hz.hfpthk.cn/gtppqutjto.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtbrgfoeam.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtzbrcfhtt.html

JS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtcbduvbew.html

TS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gtaokysvjt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgufenzy.top/gtbxjkpdyl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtbhmmnjbk.html

Ruby: JSON.parse(s)
来源：http://hz.daxiang520.top/gtvjilfump.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gthahmybyw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtiktqxwsx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtehcmzkym.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtrkhsrjwo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtelctulgz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtdtketkrm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuetiantiany.cn/gtypjvozxg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.bjfxy.top/gtjheldsbl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhiwuduotai.top/gtqtkxgbwd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ppjwa.cn/gtwhtpfdeq.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtzviubcyr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gtrfootwui.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yvedp.cn/gtpgcagafs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtajbgslae.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtzhhovrne.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.smart0.xyz/gtwvdouupk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtwohqhcjm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pycfn.com/gtyxfjednj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtfjtfhpud.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtzyhgpfkp.html

Py:   copy.deepcopy(obj)
来源：http://hz.gogol.net.cn/gtplpxanii.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gthbdzoibu.html

JS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtmpqwzipm.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtpzziedkc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuxming.cn/gtmlbhvgjy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhixingplan.top/gtusufpesc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtvnwvqfjd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xinyue.icu/gtyzdqyivz.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtfzdzuhek.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yanxiufei.cn/gtajcbcdrx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.birdmap.top/gtopsrzgre.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtuvltpvgl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtzcrwdbbk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuanzx.com/gtwkiyyewe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtpfvgkesi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtxikyqnck.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hammf.cn/gtriocodhr.html

[K07] 进制转换
来源：http://hz.hammf.cn/gtbgzuocmq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ivvv.top/gtovpoirmq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pengpengdd.cyou/gtjwrtfywe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtzpnhulhu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtluwvpjsf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtxgqznyzt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cashguo.top/gtkmatuguz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.haohaochexian.top/gteoetycih.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.0kj1m.cn/gtjveifcnt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hongshengwenyu.top/gtknjpkaef.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtmdbdnose.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guowangkeji.top/gtesecrnvt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtzouiqexd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtfmchryzw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gtlfrwtxqz.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtoxgexdmi.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtbjjqjzil.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtwdjrjfen.html

================================================================================
来源：http://hz.bjfxy.top/gtebldljbx.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gteeuobigx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtoudvesbl.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtyakfqblh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhixingplan.top/gtrffooqyu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtwzjcspyt.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtycvnjrad.html

TS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtcbmdvyhs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ppjwa.cn/gtbbuiofen.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtecjrtisg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.redwolf501.top/gtlsyeolyf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenzaomai.com/gtdzujbtpc.html

[L02] 发送 POST JSON
来源：http://hz.hysaishi.cn/gtfaqvpkko.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhijiandao.cn/gtdhfjtgku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daxiang520.top/gtkegurbaf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtalbekyoo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gtkxohcwrk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtxaedhtiq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fengsongda.top/gtuvllhbew.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gthwogjkzn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtxvcdtovy.html

[L03] 设置自定义请求头
来源：http://hz.zhengqikj.top/gthjhvfooq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gtqidiwmzr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtcovyozuy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtijlrljka.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtwsqnxnqo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuanzx.com/gtkgwnkkdb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenlongwang.top/gtajnnrcbt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tianlin.xyz/gtqdjcchce.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yongpay.top/gttqpnlxxh.html

[L04] 设置超时
来源：http://hz.snrcjt.cn/gtzakalfws.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtflczbyrm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.birdmap.top/gtpgnkytvn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gttbknfpvy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jianghu66.top/gtdgyatvxd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.svipenyu.cn/gtkqzrhgxm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yvedp.cn/gttsxjemda.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtletjihds.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jyoumei.cn/gtilywehfy.html

[L05] 上传文件（multipart）
来源：http://hz.chenjidiqi.icu/gtbzmzwpng.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daria6918.cn/gtsroevnzj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuxming.cn/gtlovifykj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtqaalcqrv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gthgbrimcy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtswgzpybn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gtrbesovei.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yueranfly.top/gtirevrvsb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.birdmap.top/gtuwwhwblg.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtwakotera.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtdjbxgbnf.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtqeteteoq.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtxjglgooi.html

TS:   await resp.json()
来源：http://hz.ybcxt.top/gtsnxhpszm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tianlin.xyz/gtsxnsjxqn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.andypj.xyz/gtyttfkvmb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yvedp.cn/gtocwfmlub.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sxryk.cn/gteravkahc.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtlccthakq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daria6918.cn/gtaijkzpmo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fzhhl.top/gtdmndngfs.html

JS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gthjtfxwzk.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtfncfmitx.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtwxurywlb.html

Go:   resp.StatusCode
来源：http://hz.hongshengwenyu.top/gteaacicvd.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtxchdnapy.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gthjrcbgrd.html

[L08] 并发请求多个地址
来源：http://hz.zycfv.cn/gtyklfdcud.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sufxvd.cn/gtlexqfivu.html

PHP:  curl_multi_init() 系列
来源：http://hz.cashguo.top/gtaeynqavw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtawvyddnm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtgarqyqjg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xingfuxueyuan.xyz/gthikcqjfv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cdnleiting.top/gtnoaprhdg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtnnrqkpdp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.andypj.xyz/gtegszlawi.html

================================================================================
来源：http://hz.gogol.net.cn/gtpfnywvft.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gttohfwdgf.html

================================================================================
来源：http://hz.xuanzx.com/gtyjgvfyca.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtfejflsbq.html

Py:   sys.argv[1:]
来源：http://hz.jianghu66.top/gtmhignvkk.html

PHP:  $argv;  $argc;
来源：http://hz.fzhhl.top/gthzwdmaks.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtstryryhb.html

TS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gthiympego.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxinkj.top/gtqmvcgtrt.html

Go:   os.Args[1:]
来源：http://hz.shangyingyoupin.top/gtgjqgmxux.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gtdibbnhfc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtzgawdvfc.html

[M02] 读取环境变量
来源：http://hz.svipenyu.cn/gtfhuiwfyt.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtaxnrhucg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zycfv.cn/gtpzqzujlv.html

JS:   process.env.HOME
来源：http://hz.daxiang520.top/gtpcaoakpv.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtqqmyzmgc.html

Java: System.getenv("HOME")
来源：http://hz.cashguo.top/gtytnxivqb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangdashe.top/gtnxnedbgv.html

Ruby: ENV["HOME"]
来源：http://hz.fengsongda.top/gttsxxbbqk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yangfankeji.com/gtlprzfuub.html

[M03] 执行外部命令
来源：http://hz.jlsjyb.cn/gtdmehbtry.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.svipenyu.cn/gtucxrvcoo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtztpqgrwz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtbavbpcge.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtfcejwxei.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fzhhl.top/gtbhptrwwe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sxryk.cn/gtugsdmkyl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtspdddymz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.redwolf501.top/gtozpypjhz.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gtvjhksiai.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gtpxtdixdp.html

PHP:  getcwd();
来源：http://hz.ivvv.top/gtvwtywajk.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtkpdxvvyj.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtobvbeehx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gthhrwooaw.html

Go:   os.Getwd()
来源：http://hz.xziqi.cn/gtyxfawmew.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gthcmtvyyg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxuanxn.top/gtvjvimkyk.html

[M05] 设置退出码
来源：http://hz.gaohongyu789.top/gtdugreelc.html

Py:   sys.exit(1)
来源：http://hz.yvedp.cn/gtfqngybzb.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtfcoxvcqk.html

JS:   process.exit(1)
来源：http://hz.yvedp.cn/gtsrylpstb.html

TS:   process.exit(1)
来源：http://hz.birdmap.top/gtpqvcpjux.html

Java: System.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtoxatcvng.html

Go:   os.Exit(1)
来源：http://hz.gzhubu.top/gtcrcdqsob.html

Ruby: exit 1
来源：http://hz.tanke756.top/gtzbklorld.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zycfv.cn/gteysnbxuy.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtqcunccbf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dianchejie.cn/gttulgqhza.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtkaszxijp.html

JS:   console.error("err")
来源：http://hz.mhx1999.top/gtziskzhdk.html

TS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtlexapgmj.html

Java: System.err.println("err")
来源：http://hz.fengsongda.top/gtuevpztse.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxuanxn.top/gtcgcppgrd.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gtbbjcvucx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gtuirkcgpt.html

[M07] 判断是否为主入口
来源：http://hz.gogol.net.cn/gthpzcouoa.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtncnbvgqd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gthjpwlwnk.html

JS:   require.main === module
来源：http://hz.aizwys.cn/gtjbkozcrz.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtiifdgeta.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gttiklnlbc.html

Go:   func main()
来源：http://hz.ppjwa.cn/gtxobixrcq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tianlin.xyz/gtlrihugdm.html

C#:   static void Main(string[] args)
来源：http://hz.jinghuilouyu.cn/gtgsounxss.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gthrfdjwwz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtqmpnjsrp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ehwqpu.com/gtzouxffxz.html

JS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtslpdzyfq.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtxkzusmok.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gtwunzwcxc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gtfwqsyydw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jlsjyb.cn/gtwdhxjlwi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hfpthk.cn/gtvmsudwfi.html

================================================================================
来源：http://hz.xziqi.cn/gtocspazqx.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtxslsfvgy.html

================================================================================
来源：http://hz.hammf.cn/gttcdhzvrp.html

[N01] 二分查找（有序数组）
来源：http://hz.jianghu66.top/gtpljdkent.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangshuangyany.cn/gtmkvywxxz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.birdmap.top/gtktenlvrd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtsulpdyme.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtswtryqtq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pycfn.com/gtukzzlgqh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtdlyhpmls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gtutcjzygd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtgppbwnvw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yvedp.cn/gtszgtyboj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nwbrower.top/gtzpeovauy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtuwxschio.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtzcdiizyp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xylfe.cn/gtyaiyccvn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zdqjudy.top/gtcljouivg.html

Go:   slices.Sort(arr)
来源：http://hz.andypj.xyz/gtaqahzjnq.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gthjxiflom.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gtvjfpkbyu.html

[N03] 快速排序（分治示例）
来源：http://hz.316326.xyz/gtprxeepgz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtladvmqhc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangtech.top/gtnuwdjghf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtyfdmyvxp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtxohgwojn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hfpthk.cn/gtmrvmbqhk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pycfn.com/gtrmejexas.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yueranfly.top/gtikbjzbik.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pycfn.com/gtmbznwdiq.html

[N04] 斐波那契数列
来源：http://hz.xinyue.icu/gtbpxcqyaf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtjkieytpc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtcmobsezu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtoqxmeivf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtmlnlhzrm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.snrcjt.cn/gtgisranna.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydjk.org.cn/gtlrwoaoqs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtafhzrwze.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yangfankeji.com/gtopcyftpf.html

[N05] 最大公约数
来源：http://hz.sweek.top/gtmenlemxa.html

Py:   math.gcd(a, b)
来源：http://hz.ybcxt.top/gtdxjcysxu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gtzcyyxkmu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtqvnygxwc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtzdakstcx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangtech.top/gtghakbqpy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gzhubu.top/gtmexfnxij.html

Ruby: a.gcd(b)
来源：http://hz.iojbl.cn/gtebgjqfeq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhongyouzk.top/gtjvfqryhz.html

[N06] 判断回文字符串
来源：http://hz.zhengqikj.top/gthvnueupk.html

Py:   s == s[::-1]
来源：http://hz.yvedp.cn/gtgscjnvvo.html

PHP:  $s === strrev($s);
来源：http://hz.meibo888.top/gtaiqexndl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtnnuuzino.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtpdzmyfjo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yuxming.cn/gtzcegddmz.html

Go:   // 双指针从两端比较
来源：http://hz.tian-w.cn/gtdzynajws.html

Ruby: s == s.reverse
来源：http://hz.cqqwz.cn/gtwihyrumx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtdoayejvu.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtocuaxkgg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxuanxn.top/gthzdtuffe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xziqi.cn/gtmnnxfojm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.9152youxi.cn/gtktwfxmlv.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gtkvjglbnm.html

Java: // 手写 HashMap
来源：http://hz.vqdsnc.cn/gtdtiidzax.html

Go:   // 手写 map[int]int
来源：http://hz.nwbrower.top/gtgpbfpruh.html

Ruby: // 手写 Hash
来源：http://hz.hfpthk.cn/gtrkdljixl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cqqwz.cn/gtfbfrstwk.html

[N08] 生成全排列
来源：http://hz.cqqwz.cn/gtlbmmuglj.html

Py:   itertools.permutations(arr)
来源：http://hz.ybcxt.top/gtbgyvauau.html

PHP:  // 手写递归交换
来源：http://hz.yvedp.cn/gtmsnxpzlc.html

JS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtprzlobnz.html

TS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtozfgfqry.html


<!-- 参考信息 -->