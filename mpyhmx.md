代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtkliqgdte.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gtvspoitoy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtrpgsvwfq.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtwcedkjqe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guowangkeji.top/gtmdjroxyx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtaddltksu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtoiofhgls.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtnymaruow.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtfggjqooa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtcwhokjey.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtddojypcd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.9152youxi.cn/gtufvmvjfd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.havefunace.top/gttgaocmfq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xziqi.cn/gtdcsmrgls.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtnwmlohdf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gtovmjgloy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sxryk.cn/gtmstxksuq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gteoaryeza.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gttngkthfm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gtnopqxnwq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtxykiccnm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtailunpng.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aibaodan.cn/gticeuluvo.html

[K05] 深拷贝对象
来源：http://hz.sufxvd.cn/gtmvmanvdm.html

Py:   copy.deepcopy(obj)
来源：http://hz.9152youxi.cn/gtmwivzbys.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aizwys.cn/gtbcimnzov.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtimydkcao.html

TS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtkbxcpyih.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtordaheru.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gteryfwcws.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.quarkkingdee.top/gtxqluuxbv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ppjwa.cn/gtvswkyxgr.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtapxfirtf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.andypj.xyz/gtvjfjydpw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xinyue.icu/gtxnqlpnde.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtgriybgps.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtlbqnhlgw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hammf.cn/gtejctlnul.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtttobhwks.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtbpnuxfxx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgufenzy.top/gttloqregi.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtourcurbl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtmsxdzwnn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gtlmgpqlet.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtqmfxipnc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtvuxjuryb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtuikngyik.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangdashe.top/gtylvjwlyk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hywenlv.cn/gtuudwhzkl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtaithkxfw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtpntxgdjr.html

Py:   pickle.dumps(obj)
来源：http://hz.xinyue.icu/gtdpvkohnu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenlongwang.top/gtvwilkkxu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtzjpjvifr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtsviyupfp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jiagoushi.top/gtwxgzygxn.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtfvquyuan.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxinkj.top/gtdehkxrjy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtyyvwjzns.html

================================================================================
来源：http://hz.jinqigufen.top/gtcczfgyss.html

L. 网络请求
来源：http://hz.nanxinkj.top/gteafmyolx.html

================================================================================
来源：http://hz.nanxinkj.top/gtohcxzzoi.html

[L01] 发送 GET 请求
来源：http://hz.feifeiyinyue.top/gtkvufswwb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cashguo.top/gtkahnhkik.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtqbbckaxs.html

JS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtytaidpst.html

TS:   await fetch(url)
来源：http://hz.zhoulong.xyz/gtrrnbszxq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtchrskqzq.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtgzatcutx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gthgapcslu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gthcsawmyk.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtyetyqqhc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuanzhike.top/gtolnmqcop.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtqflignqr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gthmgjwhlm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtlaegreul.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zycfv.cn/gtoekihkhk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtwxcsfhrr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtndxgulil.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gttuajpltc.html

[L03] 设置自定义请求头
来源：http://hz.cdnleiting.top/gtbzycusgj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigfzy.top/gtyxtqjwgo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtleyqqmdz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtkerthmdq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtdzbthaab.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gtrhjlntyk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gtqkkjxvfq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xylfe.cn/gtniudonfw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtvelynlzm.html

[L04] 设置超时
来源：http://hz.hfpthk.cn/gtjmrkgfyu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtolyphctv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ivvv.top/gtxtufnyne.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtqcstzbad.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gteganwaoa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtpyesfzcd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhongyouzk.top/gtzhpkjsty.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtjdljaijy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenzaomai.com/gtarsixogj.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258888.top/gtzcgawohe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xingfuxueyuan.xyz/gttwijfyjt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtuilgmbxu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtyyfhenie.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gtmganmdng.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtrrwchuja.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xylfe.cn/gthzltnewp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gtadjdwqll.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtfpvvzckl.html

[L06] 解析响应为 JSON
来源：http://hz.ywan-chungtsiang.top/gtbchsbcwx.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtwmshlioa.html

PHP:  json_decode($body, true);
来源：http://hz.yj20258.top/gtgckmluui.html

JS:   await resp.json()
来源：http://hz.yj20258.top/gtecwttmlo.html

TS:   await resp.json()
来源：http://hz.yj20258.top/gtsiiwnecb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtxpifrwzo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtgyyielsn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydjk.org.cn/gtiqtrbgsh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.316326.xyz/gttqatxrox.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtlyipeete.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jlsjyb.cn/gtpsjqzfrj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.mhx1999.top/gtsprmdpoh.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtuadijglp.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangkeji.top/gtbumvrcne.html

Java: resp.statusCode()
来源：http://hz.hfpthk.cn/gtwhhvwjja.html

Go:   resp.StatusCode
来源：http://hz.haohaochexian.top/gtsoiivldz.html

Ruby: resp.code.to_i
来源：http://hz.yongpay.top/gtslqwszpt.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtybijysqn.html

[L08] 并发请求多个地址
来源：http://hz.zhengqikj.top/gtgaoogafu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sufxvd.cn/gtejqwcegw.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtmauhqwpt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtmjznaykl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtkdedcusg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtqpwblzhb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.meibo888.top/gtabqqszzv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtrspwmoqj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydzc1.top/gtneegrhji.html

================================================================================
来源：http://hz.nwbrower.top/gtxvktxnyu.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtsfubpjlv.html

================================================================================
来源：http://hz.52xcode.cn/gtekxvipat.html

[M01] 读取命令行参数
来源：http://hz.sysykeji.top/gtclozjeva.html

Py:   sys.argv[1:]
来源：http://hz.pengpengdd.cyou/gtsmlggvlh.html

PHP:  $argv;  $argc;
来源：http://hz.hammf.cn/gtxvajfoxh.html

JS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtiaptxvln.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gttdnkttzt.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gttjvahtfh.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtfpatgjaw.html

Ruby: ARGV
来源：http://hz.shanyushiyangtech.top/gttxxioyqd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.316326.xyz/gtzqavomqv.html

[M02] 读取环境变量
来源：http://hz.52xcode.cn/gtohkjfnjm.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgfzy.top/gtdeeqvedh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ivvv.top/gthwcfktgw.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gtolckjhsy.html

TS:   process.env.HOME
来源：http://hz.yj202588.top/gtfarskbnq.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtnzvqlope.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtnrpqmcmw.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtajlpsaqm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gtjmhrbutk.html

[M03] 执行外部命令
来源：http://hz.iojbl.cn/gtcdvvunop.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yanxiufei.cn/gttloofbpy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtogivpzqp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtccyapfkc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtelpawojy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtpyhryltg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtxxtaswar.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtnjmlskun.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtkzoppqmh.html

[M04] 获取当前工作目录
来源：http://hz.hnxiangtu.top/gtumbbyogk.html

Py:   os.getcwd()
来源：http://hz.yj20258888.top/gtjbpzmtkj.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtkoupoebf.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gteoxvcqqv.html

TS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtlplgqidj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.c1oappe.top/gtundjowlq.html

Go:   os.Getwd()
来源：http://hz.yangfankeji.com/gtvqggyxdb.html

Ruby: Dir.pwd
来源：http://hz.ydjk.org.cn/gtuupznfcy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtgrinfmmj.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gtthwtinhm.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtnksjtjlc.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtftfnlnli.html

JS:   process.exit(1)
来源：http://hz.cashguo.top/gtqfsipykc.html

TS:   process.exit(1)
来源：http://hz.tian-w.cn/gthjmtbues.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtnlpeosbw.html

Go:   os.Exit(1)
来源：http://hz.pycfn.com/gtnetflrqr.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtqomaikrv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gtzormapwm.html

[M06] 向标准错误输出
来源：http://hz.xziqi.cn/gtewdjhyam.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtkukdqbmf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj202588.top/gtvscalfus.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtrqqyratr.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtistppuse.html

Java: System.err.println("err")
来源：http://hz.cdnleiting.top/gtexpdzcqg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.feifeiyinyue.top/gtdbbgklib.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtcgifaifm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigfzy.top/gtaxnarnjf.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtmzuvwogm.html

Py:   if __name__ == "__main__":
来源：http://hz.gogol.net.cn/gtxiieicbp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtxcdajvim.html

JS:   require.main === module
来源：http://hz.hywenlv.cn/gtrlosbyem.html

TS:   require.main === module
来源：http://hz.yj20258.top/gtesgvbhww.html

Java: public static void main(String[] args)
来源：http://hz.tian-w.cn/gtbckkmvrw.html

Go:   func main()
来源：http://hz.sysykeji.top/gttexrkgkx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenzaomai.com/gtjmifgmio.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtajtyqgmy.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtzpxwuvtd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtsjdaiohk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gotoacloud.top/gtzagachzn.html

JS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtrmdfbhqk.html

TS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtnxruszbc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhongyouzk.top/gtxyloklwv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gtfapybror.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.52xcode.cn/gtwmfnotqk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gtfrdsjooq.html

================================================================================
来源：http://hz.ydzc1.top/gttdnswazr.html

N. 数据结构与算法
来源：http://hz.shuidangran.top/gtxjrypksj.html

================================================================================
来源：http://hz.yonumen.top/gtkgyjsdwf.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangtech.top/gtwthehdxu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigufen.top/gtlhpxqvxi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gtgiymtfxu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtbdomcyhd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtfayifrql.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fzhhl.top/gtdmacwrmj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.birdmap.top/gtafvjpanj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtnhcjuuru.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daxiang520.top/gtrzjoxeqf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guowangkeji.top/gtovyvwlts.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxuanxn.top/gtdbtshiuy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cqqwz.cn/gtlxjhadpl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtzokicftz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtorxbbtys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fzhhl.top/gtnahehssw.html

Go:   slices.Sort(arr)
来源：http://hz.guannengcc.top/gtfvytkdcu.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtyxqykmco.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnxiangtu.top/gtldvbamti.html

[N03] 快速排序（分治示例）
来源：http://hz.shzxlz.cn/gteoozdjke.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtogianvmc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.0kj1m.cn/gtgpzmjida.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtujscilwx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtfpcfbyjg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhaomingkeji.xyz/gtdfsvxmbr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtezgqmvzq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sufxvd.cn/gtkmigthmv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtrfmiwgif.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtsjnrmiks.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtpltilwam.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhixingplan.top/gtoraobwjo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtbrelenwg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtkfmzflkf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cheryme.top/gtnjkcyeau.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cucudq.cn/gthapnxkss.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtdpypmnjj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydzc1.top/gtshlbnxuv.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtynsaxyft.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtzkrzawfp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydzc1.top/gtfncqafqh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtfktrxhnl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtddpjfmgw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhijiandao.cn/gtlscflsra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cqqwz.cn/gtvaksbrbp.html

Ruby: a.gcd(b)
来源：http://hz.shangyingyoupin.top/gtdewjjcmr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xingfuxueyuan.xyz/gtsudesruv.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtauwgzaqa.html

Py:   s == s[::-1]
来源：http://hz.yonumen.top/gtjyceealb.html

PHP:  $s === strrev($s);
来源：http://hz.shangyingyoupin.top/gtwjveqppp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtnkyednld.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtazywnmlf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guannengcc.top/gtxjsvtgcb.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtwrsmscon.html

Ruby: s == s.reverse
来源：http://hz.sweek.top/gtfqgedjne.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtodtgpwbq.html

[N07] 两数之和（返回下标）
来源：http://hz.andypj.xyz/gtslkzegfm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangtech.top/gtvkdpxkut.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cqqwz.cn/gtvccjswyg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtenqbbawi.html

TS:   // 手写 Map<string, number>
来源：http://hz.svipenyu.cn/gtkiajtodb.html

Java: // 手写 HashMap
来源：http://hz.hammf.cn/gtaetllnqu.html

Go:   // 手写 map[int]int
来源：http://hz.jlsjyb.cn/gtyjootjjn.html

Ruby: // 手写 Hash
来源：http://hz.jiagoushi.top/gtisknlexo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shangyingyoupin.top/gtvpmbaizp.html

[N08] 生成全排列
来源：http://hz.yj20258.top/gtdhislddp.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtrmndwdms.html

PHP:  // 手写递归交换
来源：http://hz.cdnleiting.top/gtzimqurmf.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtwtfqbvlr.html

TS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtjolkuryq.html

Java: // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtwylzexqg.html

Go:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtsjttvsbx.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtzegysfai.html

C#:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtvisdhajo.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtxrynsxpz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hfpthk.cn/gtszoqbfsc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuxming.cn/gtlcxfsvvq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258888.top/gtzyztuyxm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtrxibjlyo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guowangkeji.top/gtqtnsbdji.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtruutfshi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gthbggdqev.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangtech.top/gttvdmvysj.html

[N10] 链表节点定义
来源：http://hz.xuetiantiany.cn/gtdzvwdnal.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtiqtucrbb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.9152youxi.cn/gtyavokcdm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhixingplan.top/gtmtgfpdxc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtbpdhkbyu.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gtcuclzrxn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258888.top/gtqwvvlvoh.html


<!-- 参考信息 -->