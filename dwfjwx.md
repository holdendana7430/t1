代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtiufvoxuz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.birdmap.top/gtepfprhmm.html

[K04] 读取 JSON 文件
来源：http://hz.svipenyu.cn/gtttkxgcta.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.andypj.xyz/gtcpqgsooz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtjqwlfral.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtuegrjduq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtwauuoprs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxinkj.top/gtsettjstq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtjldvzxjq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jlsjyb.cn/gttdwfmpgw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hfpthk.cn/gtgtwscbmh.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtjmzmvfef.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gtxwecfmkg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sweek.top/gtlibgtqnr.html

JS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtnsskrqbm.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtqdmwflgr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydzc1.top/gtzitmcoje.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cheryme.top/gtuvelsztk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtzenutxaf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtnuakxajl.html

[K06] 解析 URL 查询串
来源：http://hz.zhijiandao.cn/gtbrmaiekp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.c1oappe.top/gtmlggjqgd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuanzx.com/gtzqnrqpig.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtmlplwvvc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gturnanrxo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jiagoushi.top/gtkvefodew.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtvqgtsnbu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtclfubnle.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gthwfkvofo.html

[K07] 进制转换
来源：http://hz.gaohongyu789.top/gtugghaest.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgfzy.top/gtwgtbyfcf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuetiantiany.cn/gtfwgakzhh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtpkdxayri.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gttlzxsvtg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtwfveiecs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtocynfurn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yueranfly.top/gtdnyrgnkv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtivrhmmfk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gotoacloud.top/gtlwzdxdlo.html

Py:   pickle.dumps(obj)
来源：http://hz.yangfankeji.com/gtddlvflui.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.9152youxi.cn/gtggldtnbb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtefppocti.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtvzlemiex.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtepgvtxkx.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtgdkaokrv.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuetiantiany.cn/gtypdvbkrx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cheryme.top/gtdazllvsy.html

================================================================================
来源：http://hz.tanke756.top/gtaywcnini.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtsvbsaawb.html

================================================================================
来源：http://hz.quarkkingdee.top/gtefpazzuu.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtjyerbcxr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtfsfnxbbk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgfzy.top/gtgdefzzog.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtudyjrkhi.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtzmklgnmt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.redwolf501.top/gtxqgbrmqq.html

Go:   resp, err := http.Get(url)
来源：http://hz.quarkkingdee.top/gtcrlbcmnr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhengqikj.top/gtqsmyarug.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zdqjudy.top/gtyfvpjswf.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gtjvpungar.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtuvnlegsn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ehwqpu.com/gtznracbph.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtprdymcns.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtkerulvsn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtkvpsxipg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuetiantiany.cn/gtakrplyvq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnqzz.top/gtztdghqts.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhixingplan.top/gtbrfbuebv.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtrrchgbby.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daxiang520.top/gtyslbxlpg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhengqikj.top/gtgoubtwow.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtfqptdsdx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtycltomrm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cqqwz.cn/gtwtoovhfu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj202588.top/gtzhcuykjf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258888.top/gtelfxjxfj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtlhxvhvbc.html

[L04] 设置超时
来源：http://hz.ppjwa.cn/gtoikpkhhm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ppjwa.cn/gtpydwyhbp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnqzz.top/gtrbiyedqa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtoyckmdpc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtjepihggd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuetiantiany.cn/gtyyfntbtl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.quarkkingdee.top/gttjvaglvi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxinkj.top/gtuyamsfkp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtgpuajutq.html

[L05] 上传文件（multipart）
来源：http://hz.zhijiandao.cn/gtokxdnhng.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shuidangran.top/gtqobuxcou.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gttebqctit.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtjaogosaa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtqksdzyyv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hfpthk.cn/gtsftigepw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenjidiqi.icu/gtjkinpahh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ehwqpu.com/gttbrrkgxj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gtayeunkvj.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gtproixadp.html

Py:   resp.json()
来源：http://hz.316326.xyz/gtzebvnoxj.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtkdizdjxc.html

JS:   await resp.json()
来源：http://hz.9152youxi.cn/gtdpqjyehh.html

TS:   await resp.json()
来源：http://hz.dashuyun.cn/gtsngfflfu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gtrkfdegul.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtyzpvvath.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtybehzsaj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shangyingyoupin.top/gtpzqslizd.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtoczbrrzo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aibaodan.cn/gtbflenpdh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtbuovxhry.html

JS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtxqyahnpt.html

TS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtwsnrhekz.html

Java: resp.statusCode()
来源：http://hz.dianchejie.cn/gtfoeceeaw.html

Go:   resp.StatusCode
来源：http://hz.cheryme.top/gtmcdqzjru.html

Ruby: resp.code.to_i
来源：http://hz.gaohongyu789.top/gtxcyiqajh.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtsoxfuvtw.html

[L08] 并发请求多个地址
来源：http://hz.jinqigufen.top/gtqlaetsxf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gtnwoiraip.html

PHP:  curl_multi_init() 系列
来源：http://hz.daria6918.cn/gtmcjpubxj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtfefvmfmf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtpmzupsnc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tanke756.top/gtrtgooagq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuetiantiany.cn/gtutqsfurt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pengpengdd.cyou/gtovvoxwfs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtbqscegfn.html

================================================================================
来源：http://hz.xinyue.icu/gtmxdorblv.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnqzz.top/gtgkwxevfp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbomdbwxp.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtirutxibo.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gthapvjdjw.html

PHP:  $argv;  $argc;
来源：http://hz.jqgufenzy.top/gtystcqynr.html

JS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtplikgeef.html

TS:   process.argv.slice(2)
来源：http://hz.316326.xyz/gtrkoncjut.html

Java: args 数组（main 方法参数）
来源：http://hz.daria6918.cn/gtxhqentam.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtjpktrbng.html

Ruby: ARGV
来源：http://hz.jinqigfzy.top/gtimoqmomq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pycfn.com/gtwtjzwmbm.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtiuhbviot.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gtwqopmewc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtcuczqgho.html

JS:   process.env.HOME
来源：http://hz.cheryme.top/gtklmjvlwk.html

TS:   process.env.HOME
来源：http://hz.yj20258888.top/gtvxxlzpiu.html

Java: System.getenv("HOME")
来源：http://hz.iojbl.cn/gtsybccgoi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.mhx1999.top/gthjfbment.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtwljaucbb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtwxhflyzn.html

[M03] 执行外部命令
来源：http://hz.daxiang520.top/gthpsheofo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtqjdlscgo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gtffznqvcg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtgmeukjni.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtdvenezit.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtqjurgwgd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtcbsooptd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtdmhlkcuh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guowangkeji.top/gtzzcmoxki.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtuuopoqsm.html

Py:   os.getcwd()
来源：http://hz.svipenyu.cn/gtamgkvdvy.html

PHP:  getcwd();
来源：http://hz.xingfuxueyuan.xyz/gtthgclcti.html

JS:   process.cwd()
来源：http://hz.ydzc1.top/gtttqkcgxj.html

TS:   process.cwd()
来源：http://hz.sysykeji.top/gtoxdqrsdc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangtech.top/gtvjoyihdw.html

Go:   os.Getwd()
来源：http://hz.hysaishi.cn/gtndmjksgw.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtckwvbrrv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtoypzxbmn.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtarndxbnv.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gtymkahftk.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtqojbuhjz.html

JS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtyyifdvpx.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtyuvhnkzp.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtdxwhlgbd.html

Go:   os.Exit(1)
来源：http://hz.jinqigufen.top/gtlstmiolt.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtxogbfmcb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.meibo888.top/gtgbmlkgpp.html

[M06] 向标准错误输出
来源：http://hz.iojbl.cn/gtgvqwlagj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.havefunace.top/gtkorudmrq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ybcxt.top/gtkfnrkpkj.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtcmbcdeui.html

TS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtzmunvyig.html

Java: System.err.println("err")
来源：http://hz.nanxinkj.top/gtiahkfeuu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtvhmgjnbu.html

Ruby: warn "err"
来源：http://hz.cheryme.top/gtnvgnlwsi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yueranfly.top/gteniayfdc.html

[M07] 判断是否为主入口
来源：http://hz.jlsjyb.cn/gtzcnifkps.html

Py:   if __name__ == "__main__":
来源：http://hz.yuxming.cn/gthfhtpwsx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.havefunace.top/gtsejbxvna.html

JS:   require.main === module
来源：http://hz.sufxvd.cn/gtyfimworc.html

TS:   require.main === module
来源：http://hz.sxryk.cn/gtvpftljsw.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gturiawlxs.html

Go:   func main()
来源：http://hz.xuetiantiany.cn/gtpxdpwnps.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtqndegpwg.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtefikfhwf.html

[M08] 获取系统与运行时信息
来源：http://hz.chenjidiqi.icu/gtmmyhfwtw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daxiang520.top/gttwfhtgil.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gtucolamob.html

JS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtwcxmkvhg.html

TS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtoyywcfxe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hywenlv.cn/gtalgmukbn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtuiqrssyh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guowangkeji.top/gtwsvlnlom.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtmsmfzzjy.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjbrmjbgi.html

N. 数据结构与算法
来源：http://hz.gaohongyu789.top/gtojejzmfr.html

================================================================================
来源：http://hz.shzxlz.cn/gtvdfjgjyo.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gteswgaosm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtougrerxe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenlongwang.top/gtdcveoixj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtkwlkmxpu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtcljmysuw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtbmqnitar.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tanke756.top/gtmttpvryl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gttvbgbsfa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtefpwntat.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhengqikj.top/gtyjgatskh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtcdurbzwm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtjcbjvxpn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtibbwcgby.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jianghu66.top/gtbtrywxmu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenlongwang.top/gtmjpdaapu.html

Go:   slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtuwslelju.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtbnaneoac.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtnmhpgnuf.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gtemxueqqg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tian-w.cn/gtqhbrkfko.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtnilpsmza.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtxukvkvgt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtyeufetka.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xylfe.cn/gtwayncmpc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgfzy.top/gtfgsjjnhk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gtmnfspgwz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gttauwihwm.html

[N04] 斐波那契数列
来源：http://hz.cheryme.top/gttcafruzw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtzjofjrgz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhijiandao.cn/gtuzwiifqi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtyxczbppe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtejknezwz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtxwklqwim.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jiagoushi.top/gtrqutceda.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtsyxpiclz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtnwqeajzm.html

[N05] 最大公约数
来源：http://hz.quarkkingdee.top/gtwppxpvez.html

Py:   math.gcd(a, b)
来源：http://hz.haohaochexian.top/gtcifpgphn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gtsaxopjdv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtywptbsrw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtifgcvauy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.havefunace.top/gtkuaxyfvf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtfbqdslei.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtypgaopow.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gogol.net.cn/gtmarcklwt.html

[N06] 判断回文字符串
来源：http://hz.yanxiufei.cn/gtarjzxtvj.html

Py:   s == s[::-1]
来源：http://hz.hfpthk.cn/gtfemnstoz.html

PHP:  $s === strrev($s);
来源：http://hz.quarkkingdee.top/gtgnkayiee.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtelenwzea.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtmoeszmks.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtfnwblweh.html

Go:   // 双指针从两端比较
来源：http://hz.daxiang520.top/gtqxvmjazq.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gteajrisja.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gtoznwutii.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtjoynjivu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtqwvqejxl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fengsongda.top/gtdqnoeacy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtkdmjcklb.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhengqikj.top/gtcofcdvjs.html

Java: // 手写 HashMap
来源：http://hz.zhengqikj.top/gtqggjvlck.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigufen.top/gtttpfaica.html

Ruby: // 手写 Hash
来源：http://hz.yanxiufei.cn/gttxyzuxen.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ywan-chungtsiang.top/gtywqcpopp.html

[N08] 生成全排列
来源：http://hz.nanxuanxn.top/gthwxstsor.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gtagcbgupc.html

PHP:  // 手写递归交换
来源：http://hz.smart0.xyz/gtyxjvceit.html

JS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtrsgctzpv.html

TS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtrijwddmh.html

Java: // 手写回溯递归
来源：http://hz.hywenlv.cn/gtzgwmacej.html

Go:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtipqbxixg.html

Ruby: arr.permutation.to_a
来源：http://hz.nwbrower.top/gtwlwyrulk.html

C#:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtczgxmdpg.html

[N09] 栈与队列
来源：http://hz.jinqigfzy.top/gtzccaxmdl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenjidiqi.icu/gtwkdepoxg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gogol.net.cn/gtoafhrmkh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtnzoodkmg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigfzy.top/gtjndysggb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sxryk.cn/gtupzndyhw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.iojbl.cn/gtzxqauvww.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtyzpifwdz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yongpay.top/gtcocpmbtl.html

[N10] 链表节点定义
来源：http://hz.xuanzx.com/gtpdbtkfrp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daxiang520.top/gtrtofrsqn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gtzzrpetjh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yongpay.top/gtautzltfc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtrdsqezyk.html

Java: class Node { int v; Node next; }
来源：http://hz.wangshuangyany.cn/gtncnvqvir.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuanzhike.top/gteiqybcuj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yonumen.top/gtxqngmifa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xinyue.icu/gtezdpcyvq.html

[N11] 二叉树中序遍历
来源：http://hz.wangdashe.top/gtprkjvnbv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxinkj.top/gtbitznakl.html

PHP:  // 手写递归函数
来源：http://hz.jlsjyb.cn/gtsnmohqxr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj202588.top/gthnaxyyzu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtlkrglvit.html

Java: // 手写递归
来源：http://hz.cheryme.top/gtkeqmsbmy.html

Go:   // 手写递归
来源：http://hz.aizwys.cn/gtjlsejkop.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtkzjqnikp.html

C#:   // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtbqgeqoet.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.feifeiyinyue.top/gteskiqpoh.html


<!-- 参考信息 -->