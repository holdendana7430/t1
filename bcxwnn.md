代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtiaiedyhf.html

TS:   s.split(",")
来源：http://hz.birdmap.top/gtqnkxgurb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnqzz.top/gtnevtfmym.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtupkogszy.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gtmjavcsko.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtanrhkrrd.html

[E08] 数组按分隔符合并
来源：http://hz.chenlongwang.top/gtklthgtlo.html

Py:   ",".join(items)
来源：http://hz.xuanzx.com/gtmpdcgxjc.html

PHP:  implode(",", $items);
来源：http://hz.jlsjyb.cn/gtynvsfrdj.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gthbiyufwa.html

TS:   items.join(",")
来源：http://hz.ydzc1.top/gtzcjklafu.html

Java: String.join(",", items)
来源：http://hz.c1oappe.top/gteltlvvpp.html

Go:   strings.Join(items, ",")
来源：http://hz.zhongyouzk.top/gtobobltfg.html

Ruby: items.join(",")
来源：http://hz.snrcjt.cn/gtvbyaztyz.html

C#:   string.Join(",", items)
来源：http://hz.xinyue.icu/gtwtjzmfdu.html

[E09] 去除所有空白字符
来源：http://hz.xuanzx.com/gtxksmvuwe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ppjwa.cn/gtfygpwnwn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtgxgguamr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtdnnvytsf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yvedp.cn/gtwambxwaq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.vqdsnc.cn/gtlrxnroyg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydjk.org.cn/gtvvxhjdaj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hfpthk.cn/gtjwzrthmi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cqqwz.cn/gtzixxwptg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.quarkkingdee.top/gtypiqbhsg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnxiangtu.top/gtsehzjvcn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zycfv.cn/gtebcvwuex.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtyxbwotfh.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtwfwecjpc.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gtgiavvtrm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yangfankeji.com/gtgkcfxxoc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.52xcode.cn/gtjzlwpxkl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgufenzy.top/gtmcehhziy.html

[E11] 反转字符串
来源：http://hz.bjfxy.top/gtmkenilis.html

Py:   s[::-1]
来源：http://hz.jyoumei.cn/gtiehchopm.html

PHP:  strrev($s);
来源：http://hz.xylfe.cn/gtkayaijgz.html

JS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gthnzcfflt.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtkiaomque.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.c1oappe.top/gtdlugjswc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xylfe.cn/gtzhugugih.html

Ruby: s.reverse
来源：http://hz.sufxvd.cn/gtafmugizn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtiqrwucee.html

[E12] 统计某字符出现次数
来源：http://hz.snrcjt.cn/gtzsbsqusg.html

Py:   s.count("a")
来源：http://hz.tianlin.xyz/gthsmygdqq.html

PHP:  substr_count($s, "a");
来源：http://hz.jinyuanbaomall.cn/gtuytqxkfw.html

JS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtfcsfnfui.html

TS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtlbtbxwsl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sweek.top/gtogetkidj.html

Go:   strings.Count(s, "a")
来源：http://hz.xziqi.cn/gtzopzedju.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtirofzecb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhixingplan.top/gtldovcldp.html

[E13] 逐字符遍历
来源：http://hz.yuanzhike.top/gtelrocfmg.html

Py:   for ch in s: print(ch)
来源：http://hz.feifeiyinyue.top/gtcdtunuke.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnxiangtu.top/gtstxecytf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gtyfubievc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtcxpvxddj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cheryme.top/gthjodcywk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sufxvd.cn/gtwjkrzjot.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.0kj1m.cn/gtgkcdzhoh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.haohaochexian.top/gtbdbmqbbt.html

[E14] URL 编码与 Base64
来源：http://hz.zhiwuduotai.top/gtsjumppyh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuetiantiany.cn/gtmuooenlx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sysykeji.top/gtkrqaruwc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pengpengdd.cyou/gtaiwohvhk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtvsaeieou.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yangfankeji.com/gtfnrkqerl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jiagoushi.top/gtmrbnkgoc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dianchejie.cn/gtjnqorzdy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sweek.top/gtxfvxfywr.html

[E15] HTML 转义 / 反转义
来源：http://hz.cdnleiting.top/gtmqkdoggo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.redwolf501.top/gtrqoovdjp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ehwqpu.com/gtesdzkqss.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangkeji.top/gtiqecmvyc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtpmkwhaws.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydzc1.top/gtmvlocbuy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangdashe.top/gtgayplitq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigfzy.top/gtnmjrmtdz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhijiandao.cn/gtsxhkivfp.html

[E16] 数字千分位
来源：http://hz.meibo888.top/gtrlvzuncb.html

Py:   f"{1234567:,}"
来源：http://hz.iojbl.cn/gtmhtirsow.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gtbyisirpc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gteryedmjn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtxgueqljn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sweek.top/gthjdinsae.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gtfshpfwkw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gogol.net.cn/gtmjbolxec.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gtjlticuhd.html

[E17] 首字母大写
来源：http://hz.52xcode.cn/gthimfewdc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.havefunace.top/gtgnosgbjv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gtxrykkrlz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gthotvzffo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gtnfcvzjdm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gtxshkkpyk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.vqdsnc.cn/gtdbtqnuxk.html

Ruby: s.capitalize
来源：http://hz.yj20258888.top/gttwikbnzk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtmgcljhpg.html

[E18] 模板占位符替换
来源：http://hz.aizwys.cn/gtrcttqheu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ehwqpu.com/gtlalbaskd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhijiandao.cn/gtmgtaprth.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtolbkjsjl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtulhtxvwl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtxkzxdljq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gogol.net.cn/gtwpezzqlo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yongpay.top/gtuxdswwac.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.redwolf501.top/gtdfngwyen.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtbzssgroq.html

Py:   s.splitlines()
来源：http://hz.gogol.net.cn/gtrwmcooyr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangtech.top/gtwlxfqpoo.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtylynqpqo.html

TS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtbvxgqrbu.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtzbaygwnf.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gtpxtdqdfu.html

Ruby: s.lines
来源：http://hz.jinqigfzy.top/gtktlatipq.html

C#:   s.Split('\n')
来源：http://hz.jinyuanbaomall.cn/gtjsqhgwhh.html

[E20] 判断字符串是否为空
来源：http://hz.316326.xyz/gtcxcavcwm.html

Py:   if not s:
来源：http://hz.0kj1m.cn/gtrhcbhtte.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guannengcc.top/gtyoptacas.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenlongwang.top/gtqhooxbmv.html

TS:   if (s === "") {}
来源：http://hz.smart0.xyz/gtorvhqcui.html

Java: if (s.isEmpty()) {}
来源：http://hz.yvedp.cn/gtfsswovru.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtlcdlafcn.html

Ruby: if s.empty?
来源：http://hz.wangshuangyany.cn/gtthqbicvp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.wangshuangyany.cn/gttbgffkxm.html

[E21] 超长截断加省略号
来源：http://hz.hfpthk.cn/gthswehqvb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhengqikj.top/gtfvlydzmx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gogol.net.cn/gtrvcsutef.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtqqmgebor.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtbfjxckrw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtvqinzmml.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gotoacloud.top/gtrpxppqee.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydjk.org.cn/gthqztlghe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtvcpwajhl.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtnnwuixwg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnxiangtu.top/gtbexlnfox.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtljllqmey.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtmwuyaanv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtrpeeqlba.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtushnsitr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.andypj.xyz/gtvoljeqla.html

Ruby: s.bytesize;  s.length
来源：http://hz.sxryk.cn/gtuzcbvaha.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258.top/gthsdzgkzq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnfziprre.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gttqxtteum.html

================================================================================
来源：http://hz.gaohongyu789.top/gtwwzcoctz.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtqzunmgxv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hywenlv.cn/gtpxznlius.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yangfankeji.com/gtlerpcpwk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jyoumei.cn/gtbasczjeb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gtmplaafuy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtalhmnzlq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ydzc1.top/gtmorpffgb.html

Ruby: File.read("a.txt")
来源：http://hz.tianlin.xyz/gtmitjjtjs.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.quarkkingdee.top/gthkbwtydn.html

[F02] 逐行读取文件
来源：http://hz.316326.xyz/gtphxjgxck.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gotoacloud.top/gtxzmfojrp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.andypj.xyz/gtmnyrpgdu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtvpftzgux.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtpgtimvaa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtyxngojiv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtbaqkfupy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gtgxyhktok.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtrnxktqft.html

[F03] 写入文件（覆盖）
来源：http://hz.xziqi.cn/gtktizfyar.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sweek.top/gtfufxbijo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtavmixupt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtcqqxdzdr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtnutghmxx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgufenzy.top/gtgyukvxib.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.iojbl.cn/gtghefhynr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.feifeiyinyue.top/gtkzuiqxpm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuanzx.com/gtxblpvvux.html

[F04] 追加写入文件
来源：http://hz.fzhhl.top/gtmrskyofj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daria6918.cn/gtuqgyudcp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuetiantiany.cn/gtahrspemm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtxhnnmpwd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sweek.top/gtyjbkxpbp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gthpcuquje.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtlellgrep.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gteovjwhzp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gzhubu.top/gtygikjlbr.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtvqjetbbu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yongpay.top/gtldibynru.html

PHP:  file_exists("a.txt");
来源：http://hz.hywenlv.cn/gtezpntwgz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtdyrcwcsb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtupxyqagm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtvadikoch.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigfzy.top/gtwjfhboxz.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtbaphojti.html

C#:   File.Exists("a.txt")
来源：http://hz.xuetiantiany.cn/gtwtunlplf.html

[F06] 删除文件
来源：http://hz.jqgfzy.top/gtotiiwbqm.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtifcncvbi.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gttfafrtyw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtbxcdxivo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtclwwzwew.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtkwaztrhz.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtsffpwcwa.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtnqvpgxmi.html

C#:   File.Delete("a.txt");
来源：http://hz.dashuyun.cn/gtvwgxexjv.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtopwghoer.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ehwqpu.com/gtjikjmpdi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhaomingkeji.xyz/gthasonxdn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gtxjnfepus.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtbkiyjajd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtxidkeuki.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtacxlugfd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtxlpnwvdx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtqyevixou.html

[F08] 遍历目录
来源：http://hz.snrcjt.cn/gtgjnzxupr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtpvzftlkc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.kuanghao11.cn/gtiymmxeal.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtadqokueb.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gteporrnes.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gthzdwgcln.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shzxlz.cn/gtfwqqtsml.html

Ruby: Dir.children("dir")
来源：http://hz.pycfn.com/gtgnnyzqop.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pycfn.com/gtxjgcbity.html

[F09] 获取文件大小
来源：http://hz.shzxlz.cn/gtlojofbyv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gtqveygzry.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtxccdceyq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtpkkhitfc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gttwsdazlw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtoonvhapy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtdtkjswgm.html

Ruby: File.size("a.txt")
来源：http://hz.redwolf501.top/gtjnjhyoau.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yanxiufei.cn/gtkfqqezsk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hammf.cn/gthzrjknro.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtoemuagoc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gogol.net.cn/gtiheyqjwm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gttbjvlwvc.html

TS:   path.extname("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtfxvvhofy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigfzy.top/gttwqhazux.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yangfankeji.com/gtlxzpkkse.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtrlggwmbl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.meibo888.top/gtajqqbmgb.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtotjpbkuf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtexgqwfur.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigufen.top/gterdntnxa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gttreiinoa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtswziirls.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxinkj.top/gtuoaaocxp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangshuangyany.cn/gtbqblvwyy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.316326.xyz/gttqcqbxaa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yvedp.cn/gtvupbbmxj.html

[F12] CSV 读写
来源：http://hz.c1oappe.top/gtchzisorq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gtecjifhtx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenlongwang.top/gtlsfuedcg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hysaishi.cn/gtsnznpmnd.html

TS:   // 同上
来源：http://hz.smart0.xyz/gteyeyfevn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuetiantiany.cn/gtrfqomvqr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hammf.cn/gtohevgxfl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pycfn.com/gteboytpmp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.iojbl.cn/gtpfedsjdi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtgwmlcbxl.html

G. 面向对象
来源：http://hz.yj202588.top/gtdlnkywjv.html

================================================================================
来源：http://hz.chenlongwang.top/gtkytxmekn.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtajjxqeom.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gthinjywhi.html

PHP:  class User {}
来源：http://hz.dashuyun.cn/gtqfruijae.html

JS:   class User {}
来源：http://hz.sxryk.cn/gtsoxhlmus.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gtdpolepyt.html

Java: class User {}
来源：http://hz.wangdashe.top/gtjmcyaghs.html

Go:   type User struct { Name string }
来源：http://hz.cheryme.top/gtiunmtiym.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtlgrnqnnj.html

C#:   class User {}
来源：http://hz.cucudq.cn/gthvrnzvkl.html

[G02] 构造函数
来源：http://hz.hnxiangtu.top/gtktnayyxj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtdhcjbelb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gtihfpzhck.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtnvqivgxw.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtoeanuuon.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtevfsptsq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gotoacloud.top/gtruegqsdc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtuhndufqw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtlehpzplh.html

[G03] 实例属性
来源：http://hz.yongpay.top/gtaswvualo.html

Py:   self.name = "x"
来源：http://hz.tian-w.cn/gtbvubevpu.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gtwnwczjuf.html

JS:   this.name = "x";
来源：http://hz.jinqigufen.top/gtfrfpuxik.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtixfzrnbk.html

Java: private String name;
来源：http://hz.yonumen.top/gtmvosaujk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xuetiantiany.cn/gtbzybrnce.html

Ruby: @name = "x"
来源：http://hz.kuanghao11.cn/gtiakotfgg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtuxyxcsan.html

[G04] 定义方法
来源：http://hz.shanyushiyangkeji.top/gtfycjoqlb.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtrxqqyvyw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtibfpgaya.html

JS:   greet() { return this.name; }
来源：http://hz.c1oappe.top/gtkiozjxsy.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtebuejsrs.html

Java: String greet() { return name; }
来源：http://hz.dashuyun.cn/gtkmvgwxcw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtsyodgygk.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtuwrquwba.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtidcgrbqp.html

[G05] 继承
来源：http://hz.yj202588.top/gtxntdrycg.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gtuhemefld.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gthprcamew.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtvfqgrqft.html

TS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtcwkkcwep.html

Java: class Admin extends User {}
来源：http://hz.xinyue.icu/gtagjoasrm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtrsmcsnyr.html

Ruby: class Admin < User; end
来源：http://hz.9152youxi.cn/gtncirqdjt.html

C#:   class Admin : User {}
来源：http://hz.c1oappe.top/gtujugheaf.html


<!-- 参考信息 -->