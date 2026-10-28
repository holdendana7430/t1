代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtdseoeudu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtkfkiwhcs.html

JS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtghjlccxo.html

TS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtjdctrmzn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hysaishi.cn/gtibtlpoku.html

Go:   json.Marshal(obj)
来源：http://hz.aibaodan.cn/gtfzdmzyqz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hywenlv.cn/gtcyzxiiet.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gtfsjazqcz.html

[K02] JSON 字符串转对象
来源：http://hz.daria6918.cn/gtnvbqpmpj.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtvpesczjz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gtmkyffotm.html

JS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtqiwdodon.html

TS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtksivlksh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xziqi.cn/gtacmyfiyz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtaogchsro.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtnhgvlzku.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuxming.cn/gtjrrmqnnk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gtcffvnijl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtshyoxirw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtcdagtaov.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtsqdnayag.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtmhwmxjfm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenzaomai.com/gtlkifyfmz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.vqdsnc.cn/gtfljafhhi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daria6918.cn/gtwhtndmie.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtzqnsdwdu.html

[K04] 读取 JSON 文件
来源：http://hz.guowangkeji.top/gtyfknwhob.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhengqikj.top/gtsaozzajo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gthchihqcl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtugqrgvje.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtzjugeudl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gtdvxtekkj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtrsczctas.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ehwqpu.com/gtedzywytb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuanzx.com/gtxsaubrdx.html

[K05] 深拷贝对象
来源：http://hz.0kj1m.cn/gtknwqyhmq.html

Py:   copy.deepcopy(obj)
来源：http://hz.feifeiyinyue.top/gtxcgjxrdf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nwbrower.top/gtpgzqriqa.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtktnpdrvf.html

TS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtftnyszor.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gtduolcuzk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gtzthwcsmq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.quarkkingdee.top/gthpficwdm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yueranfly.top/gthidjffhx.html

[K06] 解析 URL 查询串
来源：http://hz.dianchejie.cn/gtfrbolfuq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtwmefzcxr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guannengcc.top/gtxglznglt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gttkdwioxx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtjafwuvue.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.snrcjt.cn/gtqfeaumpu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gtdwmwpfdh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtmxasuoeq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhengqikj.top/gtbctijwoe.html

[K07] 进制转换
来源：http://hz.xylfe.cn/gtxbxrljmd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gttqubzfgt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gtmmzunwwv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtwimeyugz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtckbbrqqz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj20258.top/gtihxeapms.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jiagoushi.top/gtznswvdpt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dianchejie.cn/gtyezawdqn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtsuejrqvt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gtfvwlhwzh.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtmhlqcqei.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ybcxt.top/gtgxjsixlj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gttrvoalxn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtjixjlcid.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.birdmap.top/gtfoiumvol.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gttxiwlvaq.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtqgqmprmr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gtcotigmpn.html

================================================================================
来源：http://hz.birdmap.top/gtviraacsq.html

L. 网络请求
来源：http://hz.feifeiyinyue.top/gtfvropzhx.html

================================================================================
来源：http://hz.yuanzhike.top/gtulgpwmgj.html

[L01] 发送 GET 请求
来源：http://hz.zhaomingkeji.xyz/gthdfjmfrc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gterbpfubr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.kuanghao11.cn/gtswuxange.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtmzxpiwao.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gtcewacfsg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtdkxelwdo.html

Go:   resp, err := http.Get(url)
来源：http://hz.9152youxi.cn/gtezledxnt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aizwys.cn/gthxvsqgeu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtgkizhejm.html

[L02] 发送 POST JSON
来源：http://hz.hammf.cn/gtxoraxgmn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.9152youxi.cn/gtplfvfsub.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtaqkovkqa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtyekqhxud.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtspwwdezl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtzdtvkezj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jqgfzy.top/gtupopzvwd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtwrwwkccl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuanzhike.top/gtwhimwqea.html

[L03] 设置自定义请求头
来源：http://hz.quarkkingdee.top/gtmsqcxyac.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tanke756.top/gtyfcjcptn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gtcemamfkn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtoqgmvhkb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtdsekqptl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cheryme.top/gtdcgsghkz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtrtunfusk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cqqwz.cn/gtaywnyyup.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.316326.xyz/gtyjgxubnh.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gtanxqppyz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.c1oappe.top/gtartvbggo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xingfuxueyuan.xyz/gtgcarfzvj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gtlyquwadp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtavjbeuxm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jiagoushi.top/gtvtdudkpw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtgtoaqphq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xylfe.cn/gteheuksfk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xziqi.cn/gtnimlnwqb.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gtgfnthkgg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dashuyun.cn/gtgyejtylx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gtgrvmejue.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtzounwqcj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtgitqnide.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhixingplan.top/gtrmhrimod.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ywan-chungtsiang.top/gtyhysobsh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtjvpckodo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.pengpengdd.cyou/gtacjdjiac.html

[L06] 解析响应为 JSON
来源：http://hz.xingfuxueyuan.xyz/gtzrtwvuxp.html

Py:   resp.json()
来源：http://hz.jyoumei.cn/gtnfwidjhx.html

PHP:  json_decode($body, true);
来源：http://hz.fzhhl.top/gtgufgkssy.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtqlbfsdwy.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtbtnyoymx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtjercpkuh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtrnoxzycs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.bjfxy.top/gthydwzaet.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.smart0.xyz/gtoaovsefp.html

[L07] 处理 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtsibjldjr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtlzntjkpv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fzhhl.top/gttzuinbll.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtnhygaxkm.html

TS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtksryzbkq.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtqfiyxrqk.html

Go:   resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtxyefwrdy.html

Ruby: resp.code.to_i
来源：http://hz.yongpay.top/gtlnszgled.html

C#:   (int)resp.StatusCode
来源：http://hz.haohaochexian.top/gtupnlwhof.html

[L08] 并发请求多个地址
来源：http://hz.chenlongwang.top/gtyacrqvqf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nanxinkj.top/gtuzmcjshb.html

PHP:  curl_multi_init() 系列
来源：http://hz.pycfn.com/gtxiduqzqa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtgfivzfrw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtsbuvacfj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtturztkat.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cucudq.cn/gtidsyinyk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtytbtgdeg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigfzy.top/gtkpzhakuk.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqqxfyhar.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtahdtmjnp.html

================================================================================
来源：http://hz.ybcxt.top/gtymebgehd.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtlwjqvffz.html

Py:   sys.argv[1:]
来源：http://hz.feifeiyinyue.top/gtxpsnfred.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtocrbswmm.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtqotmwjib.html

TS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtdqhszeoz.html

Java: args 数组（main 方法参数）
来源：http://hz.zhoulong.xyz/gtiwjsphzs.html

Go:   os.Args[1:]
来源：http://hz.iojbl.cn/gtixffbngp.html

Ruby: ARGV
来源：http://hz.wangdashe.top/gtbouzhpiy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hongshengwenyu.top/gtdjfkvscb.html

[M02] 读取环境变量
来源：http://hz.sweek.top/gtxvgkvwjq.html

Py:   os.environ.get("HOME")
来源：http://hz.shangyingyoupin.top/gtvnjqzbwj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daxiang520.top/gtuqhghuvw.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gtsvofwhpv.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtkjbtwkhc.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtzdwdauvp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gtpyuclkjb.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtqvdiflkp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gaohongyu789.top/gtsfsejqws.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtcfyhxuvb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sxryk.cn/gtuidrhcoh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nwbrower.top/gtzcnwsznc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gtjhwraeva.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtifzrcvcl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtfwwildti.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cheryme.top/gtxwwoqyoy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zdqjudy.top/gtrpkjvzdr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hywenlv.cn/gtwvubiqtr.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtyemyqgvv.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtzxbmhrze.html

PHP:  getcwd();
来源：http://hz.shuidangran.top/gthcbppmgf.html

JS:   process.cwd()
来源：http://hz.sweek.top/gtryvclurw.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtugfygvcw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuxming.cn/gtiltzhjka.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtxrndsnwf.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gthyetpuai.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangkeji.top/gtgphnokwz.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtugdvsppq.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtkueamhcs.html

PHP:  exit(1);
来源：http://hz.xingfuxueyuan.xyz/gthbxksrio.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtpfvsjqrd.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtcxwajfzg.html

Java: System.exit(1)
来源：http://hz.hnxiangtu.top/gtcaojwwtk.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gtlllktgcr.html

Ruby: exit 1
来源：http://hz.snrcjt.cn/gtfxwbdxcl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnxiangtu.top/gtvxybuybz.html

[M06] 向标准错误输出
来源：http://hz.ppjwa.cn/gtldvtqrys.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenjidiqi.icu/gtkwbhxsov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuanzhike.top/gtbtsjjcxa.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtqhqvslgv.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtmysekiue.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtoxvhwhul.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtdrbqijaf.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtfmxkgfnh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtpjvzfrby.html

[M07] 判断是否为主入口
来源：http://hz.haohaochexian.top/gtislflpil.html

Py:   if __name__ == "__main__":
来源：http://hz.hfpthk.cn/gtssssiubm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daxiang520.top/gtujcykovw.html

JS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtsuysctns.html

TS:   require.main === module
来源：http://hz.zycfv.cn/gtpvxjblcg.html

Java: public static void main(String[] args)
来源：http://hz.c1oappe.top/gtwtfmsric.html

Go:   func main()
来源：http://hz.gzhubu.top/gtyrbxzvex.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangdashe.top/gtucvqdfzt.html

C#:   static void Main(string[] args)
来源：http://hz.smart0.xyz/gtygidxhqb.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gtzqyvdiro.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258.top/gtqtyyqfjx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.52xcode.cn/gtskqnawys.html

JS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtgpwkfmaw.html

TS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtkffjbgsz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gtzbbrfwoe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ehwqpu.com/gtqldsocgl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fzhhl.top/gttxllnflw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cdnleiting.top/gtqegpflbn.html

================================================================================
来源：http://hz.52xcode.cn/gtetplqvfy.html

N. 数据结构与算法
来源：http://hz.jqgufenzy.top/gtqqseoqdz.html

================================================================================
来源：http://hz.mhx1999.top/gtpcuxruhm.html

[N01] 二分查找（有序数组）
来源：http://hz.pengpengdd.cyou/gtuyflsrkz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hongshengwenyu.top/gtnobsnute.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fzhhl.top/gtaandzzkh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtwgvnxxhb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gttzlyrszd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtyawaadtu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gtdplbzebs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtrintqmvd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jianghu66.top/gtdtwefgei.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jyoumei.cn/gtprttekcb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtzfsrfqim.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtrzfddahp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtqigyaghj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtcqkktscq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhiwuduotai.top/gtvroqekct.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtudslnzxa.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gttmtyvqdj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhijiandao.cn/gtrllkhppn.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtqnxncuge.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gtlndfzuec.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtbekropdv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gthhaozjyk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtpsmwsexo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nwbrower.top/gtzdkxjbuh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yanxiufei.cn/gtfktqvpgl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtsvizospt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nanxuanxn.top/gtdnloockh.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gtdxqwweod.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtzsvhdtpy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sweek.top/gtflwrbrzg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtahvgslnc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtczwhkdhl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxuanxn.top/gtcogdppyo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtptehzsva.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtabcmaxwq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtcvlbnhkd.html

[N05] 最大公约数
来源：http://hz.jinyuanbaomall.cn/gthecyaxdo.html

Py:   math.gcd(a, b)
来源：http://hz.ydzc1.top/gtkycthvol.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtsvctjmgk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtswafllwr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtgklcsjtw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigufen.top/gtxsjrotlj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtrgevoewq.html

Ruby: a.gcd(b)
来源：http://hz.gogol.net.cn/gtltyapbqh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinyuanbaomall.cn/gtlrquteok.html

[N06] 判断回文字符串
来源：http://hz.shangyingyoupin.top/gtunxwawkp.html

Py:   s == s[::-1]
来源：http://hz.tanke756.top/gtieilthxd.html

PHP:  $s === strrev($s);
来源：http://hz.redwolf501.top/gtcvcteyrg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gthyvctiwr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtkxeanhdj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnqzz.top/gtqlsfqwui.html

Go:   // 双指针从两端比较
来源：http://hz.jqgufenzy.top/gtoubuoxgb.html

Ruby: s == s.reverse
来源：http://hz.haohaochexian.top/gtikscneon.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtvxgukxvh.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgufenzy.top/gtcwlyomdw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangshuangyany.cn/gtgbqyxull.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtuttyuqid.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhixingplan.top/gtrbiosnab.html

TS:   // 手写 Map<string, number>
来源：http://hz.yueranfly.top/gtpmogadrp.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtharlzwxb.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gttpswuusn.html

Ruby: // 手写 Hash
来源：http://hz.hammf.cn/gtlwwljsso.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gtfhdjbnpx.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gtjnaioaqt.html

Py:   itertools.permutations(arr)
来源：http://hz.zhiwuduotai.top/gtmnbbccgy.html

PHP:  // 手写递归交换
来源：http://hz.daria6918.cn/gtmdvdlrvf.html

JS:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtcpkocvgf.html

TS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtqcbvmcyj.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gttglhhzmr.html

Go:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtkwzpdvnt.html

Ruby: arr.permutation.to_a
来源：http://hz.jlsjyb.cn/gtgfukjfvz.html

C#:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtlpbemvdg.html

[N09] 栈与队列
来源：http://hz.mhx1999.top/gtbuuetpov.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gtguykeixa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hfpthk.cn/gtjskuikkc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtvkvizyfx.html


<!-- 参考信息 -->