代发 wailian999

[K02] JSON 字符串转对象
来源：http://hz.0kj1m.cn/gttpytlehc.html

Py:   json.loads(s)
来源：http://hz.yongpay.top/gtqjxobheh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sysykeji.top/gtgrqneejt.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtxhbcjqse.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtkoiboklb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gtbutqljhp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtnkhcgopa.html

Ruby: JSON.parse(s)
来源：http://hz.hnqzz.top/gtatdbxssa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gtemmvvjkw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtyictxrqy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtbxtpgsym.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtivrzzbzp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtfezeturp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gttoiejkce.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fengsongda.top/gtztcvccpr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gogol.net.cn/gtscdajuel.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tanke756.top/gttgzbqjnz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.316326.xyz/gtrcumtanl.html

[K04] 读取 JSON 文件
来源：http://hz.cdnleiting.top/gtpndabrid.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daxiang520.top/gtqzcrmytn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtvdotrsep.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gttljsglie.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtudajshlv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gtzrzraxbh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtvcyhtwoa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gtxukmndts.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.redwolf501.top/gtffrpsyrt.html

[K05] 深拷贝对象
来源：http://hz.yuxming.cn/gtkhnylqfc.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gtgasfwxyi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinyuanbaomall.cn/gtcjkcqinr.html

JS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtqnpuixfv.html

TS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtsbdarzbw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtpvtrcdyc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gtgwfpsbom.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ybcxt.top/gttndklymi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnxiangtu.top/gtvdudtpbs.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gtigxtqdia.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtculapfeh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gtiyqbkycv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtishgeopx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtipdkcqos.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuetiantiany.cn/gtdluukcgh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtulutexaj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtcchuhfaf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtnuieuvrr.html

[K07] 进制转换
来源：http://hz.zhongyouzk.top/gtqiukcceq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pengpengdd.cyou/gtdnslurtq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.9152youxi.cn/gtpopzvmrx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtcgofmmuz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtaswlmozf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtgepoixlh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtnlphuscv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xziqi.cn/gtmghqvckf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xziqi.cn/gtwvndinky.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtwfuekbno.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtvluknofm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xziqi.cn/gtleyhlatr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtiulozicg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gthjlqinzo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nwbrower.top/gtocqgztpa.html

Go:   encoding/gob
来源：http://hz.shanyushiyangkeji.top/gtdtrxrhta.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtwvqhrwvj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtyvxhlihf.html

================================================================================
来源：http://hz.chenzaomai.com/gtltmtvscx.html

L. 网络请求
来源：http://hz.ehwqpu.com/gtijvdkjtn.html

================================================================================
来源：http://hz.fzhhl.top/gtfoobqbsf.html

[L01] 发送 GET 请求
来源：http://hz.yonumen.top/gtoqrdyxyt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gtiiwimyub.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gtbvebhclk.html

JS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtibtzedsr.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtpqyrtxzv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hfpthk.cn/gtfrepzsqu.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtnnmasbeg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.birdmap.top/gtcymryaoj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigufen.top/gtgfiwhvcy.html

[L02] 发送 POST JSON
来源：http://hz.yangfankeji.com/gtadnbbgcz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtfbgpcxbv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtejhqlkrv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtlbgortrg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtuobjauad.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtebamvlmj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pengpengdd.cyou/gtdfpjxhvx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shuidangran.top/gtszutitkh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtckszboih.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gtwhzsnoys.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sweek.top/gtdafteiim.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhoulong.xyz/gtuxgtgejq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtsufjqttl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtajgnkogl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtnvxgnhcc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258.top/gtjwjvysrn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gtubhgqszl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtkwpsnbvx.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtutzzhkoq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.snrcjt.cn/gtsphukjez.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gtiglgfuly.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtdrflpqlm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtrufhhmpq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgfzy.top/gtcrvqdxdt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtebegrwtp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtjzfqinnv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtlexnhzbd.html

[L05] 上传文件（multipart）
来源：http://hz.aizwys.cn/gtromdtyqf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtuohjjfmf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnqzz.top/gtoxiqejhv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtzckhwtph.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtrpzeynpa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtqzqitxfc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xziqi.cn/gtxjsiolqc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hywenlv.cn/gtqbmmcast.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fengsongda.top/gtzbnsaapd.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gtslagrryp.html

Py:   resp.json()
来源：http://hz.daxiang520.top/gtoxsghmas.html

PHP:  json_decode($body, true);
来源：http://hz.sufxvd.cn/gtrvjarlfw.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gtcgyevlsv.html

TS:   await resp.json()
来源：http://hz.andypj.xyz/gtrwymwhll.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuetiantiany.cn/gttwerdwiw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtdmumijmp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gtkideirus.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258888.top/gttjukyaio.html

[L07] 处理 HTTP 状态码
来源：http://hz.sufxvd.cn/gtafcqvfry.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guannengcc.top/gtynrpsixx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhaomingkeji.xyz/gtehkabhot.html

JS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtxnmydkuf.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtymrvffec.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gtcwbaurfk.html

Go:   resp.StatusCode
来源：http://hz.zycfv.cn/gtggxinkmz.html

Ruby: resp.code.to_i
来源：http://hz.zhiwuduotai.top/gthulucrss.html

C#:   (int)resp.StatusCode
来源：http://hz.iojbl.cn/gtdtahxdun.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtpnybgabr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gtiaefhnna.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtoetzohxe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtbtyddpuo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtnvjpuyjq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nwbrower.top/gtsumcthzm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gtrymspzpq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj202588.top/gtjgtamacn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cucudq.cn/gtrisoawng.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmdjsicnv.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtgggqrpyt.html

================================================================================
来源：http://hz.mhx1999.top/gtatvrfjai.html

[M01] 读取命令行参数
来源：http://hz.cdnleiting.top/gttrzpqwni.html

Py:   sys.argv[1:]
来源：http://hz.cashguo.top/gttklyjbxh.html

PHP:  $argv;  $argc;
来源：http://hz.shzxlz.cn/gtyoqizcqh.html

JS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtchfoaxce.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtxejzkqrk.html

Java: args 数组（main 方法参数）
来源：http://hz.316326.xyz/gtdxpgrwdr.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gtjrwxpqlb.html

Ruby: ARGV
来源：http://hz.yj202588.top/gtfvbhyaao.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gtafmhuucr.html

[M02] 读取环境变量
来源：http://hz.ehwqpu.com/gthbgasfkv.html

Py:   os.environ.get("HOME")
来源：http://hz.cqqwz.cn/gtxztqnwov.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.iojbl.cn/gtnumdfzzs.html

JS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtlzwcdsnu.html

TS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtldkridln.html

Java: System.getenv("HOME")
来源：http://hz.gogol.net.cn/gtyblukdxn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yanxiufei.cn/gtclitkdjk.html

Ruby: ENV["HOME"]
来源：http://hz.daria6918.cn/gtpddqenee.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jiagoushi.top/gtmavuxdbw.html

[M03] 执行外部命令
来源：http://hz.sxryk.cn/gttmwufrnv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtnnuzqhwt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtcmccbhwl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gthzpjjoiw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gttanieajs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxuanxn.top/gtwwbdnlvg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ppjwa.cn/gtcgqshkxg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenzaomai.com/gtdrnynjxj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ivvv.top/gtwoztizni.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtobdjybay.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtyjqvwozg.html

PHP:  getcwd();
来源：http://hz.hnqzz.top/gtdahjuzbm.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gtfryooqcc.html

TS:   process.cwd()
来源：http://hz.xylfe.cn/gtkvpaopdq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtwummhztp.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtmrpkfmzg.html

Ruby: Dir.pwd
来源：http://hz.fengsongda.top/gtfzdolomm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtlbtuhlhw.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gtrunvdfyq.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtnhtnqmwk.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gtbbuwuolt.html

JS:   process.exit(1)
来源：http://hz.hammf.cn/gtwhmmrupz.html

TS:   process.exit(1)
来源：http://hz.yueranfly.top/gtvddeydcr.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtthditzeu.html

Go:   os.Exit(1)
来源：http://hz.zycfv.cn/gtqgrwfcmk.html

Ruby: exit 1
来源：http://hz.quarkkingdee.top/gtilkulkwk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tanke756.top/gtwpkpzlzb.html

[M06] 向标准错误输出
来源：http://hz.yj20258.top/gtiloivsld.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gteetnnwbz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.52xcode.cn/gttbuadvak.html

JS:   console.error("err")
来源：http://hz.tanke756.top/gtovdkdfie.html

TS:   console.error("err")
来源：http://hz.ppjwa.cn/gtxsgtxkwu.html

Java: System.err.println("err")
来源：http://hz.vqdsnc.cn/gtypnnodxr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtjdhnfwov.html

Ruby: warn "err"
来源：http://hz.andypj.xyz/gttztizjxy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtqssdlmcu.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gtbbtfhjfa.html

Py:   if __name__ == "__main__":
来源：http://hz.chenjidiqi.icu/gtuypfkqcb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sysykeji.top/gtbpkpfhmw.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtbdwsyihx.html

TS:   require.main === module
来源：http://hz.hnqzz.top/gtmqxdhkdo.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gtsujoqjri.html

Go:   func main()
来源：http://hz.haohaochexian.top/gtapwolnwo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnxiangtu.top/gthpqmwipy.html

C#:   static void Main(string[] args)
来源：http://hz.andypj.xyz/gtgzlflvgc.html

[M08] 获取系统与运行时信息
来源：http://hz.xuetiantiany.cn/gtjbxudbgb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gzhubu.top/gtgzvekszl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtrznsdmth.html

JS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtsiehbfyb.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtiompdhdg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yvedp.cn/gtyduhllzz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zycfv.cn/gtktghvrzg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.0kj1m.cn/gteftirvdp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtvyjgmpih.html

================================================================================
来源：http://hz.havefunace.top/gtmzznmkvz.html

N. 数据结构与算法
来源：http://hz.wangshuangyany.cn/gtflxrbhxu.html

================================================================================
来源：http://hz.jqgfzy.top/gtijruucqj.html

[N01] 二分查找（有序数组）
来源：http://hz.bjfxy.top/gtnydvzpfm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cucudq.cn/gtivpwrupj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gthwpzizlf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtkdurddii.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gteoylhacz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daria6918.cn/gtuukdukpo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xinyue.icu/gtnxhkyvvv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.iojbl.cn/gtwxlukkam.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ivvv.top/gtucrndfzf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gtocngukya.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtlgiejyct.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gttwbotxiv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gthzoebcmi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xylfe.cn/gtdpgjdbhz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gtbloqwbie.html

Go:   slices.Sort(arr)
来源：http://hz.tanke756.top/gtiydnzhhm.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtsgqsnzdl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtbzcdcujn.html

[N03] 快速排序（分治示例）
来源：http://hz.bjfxy.top/gtqmgfqqud.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yangfankeji.com/gttaeiitug.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtrsbjrzvz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtuurascsu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtaymypfyl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtlgmsvjlv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gthwwpcdyx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guannengcc.top/gtajwimzli.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtnllidjjb.html

[N04] 斐波那契数列
来源：http://hz.jinqigfzy.top/gtdtmandcg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtpkozylqg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.redwolf501.top/gtavibmtny.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtxxdgpppr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtjneylzjp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtxoifzeui.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gttriusxwk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gthrtvgypb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gtzkyquwmq.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtmjmvendz.html

Py:   math.gcd(a, b)
来源：http://hz.fzhhl.top/gtsqugkzwa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhixingplan.top/gtthknqzas.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtgddissvm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtgvatifws.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.redwolf501.top/gtlwavxrhp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtehrodktr.html

Ruby: a.gcd(b)
来源：http://hz.zhengqikj.top/gtachbbaiq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hongshengwenyu.top/gttztyxxzs.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gtarskhtia.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtkdjoaiec.html

PHP:  $s === strrev($s);
来源：http://hz.tianlin.xyz/gttlxizeuc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtviejddvz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gthdcylmfo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daxiang520.top/gtcrxnttvs.html

Go:   // 双指针从两端比较
来源：http://hz.haohaochexian.top/gtxhvtnpgy.html

Ruby: s == s.reverse
来源：http://hz.gotoacloud.top/gtefhkextd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.aibaodan.cn/gtsvtnzyqy.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtdghguuzr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xinyue.icu/gtbthjfomm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yongpay.top/gtjrlhtitj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gttwfqyjyz.html

TS:   // 手写 Map<string, number>
来源：http://hz.sufxvd.cn/gtfcvwuifh.html

Java: // 手写 HashMap
来源：http://hz.zdqjudy.top/gthzgebfzz.html

Go:   // 手写 map[int]int
来源：http://hz.shangyingyoupin.top/gtybisghlj.html

Ruby: // 手写 Hash
来源：http://hz.smart0.xyz/gtufkejcpa.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.9152youxi.cn/gtkwyzusre.html

[N08] 生成全排列
来源：http://hz.ivvv.top/gtilegoiqi.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtheujaiig.html

PHP:  // 手写递归交换
来源：http://hz.jianghu66.top/gtpyrufljk.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtfiqgojfm.html

TS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtmnbhtofc.html

Java: // 手写回溯递归
来源：http://hz.nwbrower.top/gtucgrhrng.html

Go:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtplupfzqa.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtmcpgztsj.html

C#:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtrrqarpfl.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtsgzxbncr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhixingplan.top/gtmhcuvmpp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pycfn.com/gtnvecurqe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtkqvjrfaa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtlcysjskv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.haohaochexian.top/gtsyrhzzgx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tanke756.top/gtrqienejo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtymjxjphw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.quarkkingdee.top/gtsntkqjlq.html

[N10] 链表节点定义
来源：http://hz.jinghuilouyu.cn/gtyquucmda.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtqjhxvwky.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgufenzy.top/gtpjdqvvub.html


<!-- 参考信息 -->