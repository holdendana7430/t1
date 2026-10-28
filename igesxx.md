代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guannengcc.top/gtdxscdamv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigufen.top/gtvaumuocg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xingfuxueyuan.xyz/gtqwkkldhn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ppjwa.cn/gtqnslwpie.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtmsgivois.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuxming.cn/gtkjyaxnpz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnxiangtu.top/gtoascqwup.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gthdtkrbgg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gttiekkwfx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.vqdsnc.cn/gtpcvfkfzj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hysaishi.cn/gtirzhvffj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuanzx.com/gtxzcwfhhp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.andypj.xyz/gtsewknrqx.html

[K07] 进制转换
来源：http://hz.zhaomingkeji.xyz/gtuapkxhwn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtufxofasn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuanzhike.top/gtkwubarlj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtrdeuxoyf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtayltehyq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtyvqxoeqx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cashguo.top/gtwsqvjokd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tanke756.top/gtiikgdijn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guannengcc.top/gtvedhwcba.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.feifeiyinyue.top/gtfhsmgpnx.html

Py:   pickle.dumps(obj)
来源：http://hz.gotoacloud.top/gtlpnguihn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gzhubu.top/gtvaevejvt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtlrjvrfyv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtlhavnvav.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ivvv.top/gtcpqrxlxh.html

Go:   encoding/gob
来源：http://hz.chenjidiqi.icu/gtxqajbehy.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gtofpkzufo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.vqdsnc.cn/gtvlmaytdt.html

================================================================================
来源：http://hz.ivvv.top/gtphslzhue.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtupjjehlv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtoceoumrq.html

[L01] 发送 GET 请求
来源：http://hz.bjfxy.top/gtsgmrptkm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtcuufbstv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtogzbvdtw.html

JS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtnjberlox.html

TS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtrmxrrzfg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtwldgbhbc.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigfzy.top/gteokvpvhx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.svipenyu.cn/gtssypcktn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gtesoefwkj.html

[L02] 发送 POST JSON
来源：http://hz.fzhhl.top/gtpulfxixe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.mhx1999.top/gtseepdnde.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cheryme.top/gtbmfzlyob.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtwyshzodj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgufenzy.top/gtpkvgcqga.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gtcqanvilv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhiwuduotai.top/gtmouuuknx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtkikcsvwm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtjjsxtqar.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtxuaipbuh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gtznkbajbd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.mhx1999.top/gtafchwvlc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gtjcehgfpy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtqpfzcggn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yonumen.top/gtnakgkrke.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtydcdwpij.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.smart0.xyz/gtayvgwlcb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtvoiwjdvz.html

[L04] 设置超时
来源：http://hz.snrcjt.cn/gtmlejfadq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ppjwa.cn/gtwowrtztg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinghuilouyu.cn/gtbzqodvjq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtdqqfqrwi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtiovnfhso.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtenoptumu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtcdehhteo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.vqdsnc.cn/gtoqtikbge.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sufxvd.cn/gtnzfuihnz.html

[L05] 上传文件（multipart）
来源：http://hz.nanxinkj.top/gtjzokhlwv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gtazkonybv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dashuyun.cn/gtiefecyas.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtkqybbkme.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtwrgqlhwp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zycfv.cn/gtbhcpnagd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.vqdsnc.cn/gtwdbaujbd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guowangkeji.top/gtdsnqqhli.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtfmwrhdqi.html

[L06] 解析响应为 JSON
来源：http://hz.yuxming.cn/gtdycxgdxz.html

Py:   resp.json()
来源：http://hz.hywenlv.cn/gtyqvkqzpm.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtdywszocz.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gthceucxan.html

TS:   await resp.json()
来源：http://hz.hnxiangtu.top/gthosmtacf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtcsjefnre.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gtpcvrhajk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shangyingyoupin.top/gthicndiyg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhaomingkeji.xyz/gtwznwopey.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigufen.top/gtnrdzkhlc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hongshengwenyu.top/gtlbhgycar.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnqzz.top/gtqgfigtjt.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gtrmjditqa.html

TS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtykonfbyv.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gtphneobis.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtucklyepe.html

Ruby: resp.code.to_i
来源：http://hz.yangfankeji.com/gtkorasein.html

C#:   (int)resp.StatusCode
来源：http://hz.daria6918.cn/gtcylmotse.html

[L08] 并发请求多个地址
来源：http://hz.jiagoushi.top/gtvxibgjsw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.9152youxi.cn/gtcfafusdq.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtphdegfyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtiuzbnuga.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtymehsvax.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtqeyfmkng.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xziqi.cn/gttyuabmwn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtjemcqysh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtgwzqotyn.html

================================================================================
来源：http://hz.zycfv.cn/gtjrodlulm.html

M. 命令行 / 进程 / 环境
来源：http://hz.52xcode.cn/gtoinyknzb.html

================================================================================
来源：http://hz.yuxming.cn/gtnhoxklzz.html

[M01] 读取命令行参数
来源：http://hz.vqdsnc.cn/gtzzwcbyaz.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtnhdxjpwe.html

PHP:  $argv;  $argc;
来源：http://hz.hongshengwenyu.top/gtxhpzwzri.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtijlixyry.html

TS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtdpgjvhef.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtutujrvyb.html

Go:   os.Args[1:]
来源：http://hz.shangyingyoupin.top/gthheidems.html

Ruby: ARGV
来源：http://hz.shanyushiyangkeji.top/gtzvnjjval.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtnkiulfxp.html

[M02] 读取环境变量
来源：http://hz.tianlin.xyz/gtcppdqqgb.html

Py:   os.environ.get("HOME")
来源：http://hz.jianghu66.top/gtvloabezt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtryzsfiej.html

JS:   process.env.HOME
来源：http://hz.yuxming.cn/gtucugxzrd.html

TS:   process.env.HOME
来源：http://hz.xinyue.icu/gtnvtysaag.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtbxxuupek.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gtwpvhxrwd.html

Ruby: ENV["HOME"]
来源：http://hz.dianchejie.cn/gtkvjaqbiu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tanke756.top/gtuyanuvva.html

[M03] 执行外部命令
来源：http://hz.ywan-chungtsiang.top/gtxfcpwyfn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gtsvhdtvmo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xingfuxueyuan.xyz/gtizmdhckh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtpienbkgy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtjuhvoazs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shangyingyoupin.top/gtjxfhlsxs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtyescgbkq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgfzy.top/gtbyqfjhcy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pengpengdd.cyou/gtdbvgcgmp.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangkeji.top/gtthpaffvc.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtjztjyjkm.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gtcgjuxnwi.html

JS:   process.cwd()
来源：http://hz.bjfxy.top/gtjfhdnojy.html

TS:   process.cwd()
来源：http://hz.zhixingplan.top/gtcupkuvpt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.vqdsnc.cn/gtkfoefxpe.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtmuhxasbt.html

Ruby: Dir.pwd
来源：http://hz.jinqigfzy.top/gtfpkedlos.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtwagmkwzw.html

[M05] 设置退出码
来源：http://hz.ydzc1.top/gthilbufcq.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtqysxbxwj.html

PHP:  exit(1);
来源：http://hz.xuetiantiany.cn/gtfyufozgz.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtaihyycza.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtcvficnei.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtfhzymsjr.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtpardufru.html

Ruby: exit 1
来源：http://hz.dianchejie.cn/gtbwcgsgqb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtwubewaqt.html

[M06] 向标准错误输出
来源：http://hz.cucudq.cn/gtzrcdmzcj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gttgaueovd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtxnxkzniy.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gteficuxqm.html

TS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtvyycpsou.html

Java: System.err.println("err")
来源：http://hz.ppjwa.cn/gtqpfhxcfs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gttzybzgsz.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtnncsulkc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtncuuvdva.html

[M07] 判断是否为主入口
来源：http://hz.hnqzz.top/gtlcygogrn.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtrcohhgmg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pengpengdd.cyou/gtebnkwcxe.html

JS:   require.main === module
来源：http://hz.hammf.cn/gtnzjlmeds.html

TS:   require.main === module
来源：http://hz.tian-w.cn/gtxwaphucl.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtvxuvxfsx.html

Go:   func main()
来源：http://hz.tianlin.xyz/gthgpjthvf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.c1oappe.top/gtjuofjson.html

C#:   static void Main(string[] args)
来源：http://hz.ywan-chungtsiang.top/gtgkptcusl.html

[M08] 获取系统与运行时信息
来源：http://hz.tianlin.xyz/gtwvikwapj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.vqdsnc.cn/gtdhdaazct.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jiagoushi.top/gtygobgell.html

JS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtgdsyikct.html

TS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gttfhjbyfc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.9152youxi.cn/gtemchympp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.daxiang520.top/gtqqnewosw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinghuilouyu.cn/gtcxlnlpyh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gtufzajxgb.html

================================================================================
来源：http://hz.andypj.xyz/gtmorhxbpu.html

N. 数据结构与算法
来源：http://hz.shuidangran.top/gtqdgtkmwv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtllhswlwz.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtlzbuhshp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.havefunace.top/gtyxeyrbav.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hammf.cn/gtgtbuzgij.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gtsugatnay.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gttapwfdcu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtlqmlwkmm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gtsujnsqls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtyiixdjhn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nwbrower.top/gthhiezfqh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fengsongda.top/gtwxvnnliv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gteheunzor.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nwbrower.top/gtjwrvibvu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtupxpunmp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtlufqmizg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sufxvd.cn/gteqigxcbn.html

Go:   slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtkmxynfuh.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtltuswuhq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhoulong.xyz/gtwpsroeqh.html

[N03] 快速排序（分治示例）
来源：http://hz.aizwys.cn/gtvlnxssfq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangdashe.top/gtsbmqglog.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuetiantiany.cn/gtgvbvbwdl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtowqrfbwy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtvojaewea.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tianlin.xyz/gtmtnrnadw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhengqikj.top/gtaehqzpgx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtphxctlrd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nanxinkj.top/gtvtlboabo.html

[N04] 斐波那契数列
来源：http://hz.pycfn.com/gtablrkkfm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtpiobdhoi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtdnkofemt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gtcxrehafj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtxvcflplt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtrpciicwg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gogol.net.cn/gtyphydsbx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtmqjvarsn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.snrcjt.cn/gtsicsvfex.html

[N05] 最大公约数
来源：http://hz.jqgufenzy.top/gtwzffhruo.html

Py:   math.gcd(a, b)
来源：http://hz.jinyuanbaomall.cn/gtgozqojft.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hongshengwenyu.top/gtqtmzlijf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtsmgqmjei.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtmhndvjru.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shzxlz.cn/gtmihynvkb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtnwxjkpup.html

Ruby: a.gcd(b)
来源：http://hz.nwbrower.top/gtgetscbpu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtwfslgtab.html

[N06] 判断回文字符串
来源：http://hz.daxiang520.top/gtcwdazlzn.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gtlvnlmjpq.html

PHP:  $s === strrev($s);
来源：http://hz.bjfxy.top/gtcfrwbpyq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gttlllmphm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtqzqodmju.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gtlqcwyflz.html

Go:   // 双指针从两端比较
来源：http://hz.hnqzz.top/gtedrfzukn.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtsiqulcle.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtxwdpqxqn.html

[N07] 两数之和（返回下标）
来源：http://hz.gaohongyu789.top/gtncnonzdw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtshopwadt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gtuzqfjnqq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtmfqajftx.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gtgnuamynb.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtgcjcomte.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gtinbpwucp.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtrvnhjefj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hongshengwenyu.top/gtliycqizr.html

[N08] 生成全排列
来源：http://hz.xingfuxueyuan.xyz/gtlxsoaouw.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gtwevaanml.html

PHP:  // 手写递归交换
来源：http://hz.mhx1999.top/gtqlphuzfq.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtlyembhsn.html

TS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtoaxwhnfs.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtylnldtiu.html

Go:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtqiorqwyn.html

Ruby: arr.permutation.to_a
来源：http://hz.guowangkeji.top/gtzspxjeyk.html

C#:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtntmumyfs.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gttalkuwav.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xuanzx.com/gtgwpqumci.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.316326.xyz/gtjtftqdwc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fengsongda.top/gtsarlrsgq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtpusxofpq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gtiwdzuojx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yangfankeji.com/gtfgjotdiu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gtqravonok.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gtghuhsnpg.html

[N10] 链表节点定义
来源：http://hz.guannengcc.top/gtudprayom.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shangyingyoupin.top/gthxfthwkp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yongpay.top/gtyhxnbxdj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sxryk.cn/gtarlergmo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.svipenyu.cn/gtuzlrjsqp.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gthswmglci.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.svipenyu.cn/gtjimguivt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yueranfly.top/gtfpboleny.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangkeji.top/gtibmjawdp.html

[N11] 二叉树中序遍历
来源：http://hz.mhx1999.top/gtqxqtekzj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yueranfly.top/gttcyllxvd.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtjgbdlxfl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtaoixlphz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangtech.top/gturrbarwx.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtyvlmknbp.html

Go:   // 手写递归
来源：http://hz.ydzc1.top/gtrxkbwrgo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.9152youxi.cn/gttobokrlm.html

C#:   // 手写递归
来源：http://hz.snrcjt.cn/gtkrwnywtk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.c1oappe.top/gtwwpbuoht.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xylfe.cn/gtucjqdwxj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnxiangtu.top/gtqtmmnfgl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtrwukhnuq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gteitxrqht.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtioegrmpt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtiwpgphlf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtlziqycqn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtymyxvebw.html

================================================================================
来源：http://hz.dianchejie.cn/gtdrmrkqro.html

O. 并发与异步
来源：http://hz.gotoacloud.top/gtcsaivvai.html

================================================================================
来源：http://hz.dashuyun.cn/gtznpohlvu.html

[O01] 启动一个线程
来源：http://hz.shanyushiyangtech.top/gtrvjvgvhf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sweek.top/gtcguuvota.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yueranfly.top/gtzfnjjdvw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.redwolf501.top/gtuqycampj.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtwuqmndcx.html


<!-- 参考信息 -->