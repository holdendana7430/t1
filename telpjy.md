代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gttoofkadl.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gthrlwrnos.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tianlin.xyz/gthdehsapg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xziqi.cn/gtxddqeuyx.html

[K02] JSON 字符串转对象
来源：http://hz.dashuyun.cn/gtvcxqgowh.html

Py:   json.loads(s)
来源：http://hz.cqqwz.cn/gttaftjsrl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.316326.xyz/gtvnphqvry.html

JS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtsligiuof.html

TS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtyzihmixg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtjvyucthi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtrjvaoquv.html

Ruby: JSON.parse(s)
来源：http://hz.xylfe.cn/gtwdswmgng.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtkirimzeu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sufxvd.cn/gtihniirat.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.316326.xyz/gtelskpabz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtbdvcviuy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtbqbgsjnj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtwfdrjwpz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cdnleiting.top/gtbbsvparc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtqkfjzlex.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuxming.cn/gtgantmyfh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenzaomai.com/gtjoughnjg.html

[K04] 读取 JSON 文件
来源：http://hz.shzxlz.cn/gtevhvggwq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtfohkgixi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtrcxsdcrj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtlgnfjyzx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtusxaxifo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuxming.cn/gtrcoeaeyq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gteqyksowe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtcnphjmwj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258888.top/gtmkcuvsnc.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gttymbibth.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtqzctlndg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigufen.top/gtvxqqqebv.html

JS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtugjanywv.html

TS:   structuredClone(obj)
来源：http://hz.yonumen.top/gthtqrarwf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtaqnqpozf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gtenhyxxhj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigfzy.top/gtkjbxxrdo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shangyingyoupin.top/gthoerrguj.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtstafudjj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenlongwang.top/gtxcrftuxm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangdashe.top/gtflmcneht.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtudwcnjrw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtgmrpfnbc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtpjcmzgdr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtetvhjnlu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtuqvsembm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhengqikj.top/gtmglqugsa.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtvlqklcaf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtaaawewid.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aizwys.cn/gtfbaetics.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtpuafiwja.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gttcizudtq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gthwuxhvcf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydjk.org.cn/gtoiblsipl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtkzaitgme.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtxjsvwcln.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tian-w.cn/gtwtfprwub.html

Py:   pickle.dumps(obj)
来源：http://hz.gotoacloud.top/gtpdpakncs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtenwnwhrm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtzfeuwezh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtrdpaftaz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.havefunace.top/gtshwatomd.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtrekohtgm.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydjk.org.cn/gtlqqvwtbf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtopetygom.html

================================================================================
来源：http://hz.bjfxy.top/gtogijixjh.html

L. 网络请求
来源：http://hz.ppjwa.cn/gtjzmdeymu.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqwtopwdm.html

[L01] 发送 GET 请求
来源：http://hz.ivvv.top/gtetesadvk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cashguo.top/gtyzexvbfc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gteapmlusi.html

JS:   await fetch(url)
来源：http://hz.jianghu66.top/gtbobwjvok.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtvvnkcbke.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.redwolf501.top/gthcoavxec.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gteyrmdowj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zycfv.cn/gttmvmqdya.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtelnjgnnc.html

[L02] 发送 POST JSON
来源：http://hz.ydjk.org.cn/gtnkdxumkn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.c1oappe.top/gtnviobjgf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtkcpadgsz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtmzxvuxgi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xziqi.cn/gtdvgrsgnx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgfzy.top/gtlkeqhsvk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtgpcjvpiv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhixingplan.top/gtiydsllba.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pengpengdd.cyou/gtjfgpzydu.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtjpxdppdv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtzlvfaoff.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aibaodan.cn/gtzmcuhbvd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtsssghbcv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtvconjfax.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtbldgnbwf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtmykilwmv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigfzy.top/gtbxvgnvkm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtommpguac.html

[L04] 设置超时
来源：http://hz.shzxlz.cn/gtdkwvzick.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtcgkihfia.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtmnzdqopv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtlkttllts.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtiffgjtzg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hywenlv.cn/gtwjaqrbzp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gtbpghvmnh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gtxvesprxf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shangyingyoupin.top/gtlhzhstkd.html

[L05] 上传文件（multipart）
来源：http://hz.ydjk.org.cn/gtpnhwyijb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtzdmbbxsg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shangyingyoupin.top/gtzqzbcnpw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtnpkilmmy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtjehniwfk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtafejuumz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtlebioyty.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtlqhiprvx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhixingplan.top/gtuhvenwux.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtravhawgc.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtvzsoqnlu.html

PHP:  json_decode($body, true);
来源：http://hz.xuetiantiany.cn/gtyjxjozuh.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gtplkqpnln.html

TS:   await resp.json()
来源：http://hz.yvedp.cn/gtqyiozkba.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtkqvvmmhz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.vqdsnc.cn/gtjtkafdig.html

Ruby: JSON.parse(resp.body)
来源：http://hz.birdmap.top/gtrptsmcse.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhijiandao.cn/gtguvluxsh.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtrnqkovzw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtwieiwfac.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtmemtwxij.html

JS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtshppspwp.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtdsbugwex.html

Java: resp.statusCode()
来源：http://hz.9152youxi.cn/gtlkloagrf.html

Go:   resp.StatusCode
来源：http://hz.jinqigufen.top/gtxhfpglys.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtraqmijyd.html

C#:   (int)resp.StatusCode
来源：http://hz.jiagoushi.top/gttlebvraw.html

[L08] 并发请求多个地址
来源：http://hz.9152youxi.cn/gtbwabvaqg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgufenzy.top/gtfqoosfus.html

PHP:  curl_multi_init() 系列
来源：http://hz.jyoumei.cn/gteffhmllz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtztkozyaj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtknrozpyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gaohongyu789.top/gtqczurpah.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgufenzy.top/gtsvamizjv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hongshengwenyu.top/gtphuaoxao.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhaomingkeji.xyz/gtvjkvnfdg.html

================================================================================
来源：http://hz.tian-w.cn/gtbsfevfjd.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj202588.top/gtnfyjstml.html

================================================================================
来源：http://hz.gogol.net.cn/gthxlnuqiq.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtlqdlkefg.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gtepwnzkuv.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gtntaqzsug.html

JS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gthxblbvqy.html

TS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtyvbauphu.html

Java: args 数组（main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtvgvoilrj.html

Go:   os.Args[1:]
来源：http://hz.yvedp.cn/gtrzhgkigd.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtaxugwcmk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtpfvvhkug.html

[M02] 读取环境变量
来源：http://hz.zhengqikj.top/gtdflhumjp.html

Py:   os.environ.get("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtsqolguzf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yvedp.cn/gtdqokqaep.html

JS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtzboxskdz.html

TS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtvfsqzdxt.html

Java: System.getenv("HOME")
来源：http://hz.ywan-chungtsiang.top/gtnrswtyrt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cqqwz.cn/gtvmjxywhp.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtnxhyyrdg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dashuyun.cn/gtkruoeaxg.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtpauybfgb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtiitygycf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yongpay.top/gtjfkbypah.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtiyzcedff.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtgheblnoa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jlsjyb.cn/gtnuxxupfk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtrqgthhdm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtogtrduwp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258888.top/gtdmkibzgw.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gtjmgxutwy.html

Py:   os.getcwd()
来源：http://hz.nanxinkj.top/gtqojvssxx.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtnexwdacr.html

JS:   process.cwd()
来源：http://hz.gotoacloud.top/gthhftxbof.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gthkymxuyn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xinyue.icu/gtytnbkuqs.html

Go:   os.Getwd()
来源：http://hz.meibo888.top/gtihciiqpl.html

Ruby: Dir.pwd
来源：http://hz.zhixingplan.top/gtrpbykgde.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtillcfwgr.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtwcpjrfno.html

Py:   sys.exit(1)
来源：http://hz.hammf.cn/gtvmtsdqzo.html

PHP:  exit(1);
来源：http://hz.jqgfzy.top/gtahpkmknu.html

JS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtdhzfcgvy.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gtgoledwtz.html

Java: System.exit(1)
来源：http://hz.iojbl.cn/gtfrngiekf.html

Go:   os.Exit(1)
来源：http://hz.birdmap.top/gteeqzkxlc.html

Ruby: exit 1
来源：http://hz.aizwys.cn/gtlvrmwuaz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fzhhl.top/gteeelszvs.html

[M06] 向标准错误输出
来源：http://hz.chenlongwang.top/gtzitbmvzi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtuifofqji.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtkusllydf.html

JS:   console.error("err")
来源：http://hz.sxryk.cn/gtyresvnrk.html

TS:   console.error("err")
来源：http://hz.yj202588.top/gtzzysiirk.html

Java: System.err.println("err")
来源：http://hz.dianchejie.cn/gtcfbuhaut.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtzwcbwkwe.html

Ruby: warn "err"
来源：http://hz.316326.xyz/gtxvftmmbb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258888.top/gtjflmkofv.html

[M07] 判断是否为主入口
来源：http://hz.zhaomingkeji.xyz/gtsmturzav.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtnioybcnr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gtigsliblj.html

JS:   require.main === module
来源：http://hz.jqgufenzy.top/gtnkrjldpy.html

TS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtlhwirgvb.html

Java: public static void main(String[] args)
来源：http://hz.shangyingyoupin.top/gtnromzxmv.html

Go:   func main()
来源：http://hz.cheryme.top/gtxykooxyo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hammf.cn/gtqolcqmla.html

C#:   static void Main(string[] args)
来源：http://hz.xuanzx.com/gtzsbboeth.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gthaobwfut.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj202588.top/gtchnkfmka.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtkqdpcvbl.html

JS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtlweuqnbb.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtcscfplef.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtnksjgoxm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenzaomai.com/gteekmyqxi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zdqjudy.top/gtszgrbjua.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtuaifyzpe.html

================================================================================
来源：http://hz.haohaochexian.top/gtkdjfmlpp.html

N. 数据结构与算法
来源：http://hz.jiagoushi.top/gtmlhtmakt.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtccvvraye.html

[N01] 二分查找（有序数组）
来源：http://hz.xuetiantiany.cn/gtkuorqtbi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxuanxn.top/gtwiyzoetu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shangyingyoupin.top/gtermvwnsj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtgtxzeoqm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtkmmhonom.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtcflknzwg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtkjkfsbxe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gaohongyu789.top/gtxedfdumv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hysaishi.cn/gtytuygymd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hongshengwenyu.top/gtcljglmxi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtmnwatbue.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtovwbvfsl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtymtrmdjh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtupyzpqbh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cdnleiting.top/gtfckpyebs.html

Go:   slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtxwczokfz.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtvfukntdt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tian-w.cn/gtlcuksbor.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtynemeqte.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.redwolf501.top/gtfcubbacd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hysaishi.cn/gtsctylycl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gtzujauffr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtgrwymevb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ivvv.top/gtkcqdwrlg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtmycyfprm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sufxvd.cn/gttowyuubi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtvhbanner.html

[N04] 斐波那契数列
来源：http://hz.cdnleiting.top/gtcpguflau.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtjvaktbni.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shangyingyoupin.top/gtonoofbmf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtxjotlbdq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtohbwecxr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yongpay.top/gtofbmbyuo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yanxiufei.cn/gtknfeyffq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtghjnhexg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.fzhhl.top/gtvtryfwsn.html

[N05] 最大公约数
来源：http://hz.aibaodan.cn/gtxkvouxbn.html

Py:   math.gcd(a, b)
来源：http://hz.tian-w.cn/gtujykvhwo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gthsinmkme.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtrkvctytg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtgwdcqddy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gtfqagccjk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cdnleiting.top/gtpzotimqj.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtjxuhpquf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tianlin.xyz/gtpfokxwlo.html

[N06] 判断回文字符串
来源：http://hz.ydzc1.top/gttjfuveva.html

Py:   s == s[::-1]
来源：http://hz.shuidangran.top/gtbymsdfns.html

PHP:  $s === strrev($s);
来源：http://hz.mhx1999.top/gtuamgncrq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtknjjkweo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtygdiwkfy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.bjfxy.top/gtsqbqumpj.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtrxhwznxi.html

Ruby: s == s.reverse
来源：http://hz.yanxiufei.cn/gtlhjpeeqn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtubrwmfrz.html

[N07] 两数之和（返回下标）
来源：http://hz.jianghu66.top/gtvslcnurh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtpjjjecon.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgufenzy.top/gtidpqsatk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtylmafvqs.html

TS:   // 手写 Map<string, number>
来源：http://hz.tianlin.xyz/gtsmhuomkq.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtufuhohcx.html

Go:   // 手写 map[int]int
来源：http://hz.gaohongyu789.top/gthmmmooxx.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gtaptmwbgb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtigrfedoj.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gthqfihujj.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtvpckfrws.html

PHP:  // 手写递归交换
来源：http://hz.zhijiandao.cn/gtkbpgchav.html

JS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtaycicgqe.html

TS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtaskddavv.html

Java: // 手写回溯递归
来源：http://hz.guannengcc.top/gteunfwvto.html

Go:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtfkweqrbx.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258.top/gtaaeaqnex.html

C#:   // 手写回溯递归
来源：http://hz.yonumen.top/gtfpolhprv.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtycadhuim.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yangfankeji.com/gtxynwpnac.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guannengcc.top/gtidvazxli.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yongpay.top/gtgbmkkeyk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtidneoqrg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sysykeji.top/gtloevqtws.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydjk.org.cn/gtdjhcbsyz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nwbrower.top/gthjhmixgb.html


<!-- 参考信息 -->