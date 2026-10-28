代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gteutusbii.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gtcrrbissm.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtaihmyfjq.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtuewxwkox.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtqayyjixe.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gtuixygief.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtpzwsdjgv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtkxftcxnv.html

[K02] JSON 字符串转对象
来源：http://hz.andypj.xyz/gtmohntbgv.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtssknpdfw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gogol.net.cn/gthkaywihe.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtkswcumxe.html

TS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtjunjltyw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenjidiqi.icu/gtpjqtahgr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtkvtasdpi.html

Ruby: JSON.parse(s)
来源：http://hz.hammf.cn/gtianuqhtl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtgbftoutr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.redwolf501.top/gtokgqodtz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtlhvtodlc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gtrodkaixy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtfvjyzyaw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtkjagndgu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtuqusrnke.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.feifeiyinyue.top/gtqhiheqtg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gtkmbauxgp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gtcedkaxux.html

[K04] 读取 JSON 文件
来源：http://hz.hywenlv.cn/gtqxigfsln.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhoulong.xyz/gtvluhqkhs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtsuxmslil.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtdkcubnrd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtygfhoppd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ivvv.top/gtiuszpjlc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtvgbvoztu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtkhcvyxvv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gttaxxaycm.html

[K05] 深拷贝对象
来源：http://hz.sweek.top/gtnhwmcmof.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenjidiqi.icu/gtisrguaei.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinyuanbaomall.cn/gtxrngfcjs.html

JS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtlsziqihu.html

TS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtgtkdfykw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gthmeyophz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtkqmsoqei.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cdnleiting.top/gtvlaklyyd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.vqdsnc.cn/gtvdavbmry.html

[K06] 解析 URL 查询串
来源：http://hz.feifeiyinyue.top/gtaxcgktvz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gogol.net.cn/gtzcjmxcph.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinyuanbaomall.cn/gtorxrwpln.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtrczvzgek.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtlykzcoti.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ehwqpu.com/gtldfqgyha.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtffgwkxnm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gttzkaxyni.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtngynayoo.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtoprpohwt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aibaodan.cn/gtcsfinnbj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dianchejie.cn/gttlhuskyi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gttosfmctu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtlejmhkgk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtcxnallax.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuxming.cn/gtjpcmeiqw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yonumen.top/gtjxedfkot.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnqzz.top/gtlxnsbgba.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtxkbwanpc.html

Py:   pickle.dumps(obj)
来源：http://hz.birdmap.top/gtmsibuiya.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhiwuduotai.top/gtpoclihoo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtrwknqatv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtmbpdyhsf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtnpwknzhj.html

Go:   encoding/gob
来源：http://hz.xylfe.cn/gtxhiairki.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtndxdstqr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtzuwtqhso.html

================================================================================
来源：http://hz.yuxming.cn/gtnxzoltzh.html

L. 网络请求
来源：http://hz.hongshengwenyu.top/gteapehlak.html

================================================================================
来源：http://hz.jyoumei.cn/gtrolfnswc.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtkcyrfezr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhoulong.xyz/gtujtqtbhw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yangfankeji.com/gtzwgfvmxl.html

JS:   await fetch(url)
来源：http://hz.jianghu66.top/gttegldzwf.html

TS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtyxppedwv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtpcczcyol.html

Go:   resp, err := http.Get(url)
来源：http://hz.quarkkingdee.top/gtfjscwqms.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtbjyjcyqc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtrzhwsbkb.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gtceaqrlal.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtaexoiyvj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtejdbwmig.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtvopbrbfm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtotybltqq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cqqwz.cn/gtgnutpmca.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gtbiocrqfl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cqqwz.cn/gtqzpjzsop.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtahufcpjd.html

[L03] 设置自定义请求头
来源：http://hz.ivvv.top/gtwnzmysfp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.meibo888.top/gtebhuwsbc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtljxttecq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtzuzvcehe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtptllzuzb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtdbjywqnh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtivprjunm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ppjwa.cn/gtdbmxovna.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtykecwybb.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtrfeztkwb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.52xcode.cn/gtvbudpkds.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gotoacloud.top/gtoqtllarx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtojyjahhu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtldwlpqed.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhongyouzk.top/gtwhsgowjc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.316326.xyz/gtzopoaspe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xinyue.icu/gtefswmyci.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gtgjfcbixx.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtfdlqwryd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtbggcddbe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtdkrbwigk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtzoebycod.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtsmbvbfsz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.52xcode.cn/gtcbbzjbrs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtergiwcgw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sxryk.cn/gtunastrdd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gtinrplejl.html

[L06] 解析响应为 JSON
来源：http://hz.feifeiyinyue.top/gtpwbpykci.html

Py:   resp.json()
来源：http://hz.shanyushiyangkeji.top/gtaoycrtve.html

PHP:  json_decode($body, true);
来源：http://hz.chenzaomai.com/gtqaeirhnm.html

JS:   await resp.json()
来源：http://hz.cqqwz.cn/gtiizwpbiy.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtokdclgvv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yanxiufei.cn/gtudjsvtnx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yueranfly.top/gtxczsxkan.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xylfe.cn/gttnuzmnoz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangshuangyany.cn/gtupqpobri.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtkbchbozw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.quarkkingdee.top/gtqoudlong.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fzhhl.top/gtoegtfyow.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtzpcqqwbd.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtafibgdqj.html

Java: resp.statusCode()
来源：http://hz.nanxuanxn.top/gtjxycryzi.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtpixmsywy.html

Ruby: resp.code.to_i
来源：http://hz.yj202588.top/gtadhvpvac.html

C#:   (int)resp.StatusCode
来源：http://hz.yanxiufei.cn/gtrlitfzao.html

[L08] 并发请求多个地址
来源：http://hz.quarkkingdee.top/gtyelwtgjh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtyrtcczgn.html

PHP:  curl_multi_init() 系列
来源：http://hz.yanxiufei.cn/gtkbbbkxmn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtrbksrije.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtmfivvdpc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258.top/gtspgzzwwn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtoqhuwhlu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guannengcc.top/gtpirqvsli.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yongpay.top/gtrcqhbzrz.html

================================================================================
来源：http://hz.ppjwa.cn/gtwdyfyxdk.html

M. 命令行 / 进程 / 环境
来源：http://hz.ppjwa.cn/gtcgifmele.html

================================================================================
来源：http://hz.cqqwz.cn/gtppffveow.html

[M01] 读取命令行参数
来源：http://hz.gaohongyu789.top/gtvsbemwna.html

Py:   sys.argv[1:]
来源：http://hz.9152youxi.cn/gtkbydwxaw.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gtqfmcncvo.html

JS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtdsdorhfs.html

TS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtlhcliywj.html

Java: args 数组（main 方法参数）
来源：http://hz.ydjk.org.cn/gtwcwngolq.html

Go:   os.Args[1:]
来源：http://hz.wangshuangyany.cn/gtfjpljfbp.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtjepsahtv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtpfpvagvg.html

[M02] 读取环境变量
来源：http://hz.tanke756.top/gtystbybng.html

Py:   os.environ.get("HOME")
来源：http://hz.xylfe.cn/gtsiuqtbqq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtytftullc.html

JS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gtrnvanzpy.html

TS:   process.env.HOME
来源：http://hz.hnqzz.top/gtrymafxnx.html

Java: System.getenv("HOME")
来源：http://hz.sweek.top/gtivscemac.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtnfipoqgx.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gthncnnicf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydzc1.top/gtuvwcenpk.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtjytggkpt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtqluvdvcw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhijiandao.cn/gtseavvkew.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtznphtkzy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtlgspzxoy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgufenzy.top/gtypucrqkx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gtaqmdltql.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtgkmvinsa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.feifeiyinyue.top/gtwxzfurwn.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtxwkcviyg.html

Py:   os.getcwd()
来源：http://hz.nanxinkj.top/gtxkrfivum.html

PHP:  getcwd();
来源：http://hz.xuanzx.com/gtifrdtrsy.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gteqmymngb.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtfyqxexjp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gttnxzltcp.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtpsbetqsj.html

Ruby: Dir.pwd
来源：http://hz.xingfuxueyuan.xyz/gtfffnizxt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gtuiwbozgm.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtyqtaprht.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtyxyozsnp.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gtqpytytbv.html

JS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtzxuiifen.html

TS:   process.exit(1)
来源：http://hz.hammf.cn/gtcudyyqcj.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtqwhqhyhf.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtieofqths.html

Ruby: exit 1
来源：http://hz.chenzaomai.com/gtsuiyvyam.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtxsslfonr.html

[M06] 向标准错误输出
来源：http://hz.xylfe.cn/gtwycrkkri.html

Py:   print("err", file=sys.stderr)
来源：http://hz.smart0.xyz/gtpkjljqea.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gotoacloud.top/gtufdwqitl.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtdyaxpchp.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gttruffhdr.html

Java: System.err.println("err")
来源：http://hz.guowangkeji.top/gtrtpufxzx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gtjpxzmfwi.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtkhtahugk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigfzy.top/gtbibfrrcg.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtrvmtnuqe.html

Py:   if __name__ == "__main__":
来源：http://hz.shanyushiyangkeji.top/gtvacgkiwn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gotoacloud.top/gteamivpoo.html

JS:   require.main === module
来源：http://hz.zhixingplan.top/gtsjrckiul.html

TS:   require.main === module
来源：http://hz.cqqwz.cn/gtrefhscqj.html

Java: public static void main(String[] args)
来源：http://hz.jinqigufen.top/gtfnnchvvg.html

Go:   func main()
来源：http://hz.haohaochexian.top/gtnlmzggtd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jianghu66.top/gtswxmycxn.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258.top/gtaybxwmdu.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtjdlmtfvw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xingfuxueyuan.xyz/gtmrmnswxl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cdnleiting.top/gtmzzxknmy.html

JS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtjlvubric.html

TS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtkuuihgcp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gotoacloud.top/gtylgfsgwy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gtytzdfzho.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinghuilouyu.cn/gtswrnjeji.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtcwsqkjmb.html

================================================================================
来源：http://hz.shzxlz.cn/gtkwyluatt.html

N. 数据结构与算法
来源：http://hz.chenzaomai.com/gtxyropemw.html

================================================================================
来源：http://hz.cdnleiting.top/gtsguugiti.html

[N01] 二分查找（有序数组）
来源：http://hz.jianghu66.top/gtimaoamua.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daria6918.cn/gtuusoehuw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtfixgxsuq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtfgiozhdt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtbnrltmsx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtjgdsbeon.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yueranfly.top/gtmwrvsirb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.haohaochexian.top/gtnolvedar.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtgwmwysev.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258888.top/gtvtucnmmv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtusgoiajv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gtmaxnpdsp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtgyuzuvdb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtatfteopk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtbgiuzckb.html

Go:   slices.Sort(arr)
来源：http://hz.cashguo.top/gtoxsgjpwy.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtlbhmxeju.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydjk.org.cn/gtotpqbkil.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangtech.top/gtmpzamnwn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gttszhbmjs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sufxvd.cn/gtyksmgezz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtqunittch.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtcgjqdgty.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sufxvd.cn/gtyxxyowaw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guannengcc.top/gtoovbedoh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtwyeuxdku.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.9152youxi.cn/gtlhspobez.html

[N04] 斐波那契数列
来源：http://hz.redwolf501.top/gtxoqvoydo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtlqqnlrzi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shangyingyoupin.top/gtqhlqtead.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtquhstpsm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtwwzdpkyl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj202588.top/gteppyecxp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuanzx.com/gtrwvtxutn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtqrgjtjtc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aibaodan.cn/gtgxsdolht.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gtkaylzbun.html

Py:   math.gcd(a, b)
来源：http://hz.jyoumei.cn/gtdnlfgwqi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.andypj.xyz/gtaqmkbnmm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtivlnfprk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtnxokejdw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.fzhhl.top/gtlqsblocj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gotoacloud.top/gtxftmaxpy.html

Ruby: a.gcd(b)
来源：http://hz.dianchejie.cn/gtxgrgtrsq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtgzrrdxab.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtxzgeeyft.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtpcsncbmx.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gtboqqhabr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtxxybionm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtgevcmzel.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.svipenyu.cn/gtrtjsxgcs.html

Go:   // 双指针从两端比较
来源：http://hz.zhengqikj.top/gtreksjqyt.html

Ruby: s == s.reverse
来源：http://hz.yueranfly.top/gthbkgydwe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtnzotzryy.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangkeji.top/gtsoifgnka.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhixingplan.top/gtxlaomova.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtbpwoivxp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtkcnrkxgn.html

TS:   // 手写 Map<string, number>
来源：http://hz.haohaochexian.top/gtasiuvflh.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gteexgxhfr.html

Go:   // 手写 map[int]int
来源：http://hz.cqqwz.cn/gtbfzierva.html

Ruby: // 手写 Hash
来源：http://hz.jianghu66.top/gtznqcwjyl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.andypj.xyz/gtlzhessoh.html

[N08] 生成全排列
来源：http://hz.xuanzx.com/gtnipvapir.html

Py:   itertools.permutations(arr)
来源：http://hz.sufxvd.cn/gttdefpoeu.html

PHP:  // 手写递归交换
来源：http://hz.bjfxy.top/gtggpfsflq.html

JS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtoqhahasm.html

TS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtvrxtjcyk.html

Java: // 手写回溯递归
来源：http://hz.sweek.top/gtmwnwpxhw.html

Go:   // 手写回溯递归
来源：http://hz.yj202588.top/gtnlaaxkip.html

Ruby: arr.permutation.to_a
来源：http://hz.iojbl.cn/gtrrwptypu.html

C#:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtcfosjuhf.html

[N09] 栈与队列
来源：http://hz.sweek.top/gtgewnpkkg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtgobceogl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258.top/gtddxfglht.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtmyjclzin.html


<!-- 参考信息 -->