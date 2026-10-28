代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhengqikj.top/gtlbaiimtp.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gtlobwauxu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydzc1.top/gtioognirr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtskrdqpvh.html

[K02] JSON 字符串转对象
来源：http://hz.daria6918.cn/gtloghalra.html

Py:   json.loads(s)
来源：http://hz.dashuyun.cn/gtvhssuqsm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hammf.cn/gtgmmvgama.html

JS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gttjqjatpk.html

TS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtvlgduhww.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtsnznerkc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtebayaelc.html

Ruby: JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtiasnhwau.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.snrcjt.cn/gtzypsnqwn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ivvv.top/gthnodiouu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtdgfpwefe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtdsbcfgxt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gteuggsmpw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtwveantrp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.iojbl.cn/gthsskgnjv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtcincjxsw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgufenzy.top/gtxlzfkccw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gtjvpcdmxh.html

[K04] 读取 JSON 文件
来源：http://hz.hongshengwenyu.top/gtbrnvhqwg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gtxyukbjoa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gttqxccuff.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gtivvodurg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtusitnzng.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tianlin.xyz/gtkcyeiakh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gthcmacirb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gttsxjqvfj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xinyue.icu/gtfwbqwixq.html

[K05] 深拷贝对象
来源：http://hz.mhx1999.top/gtrwtdgoel.html

Py:   copy.deepcopy(obj)
来源：http://hz.cheryme.top/gtsvtmcyku.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gtucqpcqzf.html

JS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtczokqehs.html

TS:   structuredClone(obj)
来源：http://hz.nanxinkj.top/gtuqsmmuyl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gttwrfkgac.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.feifeiyinyue.top/gtbhnmpwia.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtyawygytt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sweek.top/gtiyhlktfm.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtzlshltgc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtxuvbxyqy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.svipenyu.cn/gtpzjzcyjn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtbmeycmtg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtrfpqzkbz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangtech.top/gttttzjtky.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ppjwa.cn/gtapqkahjp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xziqi.cn/gtrqhhfpsl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtuqhkmeni.html

[K07] 进制转换
来源：http://hz.aibaodan.cn/gtswnuflpo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daria6918.cn/gtqlvvbwsz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangtech.top/gtchomouoc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtksmeefyg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gttsdmohln.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtqytcfhch.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zycfv.cn/gtjxiombne.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.bjfxy.top/gtreycfhxq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigufen.top/gtlseozfes.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yvedp.cn/gtkvoyiskx.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gtmncsnezt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xinyue.icu/gtxbntqjim.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtscumoozv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtqxuwwhfg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.vqdsnc.cn/gtflxyyudz.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtagpnxiok.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtznwsyrpm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gtplcwoouj.html

================================================================================
来源：http://hz.wangdashe.top/gtcokfybze.html

L. 网络请求
来源：http://hz.fzhhl.top/gttdyptcaz.html

================================================================================
来源：http://hz.hywenlv.cn/gtvfntkmou.html

[L01] 发送 GET 请求
来源：http://hz.chenlongwang.top/gtlqxkrfem.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtuxsrthun.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gttouzyats.html

JS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtrholdokr.html

TS:   await fetch(url)
来源：http://hz.iojbl.cn/gtdcggoqfn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.bjfxy.top/gtvqzkustv.html

Go:   resp, err := http.Get(url)
来源：http://hz.9152youxi.cn/gtxdozwcis.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ehwqpu.com/gtvvxtijkn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigfzy.top/gtpufcelxo.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gteajycaix.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shzxlz.cn/gtlviroarl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jianghu66.top/gtxxiqumcs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtxonvxchf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtiytxuovb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.snrcjt.cn/gtynngtzgn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtwwiezolp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gtjscrgjtm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgfzy.top/gtepwfhbin.html

[L03] 设置自定义请求头
来源：http://hz.jinqigufen.top/gtrgifipiq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jiagoushi.top/gtmzumocup.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sweek.top/gteglzglwf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydzc1.top/gtwzerqsjd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtjzvjcusy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ehwqpu.com/gtccipgwqz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258888.top/gticfsatpy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daria6918.cn/gtflersqpb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtnnnokbui.html

[L04] 设置超时
来源：http://hz.xingfuxueyuan.xyz/gtqnmbmffm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gthhkcpcul.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtxhhlphcd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtqprhhphb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gtiapeinnu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtxgigbeii.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.0kj1m.cn/gtlhsxnejj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangshuangyany.cn/gtsinwbmlp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtulslwqdt.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gthwuevorn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtotaoveej.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ywan-chungtsiang.top/gtrnmzhrrc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtogxbzvwb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtokbebvbj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gtljnvzdgt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.kuanghao11.cn/gteajetzgt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.vqdsnc.cn/gtdwtxnkne.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gtlleswuqb.html

[L06] 解析响应为 JSON
来源：http://hz.ivvv.top/gtpksqgdmf.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gtaqramcag.html

PHP:  json_decode($body, true);
来源：http://hz.52xcode.cn/gtbpasfcoy.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtmrdzrfil.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gtqrnqgysm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.0kj1m.cn/gtsacccvbx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydzc1.top/gtciiunlqs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.iojbl.cn/gtftxjvpjk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigufen.top/gtrnwbrzih.html

[L07] 处理 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtlmxmnysq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yvedp.cn/gtnsdugmox.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtsefrbski.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtkjyufxvv.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtnzqejgtr.html

Java: resp.statusCode()
来源：http://hz.hnqzz.top/gtyjieicvl.html

Go:   resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtqutfiqky.html

Ruby: resp.code.to_i
来源：http://hz.sufxvd.cn/gtnsylahah.html

C#:   (int)resp.StatusCode
来源：http://hz.fengsongda.top/gtcaqhhwyw.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtswlnzakf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.c1oappe.top/gtknonznfy.html

PHP:  curl_multi_init() 系列
来源：http://hz.c1oappe.top/gtoplhkuuz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtpxdukrys.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtzgkzlpxb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.haohaochexian.top/gttzpmyfio.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gtmfqqcdou.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yueranfly.top/gtuevfqghv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gthncvpzdi.html

================================================================================
来源：http://hz.daxiang520.top/gthuptadgo.html

M. 命令行 / 进程 / 环境
来源：http://hz.yonumen.top/gtuctrimcu.html

================================================================================
来源：http://hz.jianghu66.top/gtjvknhzjl.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gtjkffqjmb.html

Py:   sys.argv[1:]
来源：http://hz.9152youxi.cn/gtotxbrtnw.html

PHP:  $argv;  $argc;
来源：http://hz.ydjk.org.cn/gtilydkqyo.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtbsclhuhj.html

TS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtnxdizxdf.html

Java: args 数组（main 方法参数）
来源：http://hz.xylfe.cn/gtfcivbmph.html

Go:   os.Args[1:]
来源：http://hz.shzxlz.cn/gtgkmloudi.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtkkisejso.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ybcxt.top/gtxunhfjav.html

[M02] 读取环境变量
来源：http://hz.ydzc1.top/gtevzakuff.html

Py:   os.environ.get("HOME")
来源：http://hz.hysaishi.cn/gtofxyhgzc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gtcqgsosnr.html

JS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtssrtinnq.html

TS:   process.env.HOME
来源：http://hz.yonumen.top/gtgwbgnepv.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtaefcpnpt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhoulong.xyz/gtrgndzaxo.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtfpwwogxi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtopouusyq.html

[M03] 执行外部命令
来源：http://hz.hfpthk.cn/gtvrkdoypc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.haohaochexian.top/gtogiqbhmj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shangyingyoupin.top/gtzyzpuppi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtjzptktso.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtsblaozes.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zdqjudy.top/gtlccmshwe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhijiandao.cn/gtjyavhnxw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.birdmap.top/gtzzbfkqyo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cdnleiting.top/gttpzoqsai.html

[M04] 获取当前工作目录
来源：http://hz.cdnleiting.top/gttjjyalkh.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtizrxxwnr.html

PHP:  getcwd();
来源：http://hz.jinqigfzy.top/gtvpialwrr.html

JS:   process.cwd()
来源：http://hz.gzhubu.top/gtvpjthpey.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gteryvwmmc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigufen.top/gtjjdonugi.html

Go:   os.Getwd()
来源：http://hz.birdmap.top/gtbwtannpu.html

Ruby: Dir.pwd
来源：http://hz.gotoacloud.top/gtrjozghfw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gogol.net.cn/gtlfbmjkkh.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtybtdspvd.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtyardhfla.html

PHP:  exit(1);
来源：http://hz.jianghu66.top/gtmzhimtmi.html

JS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtsalsevgd.html

TS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtcnrdwqii.html

Java: System.exit(1)
来源：http://hz.haohaochexian.top/gtcilnnryo.html

Go:   os.Exit(1)
来源：http://hz.jinghuilouyu.cn/gtrxpawtml.html

Ruby: exit 1
来源：http://hz.zdqjudy.top/gtwqmbmajd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenzaomai.com/gtvgcpgzgy.html

[M06] 向标准错误输出
来源：http://hz.cucudq.cn/gtyrbkxmpt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtlafzumgl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cheryme.top/gtvdpupclr.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtblcapluo.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtajpgkvak.html

Java: System.err.println("err")
来源：http://hz.yueranfly.top/gtjhhovaeg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gthykygsbz.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtrplrobwx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.c1oappe.top/gtoksfdwgp.html

[M07] 判断是否为主入口
来源：http://hz.havefunace.top/gtpzegpvfg.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258888.top/gtcmbwfrik.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtpyefhfgx.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtrujgrgmb.html

TS:   require.main === module
来源：http://hz.zhoulong.xyz/gtmblsecsn.html

Java: public static void main(String[] args)
来源：http://hz.sxryk.cn/gtchuvklkm.html

Go:   func main()
来源：http://hz.xziqi.cn/gttcjucjoy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.52xcode.cn/gtbapiavmc.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gthzmyguki.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gtkzhnttac.html

Py:   platform.system();  platform.python_version()
来源：http://hz.bjfxy.top/gtdinaojud.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhongyouzk.top/gtjutknoxk.html

JS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gtwptjhojj.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtgslbjnct.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.0kj1m.cn/gtrnisatxz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenjidiqi.icu/gtxdzuslfv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gtxftwbrme.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.c1oappe.top/gtayzimtvw.html

================================================================================
来源：http://hz.tianlin.xyz/gtunpswzth.html

N. 数据结构与算法
来源：http://hz.cucudq.cn/gtanvjhvkb.html

================================================================================
来源：http://hz.ydzc1.top/gthzmpzrdh.html

[N01] 二分查找（有序数组）
来源：http://hz.xuanzx.com/gtdkqceywg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.andypj.xyz/gtnmxvxqne.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.9152youxi.cn/gtygelctng.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtkdpzkhqd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtgefpubft.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtzcmhtlwi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuxming.cn/gtkjggeugn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fzhhl.top/gttyynljku.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pycfn.com/gtpccfoqdl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.9152youxi.cn/gtfdnanzpr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhiwuduotai.top/gtjumgxwhe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangdashe.top/gttivjwipw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtvoljrbnz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtinxdneee.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gtssvkxdjw.html

Go:   slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtauisvgpw.html

Ruby: arr.sort
来源：http://hz.xinyue.icu/gtrogqnsaq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cheryme.top/gtsmcvzesk.html

[N03] 快速排序（分治示例）
来源：http://hz.yangfankeji.com/gtlnldncnb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tianlin.xyz/gtvcmfakdp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gthidjttdi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gtjrnpesmw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtidelcclb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gtaeikxdfx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fzhhl.top/gtqujgansi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sysykeji.top/gtkxlvdalw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtxwvqqxfj.html

[N04] 斐波那契数列
来源：http://hz.yvedp.cn/gtqbprgbky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtemdkkvur.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.andypj.xyz/gtedndmymq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtgxyhgbuo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gtrnvccibp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.iojbl.cn/gtkuvzgbwn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hfpthk.cn/gtobtwcgpx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtsyjzvcmd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtyxznhpeu.html

[N05] 最大公约数
来源：http://hz.xziqi.cn/gtdnukxqpp.html

Py:   math.gcd(a, b)
来源：http://hz.9152youxi.cn/gthscadbsz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gzhubu.top/gtsslcyqvb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtvryxiuyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shuidangran.top/gtchtliawk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sufxvd.cn/gtyspzgbwj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258888.top/gtxhntddxa.html

Ruby: a.gcd(b)
来源：http://hz.jinyuanbaomall.cn/gtvpawzufr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.iojbl.cn/gtnznbcfpm.html

[N06] 判断回文字符串
来源：http://hz.yueranfly.top/gtznspvpry.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtmwaoxxrl.html

PHP:  $s === strrev($s);
来源：http://hz.bjfxy.top/gtxdkjbihr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtsmosyzzo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtakvxxtku.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jlsjyb.cn/gtbezybkbs.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gtdlcalxml.html

Ruby: s == s.reverse
来源：http://hz.jianghu66.top/gtdarrfedl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtddtgbjyu.html

[N07] 两数之和（返回下标）
来源：http://hz.shzxlz.cn/gtemvanivq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ywan-chungtsiang.top/gtqyqornol.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cdnleiting.top/gtiifgecpj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gtqlibxbfe.html

TS:   // 手写 Map<string, number>
来源：http://hz.sysykeji.top/gtovjulmod.html

Java: // 手写 HashMap
来源：http://hz.chenjidiqi.icu/gtgotyiipg.html

Go:   // 手写 map[int]int
来源：http://hz.xuetiantiany.cn/gtaxbdvbxr.html

Ruby: // 手写 Hash
来源：http://hz.jinghuilouyu.cn/gttydrbuds.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hywenlv.cn/gttdgnwsgc.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gtbjlmlwim.html

Py:   itertools.permutations(arr)
来源：http://hz.0kj1m.cn/gtnpszebur.html

PHP:  // 手写递归交换
来源：http://hz.xingfuxueyuan.xyz/gtajnpjawq.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtruqkvatb.html

TS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gttsozvszy.html

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gtgkyzllcd.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtaqrjxxrh.html

Ruby: arr.permutation.to_a
来源：http://hz.jianghu66.top/gtfenlluam.html

C#:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtbmzeruky.html

[N09] 栈与队列
来源：http://hz.hywenlv.cn/gtkibrfghf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gtovtvnsdp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.meibo888.top/gtezfpvmxg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtqtksilfv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jlsjyb.cn/gtdajfxvrj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daria6918.cn/gthacsdkmq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtiflsoecy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.0kj1m.cn/gthnyteeaw.html


<!-- 参考信息 -->