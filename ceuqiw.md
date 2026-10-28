代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jyoumei.cn/gtaatgzeeg.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtqozjxftx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtcxxkfvaw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtuurbaerm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtshjzsciw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtllbishmx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtsxfoyodt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtfphneqoj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtibqmibaz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtqamntyxc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.smart0.xyz/gtpwpiuvjp.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtteypikbw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtixboiyyz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtffnwjpmb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cucudq.cn/gtkgdamynm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aizwys.cn/gtynismjzj.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtwehjloev.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gtcszmgybx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtitejnekh.html

================================================================================
来源：http://hz.gotoacloud.top/gtfdlgbmur.html

L. 网络请求
来源：http://hz.zhongyouzk.top/gtuquxdiqn.html

================================================================================
来源：http://hz.52xcode.cn/gtnqajtkpq.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gttzmovhve.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yueranfly.top/gtfksednqu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aizwys.cn/gtcgqpqhhw.html

JS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtwdocnlux.html

TS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtbzbenybu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gtyiddaccz.html

Go:   resp, err := http.Get(url)
来源：http://hz.aizwys.cn/gtibiugijv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.c1oappe.top/gtdkgasraz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuxming.cn/gtfdwhytos.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtzqpwvbjq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangtech.top/gtrlftcmdk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtxjcqrbdv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtuiexynqq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtaubkqmaj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pengpengdd.cyou/gtneqfpils.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gtzpmaturg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hysaishi.cn/gtwocnjilc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangtech.top/gtjxknfdeb.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtmvsnvbyv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shanyushiyangtech.top/gtmwcyssmb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dianchejie.cn/gtiovvljzf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtwentsifs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtywggiaht.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gotoacloud.top/gtrzagvadq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtroawibwi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtvitueekm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtdtxpxget.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtfzityrsr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.bjfxy.top/gtjfnnphdv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtgdgzkkvz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtncrrtaab.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtyizpvauz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gtkkzlfksb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtygwsbotp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtxtewvcqu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxinkj.top/gtdqufbyup.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtphdckhgs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtzibwbkjk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guowangkeji.top/gthdfpfjyo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtaksrjppl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtstmldbiu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtkelaemtq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtxbadtodp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtxyewtgde.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtteztwelx.html

[L06] 解析响应为 JSON
来源：http://hz.sxryk.cn/gtjixrvqjy.html

Py:   resp.json()
来源：http://hz.jyoumei.cn/gtdledrgyg.html

PHP:  json_decode($body, true);
来源：http://hz.fzhhl.top/gtoiichlak.html

JS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtnsobqwvc.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtksjnjocm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nwbrower.top/gtyhrntzyb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gttiqwlsig.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtnriyvkds.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sufxvd.cn/gtcjauwone.html

[L07] 处理 HTTP 状态码
来源：http://hz.andypj.xyz/gtgkqrfuqx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jianghu66.top/gtjwpjjbbi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gtwgvyyaqn.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gthftqtqdd.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtupojkidz.html

Java: resp.statusCode()
来源：http://hz.zhixingplan.top/gtjmdbbezz.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtnsjgiwbh.html

Ruby: resp.code.to_i
来源：http://hz.tanke756.top/gtiephnghb.html

C#:   (int)resp.StatusCode
来源：http://hz.xziqi.cn/gtncyzqpil.html

[L08] 并发请求多个地址
来源：http://hz.yongpay.top/gtrkzxkduu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhengqikj.top/gtgjvxajim.html

PHP:  curl_multi_init() 系列
来源：http://hz.havefunace.top/gtgyzvtwlb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtsshtzcfa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtjdudkbym.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gtrkhmpdrv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtbzqwxbjm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cdnleiting.top/gtmpygkryt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.bjfxy.top/gtojzjreyk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtapxlaupj.html

M. 命令行 / 进程 / 环境
来源：http://hz.jianghu66.top/gtkposlivz.html

================================================================================
来源：http://hz.hywenlv.cn/gtbwejzvef.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtgjsotxyd.html

Py:   sys.argv[1:]
来源：http://hz.shuidangran.top/gtsqceumxs.html

PHP:  $argv;  $argc;
来源：http://hz.ywan-chungtsiang.top/gtanqfwijx.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtomiaflzz.html

TS:   process.argv.slice(2)
来源：http://hz.yueranfly.top/gtdnrojinu.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtrnkpkypw.html

Go:   os.Args[1:]
来源：http://hz.sufxvd.cn/gtahtzbkms.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtfpcvhjzj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gthcixxvdj.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtfrwrwond.html

Py:   os.environ.get("HOME")
来源：http://hz.fzhhl.top/gtpqopgrtt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtynnupzxv.html

JS:   process.env.HOME
来源：http://hz.yuanzhike.top/gthgyhmisf.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtkmdyprus.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtixhhmymg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hongshengwenyu.top/gttodlizuq.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gtsyhlzzxi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xinyue.icu/gtshculezz.html

[M03] 执行外部命令
来源：http://hz.kuanghao11.cn/gtqjnvbizt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtxwchdeef.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnxiangtu.top/gttjxrwmpw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtneojqcal.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtrorvlbxb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guannengcc.top/gtbygpzhru.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xziqi.cn/gtiivcmeiw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.andypj.xyz/gtmilqxhbz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gzhubu.top/gtzmjyomop.html

[M04] 获取当前工作目录
来源：http://hz.haohaochexian.top/gtfiedeqsl.html

Py:   os.getcwd()
来源：http://hz.haohaochexian.top/gtkdagorns.html

PHP:  getcwd();
来源：http://hz.sufxvd.cn/gthbqjiqhy.html

JS:   process.cwd()
来源：http://hz.iojbl.cn/gttueqjubd.html

TS:   process.cwd()
来源：http://hz.yuxming.cn/gtunozfeoz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hfpthk.cn/gtweuxazwz.html

Go:   os.Getwd()
来源：http://hz.fengsongda.top/gtzffkgpns.html

Ruby: Dir.pwd
来源：http://hz.fengsongda.top/gtsexlkkid.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pengpengdd.cyou/gtdqtylkwk.html

[M05] 设置退出码
来源：http://hz.yvedp.cn/gtczksuahh.html

Py:   sys.exit(1)
来源：http://hz.316326.xyz/gtplwfvxgc.html

PHP:  exit(1);
来源：http://hz.aizwys.cn/gtwjckormg.html

JS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtmbshrqfv.html

TS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtrueqftml.html

Java: System.exit(1)
来源：http://hz.mhx1999.top/gtwglhxcmz.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtqhaaqjez.html

Ruby: exit 1
来源：http://hz.zhiwuduotai.top/gtaldlzwqs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cashguo.top/gtmndtatsm.html

[M06] 向标准错误输出
来源：http://hz.jianghu66.top/gtfkiwntxp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gtkfbxvsuc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.iojbl.cn/gtweepomaz.html

JS:   console.error("err")
来源：http://hz.sufxvd.cn/gtxjqnszpd.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtwmsvyfxg.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtngroiryt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fzhhl.top/gttjkordli.html

Ruby: warn "err"
来源：http://hz.daxiang520.top/gtrqorowqp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinyuanbaomall.cn/gtfyzfkvbr.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtzgkeaqly.html

Py:   if __name__ == "__main__":
来源：http://hz.haohaochexian.top/gthujacdiu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.smart0.xyz/gtyggmovhs.html

JS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtfvrhnzvg.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtuxcvsusu.html

Java: public static void main(String[] args)
来源：http://hz.pengpengdd.cyou/gtbyxvfehs.html

Go:   func main()
来源：http://hz.fengsongda.top/gtmhsnrisf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.9152youxi.cn/gtpxhqtgqg.html

C#:   static void Main(string[] args)
来源：http://hz.guannengcc.top/gtqubriomr.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gtiyxjklhg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtfguazuvm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtkomzkvjk.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtfpgvwbwv.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtxfwzlmpj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangdashe.top/gtogvnxcsa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtarrzjspo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gtveknddqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aizwys.cn/gtwgqrkkca.html

================================================================================
来源：http://hz.mhx1999.top/gtmnpmdmub.html

N. 数据结构与算法
来源：http://hz.guannengcc.top/gtflqqdkpj.html

================================================================================
来源：http://hz.bjfxy.top/gtjsidzqrx.html

[N01] 二分查找（有序数组）
来源：http://hz.svipenyu.cn/gtxnhkcxqd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guannengcc.top/gtuufnxaot.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.9152youxi.cn/gttaasolae.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtjrgcuqmt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gttzojdxvd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cashguo.top/gtvdfdalef.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtwioloxbg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ivvv.top/gtumhqgyfd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtfhuquzjs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zycfv.cn/gtpanyhyrr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtjphmeirg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shangyingyoupin.top/gtusufxsdm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtuwhlvsnu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtyqiwooyt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangshuangyany.cn/gtveywntof.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtcsbobmhz.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtrjamrtar.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fzhhl.top/gttdycghvj.html

[N03] 快速排序（分治示例）
来源：http://hz.havefunace.top/gtxwfjpxsj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhijiandao.cn/gtocirxzua.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zycfv.cn/gtydfhelve.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtkoefashm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtzfzopvtf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtkictfrse.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtnasxmemr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhongyouzk.top/gtuzzyagxo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtawsvacfh.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtvnksqyxr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtmfevxqah.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.c1oappe.top/gtumnfktkf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtwpfwefog.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtmbbumcel.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtvuqmzkzu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yvedp.cn/gtzhdeifdr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtgrhjlszv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtmiwqchpj.html

[N05] 最大公约数
来源：http://hz.svipenyu.cn/gtsziwoqmm.html

Py:   math.gcd(a, b)
来源：http://hz.tanke756.top/gtfqjcbcwb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.mhx1999.top/gtdvwisclj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtazjoopcv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtxkmxbwpe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtqgaphjnx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtzgwpwhqv.html

Ruby: a.gcd(b)
来源：http://hz.andypj.xyz/gtzsrpfoxl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ehwqpu.com/gtzassyazj.html

[N06] 判断回文字符串
来源：http://hz.quarkkingdee.top/gtfdqvoqvz.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtslibvtys.html

PHP:  $s === strrev($s);
来源：http://hz.yvedp.cn/gtukzueuvw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtuqfcvzni.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtbvuptluw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hammf.cn/gtxuevdqmg.html

Go:   // 双指针从两端比较
来源：http://hz.ivvv.top/gteipukdai.html

Ruby: s == s.reverse
来源：http://hz.yuanzhike.top/gtzztiiypu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtjpqewmun.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gtfwdriflg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhiwuduotai.top/gtmmcfhfbo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.quarkkingdee.top/gtbdluvctx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ybcxt.top/gtangtqfpw.html

TS:   // 手写 Map<string, number>
来源：http://hz.feifeiyinyue.top/gtigqyqxbo.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtanmrgreu.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtrkamlsmq.html

Ruby: // 手写 Hash
来源：http://hz.andypj.xyz/gtyeymkfjz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtxtqyubxm.html

[N08] 生成全排列
来源：http://hz.ppjwa.cn/gtcgairtqd.html

Py:   itertools.permutations(arr)
来源：http://hz.jyoumei.cn/gtuyqvbtbw.html

PHP:  // 手写递归交换
来源：http://hz.yonumen.top/gtuusvhdod.html

JS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gthcmwrhxn.html

TS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtxznbxkfc.html

Java: // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtduwbhjib.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtrldislhv.html

Ruby: arr.permutation.to_a
来源：http://hz.gaohongyu789.top/gtzbrrnbwy.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtnpzuauwg.html

[N09] 栈与队列
来源：http://hz.daxiang520.top/gtftxreuah.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtctfwvtsj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangshuangyany.cn/gtnuwxciat.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ydjk.org.cn/gtjpeobxlq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhijiandao.cn/gtydjzbdds.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gtvxcfnkbi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tanke756.top/gtghddtdwr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yongpay.top/gtklqhgyuf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tianlin.xyz/gtxpnyvxtl.html

[N10] 链表节点定义
来源：http://hz.ydjk.org.cn/gtyhjmtstr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtwevxllxf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinghuilouyu.cn/gtpqccsyuz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhongyouzk.top/gtviodnzuw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.quarkkingdee.top/gtbasrxqrl.html

Java: class Node { int v; Node next; }
来源：http://hz.yuanzhike.top/gtvuciarec.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aibaodan.cn/gtupoedmdy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xziqi.cn/gtadhbjzpe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnxiangtu.top/gtgznjgtvf.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtpvotsnfx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.iojbl.cn/gtieekvxhz.html

PHP:  // 手写递归函数
来源：http://hz.ybcxt.top/gtqjqmplbv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtnnsphgap.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gthxbgwcyr.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtipfvcpty.html

Go:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtmstwfwke.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.kuanghao11.cn/gtkwhbckyx.html

C#:   // 手写递归
来源：http://hz.hammf.cn/gtkvgmccov.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtxeocifym.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yongpay.top/gtsvrroqyc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigufen.top/gtqobnnuvj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.52xcode.cn/gtwixmkxph.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtveackvgh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtabfzocfa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gttuferdct.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yangfankeji.com/gttolzbrzo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtqrhatkzm.html

================================================================================
来源：http://hz.9152youxi.cn/gtilkakvcp.html

O. 并发与异步
来源：http://hz.havefunace.top/gtfwhebdny.html

================================================================================
来源：http://hz.hnqzz.top/gtkvusfnma.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtltykvptw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hammf.cn/gtdnyyjlbh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.andypj.xyz/gtyhurqvbm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtliqwaajl.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtklbydplt.html

Java: new Thread(() -> f()).start()
来源：http://hz.9152youxi.cn/gtkmykpavo.html

Go:   go f()
来源：http://hz.pengpengdd.cyou/gtmvfcvudg.html

Ruby: Thread.new { f }
来源：http://hz.yueranfly.top/gtyztvcmem.html

C#:   Task.Run(() => F());
来源：http://hz.gotoacloud.top/gtlgkthnfd.html

[O02] 使用线程池
来源：http://hz.yueranfly.top/gtrwmxpvgl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pengpengdd.cyou/gtkddxwzmj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydjk.org.cn/gttkfeihjw.html

JS:   // worker_threads 线程池
来源：http://hz.ywan-chungtsiang.top/gtiwvovtmq.html

TS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtanwzzkds.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtuxbbnifj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydjk.org.cn/gtlairntlh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.dianchejie.cn/gtdanciqfl.html


<!-- 参考信息 -->