代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtoumjgbtk.html

C#:   s.Substring(1, 3)
来源：http://hz.hywenlv.cn/gtsqgyxjfp.html

[E04] 查找子串位置
来源：http://hz.zhiwuduotai.top/gtiuxzwfqv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydjk.org.cn/gtfmddvsrr.html

PHP:  strpos($s, "x");
来源：http://hz.feifeiyinyue.top/gtrrhlasna.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cqqwz.cn/gtruhlnhil.html

TS:   s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtjuqlnffz.html

Java: s.indexOf("x")
来源：http://hz.yuanzhike.top/gtbrmhinvq.html

Go:   strings.Index(s, "x")
来源：http://hz.316326.xyz/gtrfltnjcx.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtudnhrrxr.html

C#:   s.IndexOf("x")
来源：http://hz.xylfe.cn/gtjbtywjgr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cheryme.top/gtqlmcjkjh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgufenzy.top/gtdholrpuq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dianchejie.cn/gtltqwzzvz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtaxetvoii.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ywan-chungtsiang.top/gtehjiuwdo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtkjtscpve.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jiagoushi.top/gtcejpqkvr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.9152youxi.cn/gtkqvuwill.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sysykeji.top/gtwnpvuwub.html

[E06] 替换子串
来源：http://hz.tianlin.xyz/gtzjljbbwl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenzaomai.com/gtlyrgqwcf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.9152youxi.cn/gtahmrdcwj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtptpzdfmi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtgafgavch.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gturyqazfn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.vqdsnc.cn/gtvfmvjcyb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ppjwa.cn/gtqjylqukp.html

C#:   s.Replace("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtyuyervdv.html

[E07] 按分隔符拆分
来源：http://hz.ydjk.org.cn/gtwigtjptf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nanxinkj.top/gtjwmtknbg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhaomingkeji.xyz/gtjaojgpqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cucudq.cn/gthrxtkgjn.html

TS:   s.split(",")
来源：http://hz.cdnleiting.top/gtgyoidnyb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jyoumei.cn/gtqmlredew.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sysykeji.top/gtokkscalg.html

Ruby: s.split(",");  s.split
来源：http://hz.nanxinkj.top/gtutrfkiwx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydjk.org.cn/gtbazgxmgw.html

[E08] 数组按分隔符合并
来源：http://hz.jqgufenzy.top/gtrzracese.html

Py:   ",".join(items)
来源：http://hz.ppjwa.cn/gtnklxxhtv.html

PHP:  implode(",", $items);
来源：http://hz.gogol.net.cn/gtizqppgdj.html

JS:   items.join(",")
来源：http://hz.pycfn.com/gthvxwytwt.html

TS:   items.join(",")
来源：http://hz.hfpthk.cn/gtfwwcmnnk.html

Java: String.join(",", items)
来源：http://hz.daria6918.cn/gtsywsmihe.html

Go:   strings.Join(items, ",")
来源：http://hz.cdnleiting.top/gtfwarrqtt.html

Ruby: items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtlpxilfsb.html

C#:   string.Join(",", items)
来源：http://hz.gzhubu.top/gtqsbvdaml.html

[E09] 去除所有空白字符
来源：http://hz.ywan-chungtsiang.top/gtkozecmzh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gtiplxvjjn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gtzevoaawc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtmbljyqxw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtpspswobb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.smart0.xyz/gtvvoctfbe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gotoacloud.top/gtwkfjgzlj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtkeljgmce.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.52xcode.cn/gtsuwwyjjz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jiagoushi.top/gtfmcrwqaf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gzhubu.top/gtvrnfpmfj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuanzhike.top/gtwolmozea.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtoiqsbzog.html

TS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtamiqeqwx.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtcwxqciwx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtojqgxikv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gtgndwrdod.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenjidiqi.icu/gtkoablgxr.html

[E11] 反转字符串
来源：http://hz.gzhubu.top/gtliiuasae.html

Py:   s[::-1]
来源：http://hz.fengsongda.top/gtptomzzgt.html

PHP:  strrev($s);
来源：http://hz.zhoulong.xyz/gtjgpmypgm.html

JS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtnmzeptgm.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gttkrptudp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhongyouzk.top/gtlzilggyf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.redwolf501.top/gtjbooqwsm.html

Ruby: s.reverse
来源：http://hz.chenlongwang.top/gtkjwoopuh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtcbukzawr.html

[E12] 统计某字符出现次数
来源：http://hz.ehwqpu.com/gtkxzixhem.html

Py:   s.count("a")
来源：http://hz.yuxming.cn/gtprvyayum.html

PHP:  substr_count($s, "a");
来源：http://hz.aibaodan.cn/gtpwisuzuo.html

JS:   s.split("a").length - 1
来源：http://hz.zhixingplan.top/gtmxpiacex.html

TS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtmkfqgook.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xingfuxueyuan.xyz/gtlzjxxcik.html

Go:   strings.Count(s, "a")
来源：http://hz.gzhubu.top/gtfqklmqxh.html

Ruby: s.count("a")
来源：http://hz.pycfn.com/gtdkjsagvy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jyoumei.cn/gtqxwfhanm.html

[E13] 逐字符遍历
来源：http://hz.wangshuangyany.cn/gtixnosbgx.html

Py:   for ch in s: print(ch)
来源：http://hz.gzhubu.top/gtfsftplsw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fengsongda.top/gtjwydpucp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtpkrokzpr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtfeyihhtc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtfsuprkwl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guowangkeji.top/gtfsocfpte.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtuzomxvsx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hammf.cn/gtijmfvofy.html

[E14] URL 编码与 Base64
来源：http://hz.gotoacloud.top/gtcgwqcxct.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnxiangtu.top/gtcrazxwyp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guannengcc.top/gtaqwrgsky.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cheryme.top/gtzyievyep.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuetiantiany.cn/gtbjywybso.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.quarkkingdee.top/gtmbyszsqw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cashguo.top/gtxgldxwyh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.9152youxi.cn/gtvhuuhwjy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.52xcode.cn/gtpbdwpizu.html

[E15] HTML 转义 / 反转义
来源：http://hz.zycfv.cn/gtqjbhcsvg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.mhx1999.top/gtbivhzjtp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.havefunace.top/gtixvjkgqs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtcslhlwua.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgufenzy.top/gtaifnfiqf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jlsjyb.cn/gtgnwzjjhw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nwbrower.top/gtjhnwnkfi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.c1oappe.top/gttiykjcvg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ywan-chungtsiang.top/gtgcskmcuk.html

[E16] 数字千分位
来源：http://hz.shzxlz.cn/gtxjokczsx.html

Py:   f"{1234567:,}"
来源：http://hz.zhixingplan.top/gtejhuznhk.html

PHP:  number_format(1234567);
来源：http://hz.fengsongda.top/gtwhgndnpe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtgapksnih.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtijsufotf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinghuilouyu.cn/gtcsadtjaa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cdnleiting.top/gtrmkxhcgs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgfzy.top/gtxlimbvxh.html

C#:   1234567.ToString("N0")
来源：http://hz.ppjwa.cn/gtkfjuvlrn.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtlmamnnqm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.redwolf501.top/gtsqylxalt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtxgalnjrr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtwuaiippx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtcxidotaa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gtbpbhijbb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fengsongda.top/gtcqjkchpx.html

Ruby: s.capitalize
来源：http://hz.hongshengwenyu.top/gtxflzsebo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.smart0.xyz/gtpdtymkfw.html

[E18] 模板占位符替换
来源：http://hz.zhixingplan.top/gtinjtqabp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.0kj1m.cn/gtgrzddnzk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.c1oappe.top/gtxysgoiyc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhoulong.xyz/gtxjgobyyk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtuzklwlez.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.svipenyu.cn/gtmgmpzrgu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fzhhl.top/gtzsczafiu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dianchejie.cn/gtpehbtpuv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.snrcjt.cn/gtubizkefu.html

[E19] 多行文本按行拆分
来源：http://hz.hnqzz.top/gtsilhjywa.html

Py:   s.splitlines()
来源：http://hz.yj20258.top/gtbajqtuka.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtwroorqio.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtaadqdlhu.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtnrpdycxv.html

Java: s.lines().toList()
来源：http://hz.ivvv.top/gtarpxayya.html

Go:   strings.Split(s, "\n")
来源：http://hz.ppjwa.cn/gtwdqjottf.html

Ruby: s.lines
来源：http://hz.yuxming.cn/gtqwytkwpl.html

C#:   s.Split('\n')
来源：http://hz.jiagoushi.top/gtrkgtllrj.html

[E20] 判断字符串是否为空
来源：http://hz.gzhubu.top/gtodcvlyyn.html

Py:   if not s:
来源：http://hz.xylfe.cn/gtheybcmil.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hysaishi.cn/gtqxwgkaim.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hfpthk.cn/gtxzwayrdl.html

TS:   if (s === "") {}
来源：http://hz.xuetiantiany.cn/gtwszabfvi.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtudrbvrsb.html

Go:   if s == "" {}
来源：http://hz.andypj.xyz/gtceadgnwp.html

Ruby: if s.empty?
来源：http://hz.quarkkingdee.top/gtjocuolpx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtkzgxhidj.html

[E21] 超长截断加省略号
来源：http://hz.gogol.net.cn/gtkorizezw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dashuyun.cn/gtnrzkhwfb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.mhx1999.top/gtewfbtgmz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtdwilvvmv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtmnekqgca.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtharnaoye.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgfzy.top/gtcydvbzbg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hysaishi.cn/gtezhrwcdg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtooovrpka.html

[E22] 字节长度与字符长度
来源：http://hz.ydjk.org.cn/gtcwngtbkb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xinyue.icu/gtlnmccmvp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtaipjskmr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtammkmhuf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtpikrxvzx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhengqikj.top/gtturfnivm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhongyouzk.top/gtzvjdvdnp.html

Ruby: s.bytesize;  s.length
来源：http://hz.ywan-chungtsiang.top/gttsxecjtg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.snrcjt.cn/gtmdiijsuv.html

================================================================================
来源：http://hz.shzxlz.cn/gtaclfwfef.html

F. 文件与目录
来源：http://hz.zhengqikj.top/gtaimefbgw.html

================================================================================
来源：http://hz.zhengqikj.top/gtmpkmrxla.html

[F01] 读取整个文件
来源：http://hz.dashuyun.cn/gtqmdbomrm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtrwmsixxi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cqqwz.cn/gtukjjqrxz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.meibo888.top/gtengzatnc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.kuanghao11.cn/gttagyiyfo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtmxnojkcy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sufxvd.cn/gtozvemdwn.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gtqwjtragf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gthxlkzwvu.html

[F02] 逐行读取文件
来源：http://hz.jiagoushi.top/gtxolkzhko.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yongpay.top/gtbahbiuhg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtwuubunji.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.0kj1m.cn/gtgltlyujg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtnmzflytu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtjvdaljjs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtufwzncmt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtahzhysnk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gtlafmfdor.html

[F03] 写入文件（覆盖）
来源：http://hz.wangdashe.top/gtyavrigbg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuxming.cn/gtovizwlft.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cucudq.cn/gtfappyomc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtzokdydcd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtkoefboat.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ppjwa.cn/gtyagmhgje.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtnbtbgpsr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yvedp.cn/gtnidyclyr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtahwwfhun.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtzeskwloh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daxiang520.top/gtbuhixkug.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tanke756.top/gtftrlyedb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtifuinnjb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtxcjzkpju.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xziqi.cn/gtuljdfrat.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yonumen.top/gtvlbvkbbd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sxryk.cn/gtqfajibkz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangdashe.top/gtldfdmljq.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhongyouzk.top/gtghoxsnhi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtinqadjvh.html

PHP:  file_exists("a.txt");
来源：http://hz.birdmap.top/gtyjeoptbu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtbfywzwnn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtiejwylis.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtikmqqfef.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cheryme.top/gtdwbpdyku.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtnhsomvjc.html

C#:   File.Exists("a.txt")
来源：http://hz.daria6918.cn/gtfzwnhztj.html

[F06] 删除文件
来源：http://hz.zhaomingkeji.xyz/gtkfqajuqq.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtkfbcanfm.html

PHP:  unlink("a.txt");
来源：http://hz.smart0.xyz/gtghdwsrdc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtwgsitdyr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtmqdsvjbe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtbcwwtlko.html

Go:   os.Remove("a.txt")
来源：http://hz.hnqzz.top/gtobiqxigx.html

Ruby: File.delete("a.txt")
来源：http://hz.pengpengdd.cyou/gtpcufvxrx.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gtrliulfio.html

[F07] 创建目录（含多级）
来源：http://hz.tian-w.cn/gtjwwecpil.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtchunykud.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.birdmap.top/gtfaqdlnpi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtjlctfvqv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtnjupzykl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.birdmap.top/gtelhkzhsa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gthfwpodnz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cucudq.cn/gtlqlytmkq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shzxlz.cn/gtucslshsr.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gtlhqyzcrc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ppjwa.cn/gtdjxhswlu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gtkoepnwld.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gttsotvbfu.html

TS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtqrpkelib.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ivvv.top/gtbrkldbsp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.bjfxy.top/gtavyrspwc.html

Ruby: Dir.children("dir")
来源：http://hz.chenjidiqi.icu/gtorppjcpr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.iojbl.cn/gtiijixtex.html

[F09] 获取文件大小
来源：http://hz.xziqi.cn/gtbmyxhlfu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zdqjudy.top/gtdeizmpai.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gtclxsvcmy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtwtgeptwb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xylfe.cn/gtzjbwehfr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gthhjkwmqc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cdnleiting.top/gtjxwpkrto.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtiuxrobfx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gtvdshofkv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jqgfzy.top/gtdwoludfc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtqtqnztqt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.birdmap.top/gtfascfyrp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtypteesaa.html

TS:   path.extname("a.txt")
来源：http://hz.cucudq.cn/gtcfjtotnl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yonumen.top/gtlchuvkjo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtbwphiwsu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtehgjyyce.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtxjzpkypg.html

[F11] 复制与移动文件
来源：http://hz.meibo888.top/gtegcpdyrg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtjtymeieh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtmelkeiyo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtvcptzflk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtesltnuye.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.kuanghao11.cn/gtjdjsxjil.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hysaishi.cn/gtnroxijih.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtmkpzmxar.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xingfuxueyuan.xyz/gtrzmbaihm.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtfpzxqkxg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shuidangran.top/gtxmheqmlv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtqyiiwgxq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shangyingyoupin.top/gtevtrewnn.html

TS:   // 同上
来源：http://hz.yvedp.cn/gtqffdtlno.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ivvv.top/gtbkymkwhx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtgdsfcans.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtyqufbuiy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtnalylfmn.html

================================================================================
来源：http://hz.cdnleiting.top/gtnnklydsu.html

G. 面向对象
来源：http://hz.tanke756.top/gtbcumynnl.html

================================================================================
来源：http://hz.birdmap.top/gttbeidmvz.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtjsxyrmsx.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gtgpavnams.html

PHP:  class User {}
来源：http://hz.zhoulong.xyz/gthkmwdneh.html

JS:   class User {}
来源：http://hz.ydjk.org.cn/gtfzpixpke.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gtklgppmbf.html

Java: class User {}
来源：http://hz.yangfankeji.com/gtygdbanlk.html

Go:   type User struct { Name string }
来源：http://hz.tian-w.cn/gtobbkendn.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gttnanziax.html

C#:   class User {}
来源：http://hz.sxryk.cn/gtvljizauw.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gtmrfxnyrr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnxiangtu.top/gtxfpgzjur.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtrqfkwrwt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtmbxlnyvz.html


<!-- 参考信息 -->