代发 wailian999

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gtudwesdkb.html

Ruby: s.index("x")
来源：http://hz.gotoacloud.top/gtnjxyvpty.html

C#:   s.IndexOf("x")
来源：http://hz.zdqjudy.top/gtdrtpcbow.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cdnleiting.top/gtxfuyufua.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jlsjyb.cn/gtpbzlzwtv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dashuyun.cn/gtkarwwviv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gtyapsqwav.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtfyfynwsv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtegnxenjd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yuanzhike.top/gtrfsamwpe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ywan-chungtsiang.top/gtwzlewlot.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.52xcode.cn/gtudfqvuxy.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtujzeghoe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sweek.top/gtwsqdbzek.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.kuanghao11.cn/gtyalgfdrf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtfdcebigj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtnfpgvfrg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtqhqoxxzf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhoulong.xyz/gtoelbzlzw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shzxlz.cn/gtqyirbdyh.html

C#:   s.Replace("a", "b")
来源：http://hz.tian-w.cn/gtoetozsmn.html

[E07] 按分隔符拆分
来源：http://hz.vqdsnc.cn/gtlmgvsiam.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258888.top/gtsuumdqoy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenjidiqi.icu/gtdcxomcnf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cdnleiting.top/gtuumiuuwm.html

TS:   s.split(",")
来源：http://hz.c1oappe.top/gtpcujlltj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhijiandao.cn/gtvbmerrqn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daria6918.cn/gtzxsfvclx.html

Ruby: s.split(",");  s.split
来源：http://hz.tanke756.top/gtktafpuxt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.bjfxy.top/gttgprpkiw.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtemtcezpz.html

Py:   ",".join(items)
来源：http://hz.yuanzhike.top/gtjzsxvpri.html

PHP:  implode(",", $items);
来源：http://hz.feifeiyinyue.top/gtbejinixl.html

JS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtquapgfge.html

TS:   items.join(",")
来源：http://hz.fengsongda.top/gtgoumufgw.html

Java: String.join(",", items)
来源：http://hz.daxiang520.top/gtpgqbreyi.html

Go:   strings.Join(items, ",")
来源：http://hz.jianghu66.top/gtsgnolbgz.html

Ruby: items.join(",")
来源：http://hz.jinghuilouyu.cn/gtgnqzleja.html

C#:   string.Join(",", items)
来源：http://hz.ydjk.org.cn/gtppydkodc.html

[E09] 去除所有空白字符
来源：http://hz.feifeiyinyue.top/gtcqzfjhea.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hongshengwenyu.top/gtvoouwxyy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenlongwang.top/gtdgltzyne.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtalqmxfmi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtbqunxsem.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuanzhike.top/gtjesvmouj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cucudq.cn/gtmlaghscp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.c1oappe.top/gtdipyljof.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jianghu66.top/gtmiyegcmz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydjk.org.cn/gtxemlreia.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhoulong.xyz/gtkkgwiepe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtcuyjprmy.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtmiqioelo.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtlekaqxne.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gtihqwrjsr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sweek.top/gtevdiyzvn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigufen.top/gtfvnpxkmi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtobeyykpc.html

[E11] 反转字符串
来源：http://hz.wangdashe.top/gtobsaaeds.html

Py:   s[::-1]
来源：http://hz.jinqigufen.top/gtwjppyoan.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtqvgiumlw.html

JS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtgrthjkfo.html

TS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtpgoieqbq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenlongwang.top/gtnidibaoz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.c1oappe.top/gtlncmyabu.html

Ruby: s.reverse
来源：http://hz.ybcxt.top/gtsjfjaydk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtrndnvwaa.html

[E12] 统计某字符出现次数
来源：http://hz.aizwys.cn/gtxorhxius.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gtmsjrhtte.html

PHP:  substr_count($s, "a");
来源：http://hz.mhx1999.top/gtgfztloqp.html

JS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtcvilopoq.html

TS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtbpepyioy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuetiantiany.cn/gtmwgpnqcu.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigufen.top/gtralgyycy.html

Ruby: s.count("a")
来源：http://hz.tanke756.top/gtgqczjcgr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tanke756.top/gtmpzhxxdv.html

[E13] 逐字符遍历
来源：http://hz.0kj1m.cn/gtlvbskdgx.html

Py:   for ch in s: print(ch)
来源：http://hz.dashuyun.cn/gthdsfaxcn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shzxlz.cn/gtgamgqpks.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtoxtkdyqg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gthtjicntf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtjqggradl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenjidiqi.icu/gtdvggbvmi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gotoacloud.top/gtclkywhby.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yvedp.cn/gtzyhupbly.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtdtcbwfcs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cucudq.cn/gtqciqksxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daxiang520.top/gtxyxhohca.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hysaishi.cn/gtooiqhcjw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.wangshuangyany.cn/gtysaplbxn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gtaffkvntu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.snrcjt.cn/gtrxqkmblb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sysykeji.top/gtbosfpbuw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gtwlmrtigo.html

[E15] HTML 转义 / 反转义
来源：http://hz.316326.xyz/gtrjjjsqig.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.0kj1m.cn/gtbqmmdxua.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.9152youxi.cn/gttaoncbhn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hysaishi.cn/gtthrouypn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.haohaochexian.top/gtzlveoyjn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.c1oappe.top/gtaxkjidgr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gogol.net.cn/gtgmndrpqw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gtjslkexxw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gtevizykrr.html

[E16] 数字千分位
来源：http://hz.cashguo.top/gtiuvmrrof.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtoxpfkuvx.html

PHP:  number_format(1234567);
来源：http://hz.yj20258.top/gthmizlaiq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtvxddspeu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtvenvfacx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ivvv.top/gtwqkabydb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dianchejie.cn/gtienjxrss.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtjiwsjrpg.html

C#:   1234567.ToString("N0")
来源：http://hz.sweek.top/gtamzrhyzv.html

[E17] 首字母大写
来源：http://hz.svipenyu.cn/gtoiwajgvj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xziqi.cn/gtrnzbpshy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nwbrower.top/gtzvcwsoxj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtdndojbgn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtyrgjlgsd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dashuyun.cn/gtgkkhdqcn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuanzx.com/gtndgapysx.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtiqtppuju.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.haohaochexian.top/gtvmfcrkbh.html

[E18] 模板占位符替换
来源：http://hz.52xcode.cn/gtmrjwbwwi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenjidiqi.icu/gtkrggniqy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydjk.org.cn/gtuwmnwsom.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtlsexwnty.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtgrpvxiyz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daxiang520.top/gthsckwcct.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhiwuduotai.top/gtoyjwimtf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gtgsdkhfnu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yangfankeji.com/gtssmyllcb.html

[E19] 多行文本按行拆分
来源：http://hz.yongpay.top/gtpcvpunow.html

Py:   s.splitlines()
来源：http://hz.jqgfzy.top/gtvlbhsidb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtldybzubk.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtyzwuleao.html

TS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtdfnvagqs.html

Java: s.lines().toList()
来源：http://hz.ywan-chungtsiang.top/gtgzzmaxsv.html

Go:   strings.Split(s, "\n")
来源：http://hz.yueranfly.top/gtgzzpsxsc.html

Ruby: s.lines
来源：http://hz.cucudq.cn/gtkhhljsgh.html

C#:   s.Split('\n')
来源：http://hz.bjfxy.top/gtdvwxrfuv.html

[E20] 判断字符串是否为空
来源：http://hz.ydjk.org.cn/gteypzzljn.html

Py:   if not s:
来源：http://hz.yj20258888.top/gtfjfjimlr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gtcxnvyzky.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xingfuxueyuan.xyz/gtsshybwsy.html

TS:   if (s === "") {}
来源：http://hz.yj20258.top/gtfwutcfkq.html

Java: if (s.isEmpty()) {}
来源：http://hz.cdnleiting.top/gtownaxbsa.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gtxzdfhwlg.html

Ruby: if s.empty?
来源：http://hz.jinghuilouyu.cn/gtgxfbxrfb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtqznhhjvu.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gtyytnagxp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gtvgdlncaf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yvedp.cn/gtfgtgtjxv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtvhfvmlnj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtfujauaqv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtmlphqfjv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cqqwz.cn/gteuosngex.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnqzz.top/gtgyafdyhr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtjpcaptrx.html

[E22] 字节长度与字符长度
来源：http://hz.jianghu66.top/gtqeubsffw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gtdhegvfie.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtovwteyjm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtnzregxoh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtzwzckdme.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.9152youxi.cn/gtfasxqfpb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yonumen.top/gtmsqkrmxc.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtrdqfhgms.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenjidiqi.icu/gtgiocmikf.html

================================================================================
来源：http://hz.sweek.top/gtycmanwnt.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gtxovmnxyc.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtnxwgpthj.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtwtovjlej.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nwbrower.top/gtuqcexika.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yongpay.top/gtvikzdfgm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtgywtwbxk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ppjwa.cn/gthncbmlmb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtoborlxbf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shzxlz.cn/gtmbbhijaq.html

Ruby: File.read("a.txt")
来源：http://hz.hongshengwenyu.top/gtcatmhpsv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gtldrggkxl.html

[F02] 逐行读取文件
来源：http://hz.ivvv.top/gtyvfqouqn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fzhhl.top/gtxhboakgd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtwxaxcvhd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtcqbntdby.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.quarkkingdee.top/gtgpwggsoi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtasyerldw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.52xcode.cn/gtitlueghq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangdashe.top/gtvyxmtxex.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gaohongyu789.top/gtlkvtokqo.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtjcznmvwy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtuzpbtmto.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtvkqofxms.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtqxuogkii.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gthwlhtgko.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tanke756.top/gtnkiekcnp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtmiijlcda.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.vqdsnc.cn/gtkjshxycq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtoaxuxpef.html

[F04] 追加写入文件
来源：http://hz.chenjidiqi.icu/gtyhuxfnfz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pycfn.com/gtznpazjxm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dashuyun.cn/gtttdedomd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtiysphxbf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtlhdttpwl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jyoumei.cn/gtebmqijrg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yvedp.cn/gtdfotwaan.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinyuanbaomall.cn/gtcwlapfxc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtizufhsaq.html

[F05] 判断文件或目录是否存在
来源：http://hz.316326.xyz/gtuhipjyni.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.feifeiyinyue.top/gttntxjoyk.html

PHP:  file_exists("a.txt");
来源：http://hz.xuanzx.com/gtlheurabq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtmmwcmilc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtgffuysnz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtwfahucky.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hnqzz.top/gtbpdovlhv.html

Ruby: File.exist?("a.txt")
来源：http://hz.ppjwa.cn/gtlvgyhtgq.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtftpjwcxc.html

[F06] 删除文件
来源：http://hz.tian-w.cn/gtqtieqlrz.html

Py:   os.remove("a.txt")
来源：http://hz.yongpay.top/gtxgomsztn.html

PHP:  unlink("a.txt");
来源：http://hz.jiagoushi.top/gtmyncjpae.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtmscdeoew.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gtxwjrfaqj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtebreuwgv.html

Go:   os.Remove("a.txt")
来源：http://hz.zhoulong.xyz/gttmptxctn.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtiyatjpmy.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gtdwmudfwv.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtxttldkgl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sysykeji.top/gtdlyxvhsz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.haohaochexian.top/gtaqbljwgp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtdaqdjgrw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gogol.net.cn/gtrmyhvfkh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gotoacloud.top/gtetzltvzv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yvedp.cn/gtkdbtirbm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtzewlmqcx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtacszzjko.html

[F08] 遍历目录
来源：http://hz.jinghuilouyu.cn/gtvpxsiswr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhengqikj.top/gtqdjoaaib.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.feifeiyinyue.top/gtdnxrrytk.html

JS:   fs.readdirSync("dir")
来源：http://hz.daxiang520.top/gtfbwmbclf.html

TS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtumypvmhq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtdpudshkm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.kuanghao11.cn/gtbzjzangf.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258.top/gtugsbfvow.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zdqjudy.top/gtvhhpwvgd.html

[F09] 获取文件大小
来源：http://hz.fengsongda.top/gtmentyshl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuetiantiany.cn/gtoxbpiiey.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtzuojspdw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtlerxexmi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtdvkcczbr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gteikcijzw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gtziidfdpl.html

Ruby: File.size("a.txt")
来源：http://hz.sxryk.cn/gtriuuhwfp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yanxiufei.cn/gtujawhwod.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.svipenyu.cn/gtuwvvjsfo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtkeirolno.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cdnleiting.top/gtnjnrwqxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gttivtlewg.html

TS:   path.extname("a.txt")
来源：http://hz.sxryk.cn/gthdwjgisk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinghuilouyu.cn/gtkzbmuvyb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cucudq.cn/gtkejqdfcb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtqahgrphp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtshmrpsyc.html

[F11] 复制与移动文件
来源：http://hz.cucudq.cn/gtgybttpfj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtzeeqiyha.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yueranfly.top/gtmxagpfdz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtlqnhwvoc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtcdskfbzw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.feifeiyinyue.top/gtdwzjglaz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.c1oappe.top/gtdoaqrpfh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtovqynkxf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtoghfjvbg.html

[F12] CSV 读写
来源：http://hz.dianchejie.cn/gtyajmpdev.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gtwmdewiix.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenlongwang.top/gtqdppfkfv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.feifeiyinyue.top/gtijradpbk.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtjcsnkyem.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gthalirnok.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pengpengdd.cyou/gthmanoiwt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gttkcxirhk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hongshengwenyu.top/gtewiyzjjm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtitqojfmg.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtyhmyvqiu.html

================================================================================
来源：http://hz.sxryk.cn/gtqweylpet.html

[G01] 定义类
来源：http://hz.yj20258.top/gtimksbosg.html

Py:   class User: pass
来源：http://hz.yj20258.top/gtsxeuaknd.html

PHP:  class User {}
来源：http://hz.shanyushiyangkeji.top/gtwolhsbvg.html

JS:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtoddjvgrb.html

TS:   class User { name: string = ""; }
来源：http://hz.jiagoushi.top/gtbpzvvqxd.html

Java: class User {}
来源：http://hz.yj20258.top/gtywrvhkvp.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gttdrjqyib.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtxoulaknh.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtiuirloaw.html

[G02] 构造函数
来源：http://hz.tanke756.top/gtwvciljrd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangshuangyany.cn/gtuftnmsxa.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yonumen.top/gtohjkwqgh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtjjksbbgl.html

TS:   constructor(public name: string) {}
来源：http://hz.zhixingplan.top/gtcynjgpkk.html

Java: User(String name) { this.name = name; }
来源：http://hz.316326.xyz/gtudptqwjq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtbdfrfotr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daxiang520.top/gtsdexdair.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtappkjsxs.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtzvbnwbit.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtfudsmasi.html

PHP:  public string $name = "x";
来源：http://hz.sufxvd.cn/gtmvnawlmc.html


<!-- 参考信息 -->