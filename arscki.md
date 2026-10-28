代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gtjedvytjo.html

[K07] 进制转换
来源：http://hz.zhixingplan.top/gtuyzvrmnc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jyoumei.cn/gtaufqhjsv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sweek.top/gtyvuvqbgm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtnumxgelk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtdzmejdwz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtlttbzobp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jiagoushi.top/gtzzryvrtx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yueranfly.top/gtaklllkzh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtqpjohgiq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgufenzy.top/gtzgmhpskz.html

Py:   pickle.dumps(obj)
来源：http://hz.zycfv.cn/gtqmrnmnme.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtrilsrqwi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtkpdantka.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtpkdykokh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenzaomai.com/gtihfetrbe.html

Go:   encoding/gob
来源：http://hz.cashguo.top/gtfxiiwbgc.html

Ruby: Marshal.dump(obj)
来源：http://hz.vqdsnc.cn/gttvnbyhfe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daria6918.cn/gtvyksuuvl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthkifuows.html

L. 网络请求
来源：http://hz.sufxvd.cn/gtucssaopo.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdkuvngag.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtuwxconlg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gaohongyu789.top/gtlgbqqyft.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gtojrxmcxg.html

JS:   await fetch(url)
来源：http://hz.cashguo.top/gtsmkkpadx.html

TS:   await fetch(url)
来源：http://hz.sweek.top/gthmoayaiy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yongpay.top/gtooylktfh.html

Go:   resp, err := http.Get(url)
来源：http://hz.xinyue.icu/gtejudrald.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.iojbl.cn/gtqkvgtrte.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgfzy.top/gtqfmdsban.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtbfcnokko.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fengsongda.top/gtzxrpclag.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pycfn.com/gtaqzcbsvt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtgzcqevpw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtpffmhufv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtyszrluua.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.svipenyu.cn/gtxraajsxr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dashuyun.cn/gttnclwrhi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtjgvwzmzf.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gtjkwhuymk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.haohaochexian.top/gtomedogvo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yvedp.cn/gtntgkwgbk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtnaqcyzkd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtuypyiply.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gttntewkxy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.c1oappe.top/gtvppzwzrg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtaiuagcao.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtmoizbphi.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtgdhcxmey.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtkyqivmfb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.smart0.xyz/gtxuqczuoe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtagrnypjo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtxmavadwp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jiagoushi.top/gttpekgtqz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yvedp.cn/gtflshkjtt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.andypj.xyz/gtvufhuuzt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtmsetknix.html

[L05] 上传文件（multipart）
来源：http://hz.iojbl.cn/gtbbqvhtgq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhaomingkeji.xyz/gtdodfpzvh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ybcxt.top/gtfaxbefpy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtxeqquuny.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtnbhkbqar.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtefbcoxpl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuanzx.com/gtuawavzqj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtxzceqqsi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ywan-chungtsiang.top/gtboijpkxv.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gtsxwtyogj.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtvyxiivyg.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangkeji.top/gtysggiipe.html

JS:   await resp.json()
来源：http://hz.shzxlz.cn/gtpfstpuqr.html

TS:   await resp.json()
来源：http://hz.52xcode.cn/gtkkjkvapb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.kuanghao11.cn/gtlokezgkc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jianghu66.top/gttofduqjh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ybcxt.top/gtnzficqux.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtshcgmdff.html

[L07] 处理 HTTP 状态码
来源：http://hz.quarkkingdee.top/gtqmbymxlg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhongyouzk.top/gtpaxxwsfh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinghuilouyu.cn/gtvvpzlygh.html

JS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtqdruejvg.html

TS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtiwxjqlxs.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtqjatiipp.html

Go:   resp.StatusCode
来源：http://hz.yvedp.cn/gtmbznftfi.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gttqzlfcbr.html

C#:   (int)resp.StatusCode
来源：http://hz.nwbrower.top/gtofsunrcb.html

[L08] 并发请求多个地址
来源：http://hz.daxiang520.top/gtevkuxsgb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hfpthk.cn/gtljzpbkwx.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtbchmrxya.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtvteecouz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtorhhsqkq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtrillbphl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.svipenyu.cn/gtdmdlehnn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.0kj1m.cn/gtkknfkphq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cucudq.cn/gtfnmhiigq.html

================================================================================
来源：http://hz.meibo888.top/gtdlnlssie.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtxdzxanul.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtddbfvfec.html

[M01] 读取命令行参数
来源：http://hz.yvedp.cn/gtxwomgiyd.html

Py:   sys.argv[1:]
来源：http://hz.sufxvd.cn/gtprltfzib.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gtrrwwlbpm.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtaczhqeux.html

TS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtpxlkeylm.html

Java: args 数组（main 方法参数）
来源：http://hz.aizwys.cn/gtzbkywlzk.html

Go:   os.Args[1:]
来源：http://hz.jiagoushi.top/gtxasjvkcv.html

Ruby: ARGV
来源：http://hz.zycfv.cn/gtuxsfcilz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gogol.net.cn/gtwhrlfzlb.html

[M02] 读取环境变量
来源：http://hz.yvedp.cn/gtcanswzid.html

Py:   os.environ.get("HOME")
来源：http://hz.dashuyun.cn/gtwpehtdky.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gtckxxpgfg.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtxaqdvjkf.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtexxrzvfb.html

Java: System.getenv("HOME")
来源：http://hz.iojbl.cn/gtjmribzmx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj202588.top/gtfckfpxzb.html

Ruby: ENV["HOME"]
来源：http://hz.ybcxt.top/gtnucptpgb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gogol.net.cn/gtevzqzbmr.html

[M03] 执行外部命令
来源：http://hz.ydjk.org.cn/gtrhwwvmnp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtityfbgiv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnqzz.top/gtyxxvhtan.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtinemptns.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtzaogixtb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.redwolf501.top/gtrimprspd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtsnnuvhko.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pycfn.com/gtgpoucuhw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtkmefuwau.html

[M04] 获取当前工作目录
来源：http://hz.zhixingplan.top/gtkrujkwes.html

Py:   os.getcwd()
来源：http://hz.bjfxy.top/gtmwccflmn.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtppglrhui.html

JS:   process.cwd()
来源：http://hz.yuxming.cn/gtylkahlxk.html

TS:   process.cwd()
来源：http://hz.daxiang520.top/gthyvzkwcj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.andypj.xyz/gtbvfomeqp.html

Go:   os.Getwd()
来源：http://hz.guowangkeji.top/gteinhkhkd.html

Ruby: Dir.pwd
来源：http://hz.cucudq.cn/gtomojtqgi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhaomingkeji.xyz/gtfusgekgw.html

[M05] 设置退出码
来源：http://hz.feifeiyinyue.top/gtwtvvlhdo.html

Py:   sys.exit(1)
来源：http://hz.snrcjt.cn/gtlwbhimql.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtlwzuitmz.html

JS:   process.exit(1)
来源：http://hz.yvedp.cn/gtaexweumb.html

TS:   process.exit(1)
来源：http://hz.yj202588.top/gtxggmuchv.html

Java: System.exit(1)
来源：http://hz.sxryk.cn/gtmlvlqful.html

Go:   os.Exit(1)
来源：http://hz.jqgufenzy.top/gtwgrxrahj.html

Ruby: exit 1
来源：http://hz.quarkkingdee.top/gtbxskaepb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigfzy.top/gthuwtppok.html

[M06] 向标准错误输出
来源：http://hz.9152youxi.cn/gtwoeupzbr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtcoaqfnzg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtnwwsharr.html

JS:   console.error("err")
来源：http://hz.dianchejie.cn/gtezhkhciw.html

TS:   console.error("err")
来源：http://hz.c1oappe.top/gtlfdhbjqk.html

Java: System.err.println("err")
来源：http://hz.zdqjudy.top/gtdohrakjd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtxpmqutzj.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gtygrtmrkl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenzaomai.com/gtyvzxuqxd.html

[M07] 判断是否为主入口
来源：http://hz.jqgfzy.top/gttrghaohf.html

Py:   if __name__ == "__main__":
来源：http://hz.wangshuangyany.cn/gtjxrivbxb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtiziqxuvd.html

JS:   require.main === module
来源：http://hz.cdnleiting.top/gtvyxxkbla.html

TS:   require.main === module
来源：http://hz.ivvv.top/gtlwvjgims.html

Java: public static void main(String[] args)
来源：http://hz.daxiang520.top/gtbichzyvv.html

Go:   func main()
来源：http://hz.aibaodan.cn/gtwlfxgkaj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtcoxhcsrd.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtxocemfmq.html

[M08] 获取系统与运行时信息
来源：http://hz.ybcxt.top/gtmvaolswd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.c1oappe.top/gtahcfvliw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtlijxfebq.html

JS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtkjpxzkkd.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtjajsnjeo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtrcrkmmmj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.feifeiyinyue.top/gtukjvqhwx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.316326.xyz/gtvzdkmozf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtnbkfyfrz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvieeoany.html

N. 数据结构与算法
来源：http://hz.xingfuxueyuan.xyz/gtjozvntai.html

================================================================================
来源：http://hz.jlsjyb.cn/gtoohmwfhz.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtyndctrrk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtuyoxisar.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guowangkeji.top/gtibjzwlio.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuanzhike.top/gtdjhoibcl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtrclmbfad.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtzncqfsin.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhengqikj.top/gtrdjpngdd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tianlin.xyz/gtvvhbehqz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ybcxt.top/gtbdbnqmhj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangtech.top/gtoanldkjn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtigodjola.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtmpxsraud.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtfpdrpjrs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtrdwycnzn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jlsjyb.cn/gtednfxkqj.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtpfvwodfu.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtluamfher.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtyukhflsi.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258888.top/gtwiedftxc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cashguo.top/gtxfwslvky.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jyoumei.cn/gtvabbicfu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtnuuzknvp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtpdhekide.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ydjk.org.cn/gtqkyytklm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jlsjyb.cn/gtajoktkkb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cheryme.top/gtggbdcsmv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sufxvd.cn/gtbladaqvz.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtjzvteoax.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtydgasrfz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gotoacloud.top/gtvsrplxoj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtqprzqyfq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gthjjtqicv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gttbntjwzg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtbtqjqjpa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtunaetveo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yvedp.cn/gtmemgjibk.html

[N05] 最大公约数
来源：http://hz.zhongyouzk.top/gtaxwuqhpr.html

Py:   math.gcd(a, b)
来源：http://hz.zhongyouzk.top/gtiomlimsw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hongshengwenyu.top/gtafrepoax.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtfmhqeexo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtzjmkziis.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gogol.net.cn/gtnmhjcfbh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuanzhike.top/gtyielxpzk.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gtfgkvuprz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yangfankeji.com/gtnmiircdf.html

[N06] 判断回文字符串
来源：http://hz.zhengqikj.top/gtbkrysjjb.html

Py:   s == s[::-1]
来源：http://hz.yvedp.cn/gtdctekwgt.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtaclhferk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtgumoivrk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gthftqvnfj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtrbmtwuti.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtwnbicotk.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtuwmgjzwn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtawjzelzd.html

[N07] 两数之和（返回下标）
来源：http://hz.guowangkeji.top/gtfzszqdrt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xziqi.cn/gthbaagpfg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtwqmxqaet.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.daria6918.cn/gtgecjhesc.html

TS:   // 手写 Map<string, number>
来源：http://hz.yanxiufei.cn/gtsfjahczv.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtdmprhdnz.html

Go:   // 手写 map[int]int
来源：http://hz.snrcjt.cn/gtfaqjektd.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gttjrzprxd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhengqikj.top/gteslycvhn.html

[N08] 生成全排列
来源：http://hz.snrcjt.cn/gtnnebrqfy.html

Py:   itertools.permutations(arr)
来源：http://hz.fengsongda.top/gtslcqtdtw.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangtech.top/gtygwbisno.html

JS:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtidbqaskg.html

TS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtdozhblwt.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtfgcrntwb.html

Go:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtjxowrgjp.html

Ruby: arr.permutation.to_a
来源：http://hz.daria6918.cn/gtzcouxunx.html

C#:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gthytfwzko.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gthpjrigtz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yonumen.top/gtqqsvvhwg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nwbrower.top/gtgyakxcsx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigufen.top/gtcnpajztb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nwbrower.top/gtrcqyaovs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sufxvd.cn/gtmbdecpnv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gttvapfjhc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtnllyfqbt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.bjfxy.top/gtjtpxzrer.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangkeji.top/gttanrzhkl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtngqwubpj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.vqdsnc.cn/gtpgmifkfy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.dianchejie.cn/gtzsggltgj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigufen.top/gtrjzeisuq.html

Java: class Node { int v; Node next; }
来源：http://hz.hammf.cn/gtfqjwifag.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hongshengwenyu.top/gtdeihyqoy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.havefunace.top/gtqjnbgpsm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtpgrzxhbs.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gttjxqbnna.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sysykeji.top/gtcdkzxjil.html

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gtbklddtre.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtiasxbhls.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtlpwrhqft.html

Java: // 手写递归
来源：http://hz.chenzaomai.com/gtdstgupvv.html

Go:   // 手写递归
来源：http://hz.sxryk.cn/gtvljkywsw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gaohongyu789.top/gtsdaagjig.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtotsmazmf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gogol.net.cn/gtqarvnkil.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtfwutxqki.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtaxnciqxv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtuwxgzukb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtmqxymjnq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhijiandao.cn/gtwpksqhej.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtvsovozsw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gtevpygiqj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtkfkdmbyd.html

================================================================================
来源：http://hz.jyoumei.cn/gtdrnfjwvd.html

O. 并发与异步
来源：http://hz.cqqwz.cn/gtyovmyuau.html

================================================================================
来源：http://hz.0kj1m.cn/gtsyyelqot.html

[O01] 启动一个线程
来源：http://hz.nanxinkj.top/gtozvdmbhi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gogol.net.cn/gtfkrarscg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtculxxnkq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnqzz.top/gtkdyvyyby.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtxuxeirkk.html

Java: new Thread(() -> f()).start()
来源：http://hz.zycfv.cn/gtzqkzbblm.html

Go:   go f()
来源：http://hz.52xcode.cn/gtvapgnjqf.html

Ruby: Thread.new { f }
来源：http://hz.zycfv.cn/gtqvamdbfg.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gteayfylva.html

[O02] 使用线程池
来源：http://hz.daria6918.cn/gthumizgwj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hysaishi.cn/gtjkavjccl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shzxlz.cn/gtikoswayk.html

JS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtvxrtewce.html

TS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtabbjacpp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gteampcocf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yangfankeji.com/gtnevmztzm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.316326.xyz/gttaenkdwg.html


<!-- 参考信息 -->