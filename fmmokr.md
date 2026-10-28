代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yanxiufei.cn/gtskhutfhd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guowangkeji.top/gtjretydmf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtozlmwgqj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shanyushiyangtech.top/gtjxnujawj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258888.top/gtdyvgofdp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jyoumei.cn/gtoqfnsxhm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtyxwkpouu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yvedp.cn/gtqljrvwry.html

[E06] 替换子串
来源：http://hz.yuanzhike.top/gtarpnhhbv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.mhx1999.top/gtlsboyuqq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shzxlz.cn/gtuddpzaoz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtqhapezpp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtuoqujtdr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtxxjkbxkz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.meibo888.top/gtoytvvlbl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.0kj1m.cn/gtxwfwtpif.html

C#:   s.Replace("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtidxnoisp.html

[E07] 按分隔符拆分
来源：http://hz.feifeiyinyue.top/gtejujeuao.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jyoumei.cn/gthqwjgkhl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhijiandao.cn/gtyqiorhlf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.iojbl.cn/gtwmvcqrcy.html

TS:   s.split(",")
来源：http://hz.guowangkeji.top/gtqjvmifxx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtjrzvnafq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tianlin.xyz/gtvyhzanjs.html

Ruby: s.split(",");  s.split
来源：http://hz.wangdashe.top/gtqdriujvr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sufxvd.cn/gtcpcwzkua.html

[E08] 数组按分隔符合并
来源：http://hz.jinyuanbaomall.cn/gtbsngdvdg.html

Py:   ",".join(items)
来源：http://hz.ydzc1.top/gtteytlujo.html

PHP:  implode(",", $items);
来源：http://hz.yuanzhike.top/gtpghfmqfp.html

JS:   items.join(",")
来源：http://hz.ppjwa.cn/gtlaiowxhi.html

TS:   items.join(",")
来源：http://hz.xuetiantiany.cn/gtdmodbmhn.html

Java: String.join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtkpgcwher.html

Go:   strings.Join(items, ",")
来源：http://hz.hysaishi.cn/gthkoxxtnf.html

Ruby: items.join(",")
来源：http://hz.ydjk.org.cn/gtjgsmzunz.html

C#:   string.Join(",", items)
来源：http://hz.cashguo.top/gtknqpcmzk.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtiqvgybeh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtotthlwgd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gtofytfelu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtlpuaxjkb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtjycpjdzh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgufenzy.top/gtjwrhwxpq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.kuanghao11.cn/gtmnivcwjx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xinyue.icu/gtjkdjixyw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hammf.cn/gtwmeanisf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtsjrfzbnm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gthfewymjm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gttcvztrex.html

JS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtbmdmjaxj.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtnqsaruka.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtvbouduad.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sweek.top/gtogayuuwf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtiyylcgaf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.snrcjt.cn/gtotuakoqg.html

[E11] 反转字符串
来源：http://hz.zdqjudy.top/gtykvacewm.html

Py:   s[::-1]
来源：http://hz.chenjidiqi.icu/gtuwptyckl.html

PHP:  strrev($s);
来源：http://hz.ydzc1.top/gtbgwecynv.html

JS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gthfyxbgcu.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtgaeqkmsu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aizwys.cn/gtzhkmlntb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangshuangyany.cn/gtjvgoqxsf.html

Ruby: s.reverse
来源：http://hz.yvedp.cn/gteeffooht.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtqjobyjaa.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtncbolcyz.html

Py:   s.count("a")
来源：http://hz.jqgufenzy.top/gtdbcljxln.html

PHP:  substr_count($s, "a");
来源：http://hz.xinyue.icu/gtofydmeze.html

JS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gtzwsxgvrf.html

TS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtcsoafkpm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daxiang520.top/gtgmyuuuov.html

Go:   strings.Count(s, "a")
来源：http://hz.xziqi.cn/gtioasyrtg.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtoqmrherw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gtludspllw.html

[E13] 逐字符遍历
来源：http://hz.jinghuilouyu.cn/gtflxusjye.html

Py:   for ch in s: print(ch)
来源：http://hz.xuanzx.com/gtwuravkmi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtyblvzlxv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cucudq.cn/gtjjpbxmdy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtbjqcreje.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.smart0.xyz/gtjnvybtin.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuetiantiany.cn/gtzwumqutx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gthvurgjrt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhaomingkeji.xyz/gtoaxvrmcs.html

[E14] URL 编码与 Base64
来源：http://hz.cdnleiting.top/gthlscyyhy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.c1oappe.top/gttmxmjfvo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jianghu66.top/gtsemhksit.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.snrcjt.cn/gtasxinhsv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cashguo.top/gtdhxdtzkv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtxnllwhif.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guowangkeji.top/gtbhhihvsd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daxiang520.top/gtbyxyonoy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenjidiqi.icu/gtmuxeipbc.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtmjofuvgd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gttsolhiga.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangkeji.top/gthtqzxqku.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigufen.top/gtboiowwrf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.birdmap.top/gtwcdnkgko.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gthcnhgdft.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pengpengdd.cyou/gtiwswehwf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinghuilouyu.cn/gtxtaddtiz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigufen.top/gtmflnyhdl.html

[E16] 数字千分位
来源：http://hz.iojbl.cn/gtqrkejkxn.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gtonnzklib.html

PHP:  number_format(1234567);
来源：http://hz.tian-w.cn/gtfqxqzubl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtbfysfovb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtrdjolhap.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuetiantiany.cn/gtsvkebhuh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.0kj1m.cn/gtzqalsseg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gotoacloud.top/gtznnbewtj.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gtgcicicxm.html

[E17] 首字母大写
来源：http://hz.hnxiangtu.top/gthpruzxsd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fzhhl.top/gtprnnzbwg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gtclvqwnve.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.feifeiyinyue.top/gtbemnpmlm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtcwoiyivi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtyrckfill.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhoulong.xyz/gtqyaevkcd.html

Ruby: s.capitalize
来源：http://hz.gaohongyu789.top/gtrxebhllp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.svipenyu.cn/gthwusvilc.html

[E18] 模板占位符替换
来源：http://hz.ivvv.top/gthwsajbbq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydzc1.top/gtbvqqqoxb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxinkj.top/gtlhiadpzb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtzmultlxc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtlwcekfyh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nwbrower.top/gtneaostqe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.iojbl.cn/gtssmnrzdf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fzhhl.top/gtldzzbfod.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenjidiqi.icu/gtdrmeshbb.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtrwiwnsfy.html

Py:   s.splitlines()
来源：http://hz.zhiwuduotai.top/gtwmbptxiv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hammf.cn/gtlfqbsnsp.html

JS:   s.split(/\r?\n/)
来源：http://hz.nwbrower.top/gtgeothvja.html

TS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gtdqgyurns.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gticvbfhkm.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhengqikj.top/gtqmzpoatu.html

Ruby: s.lines
来源：http://hz.gaohongyu789.top/gtiivihiso.html

C#:   s.Split('\n')
来源：http://hz.wangshuangyany.cn/gthwpwoade.html

[E20] 判断字符串是否为空
来源：http://hz.jinghuilouyu.cn/gtgdsdltby.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtiyapotiu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cashguo.top/gtddbmnvfn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yueranfly.top/gtftrugivb.html

TS:   if (s === "") {}
来源：http://hz.chenzaomai.com/gtktdemcql.html

Java: if (s.isEmpty()) {}
来源：http://hz.cdnleiting.top/gtdbyxfcle.html

Go:   if s == "" {}
来源：http://hz.birdmap.top/gtsfnxdhnm.html

Ruby: if s.empty?
来源：http://hz.andypj.xyz/gtnxfmovvy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.316326.xyz/gtbvoffpyt.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtrnqxoquy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtrtaizcss.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgufenzy.top/gtcpcrmqcx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtlqzfwqnx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtcwmnidli.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtojrzeujs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gotoacloud.top/gteollstif.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cqqwz.cn/gtgvmxxjak.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guannengcc.top/gtsmhuxxrm.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtzgnduqsb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.feifeiyinyue.top/gtcftuxdpx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtelxcgtrs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtxvijcfpy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtvhqqvdpd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xziqi.cn/gtepwrtgbo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cucudq.cn/gtmmoxixpz.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinyuanbaomall.cn/gtdhkcuynz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangshuangyany.cn/gtjynwjmbl.html

================================================================================
来源：http://hz.shuidangran.top/gtjhbqisxs.html

F. 文件与目录
来源：http://hz.shzxlz.cn/gtzxuvcqan.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtldkxcszs.html

[F01] 读取整个文件
来源：http://hz.hysaishi.cn/gtvyhcjaiz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtgkhvhtpl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yanxiufei.cn/gtjcvqaffc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ppjwa.cn/gtlsdfwqei.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cdnleiting.top/gtfeyrzwpj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gthkusvukv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gteouownhn.html

Ruby: File.read("a.txt")
来源：http://hz.tianlin.xyz/gtacvycnxe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cdnleiting.top/gtvhdsaopj.html

[F02] 逐行读取文件
来源：http://hz.zycfv.cn/gttfqlkzrl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtrfaejqdl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.daria6918.cn/gtzesfcsbw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtvyxqfnum.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtceaygujz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gthfodiiky.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gtlnffsfrf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtcgybnikx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgfzy.top/gtqohsahnp.html

[F03] 写入文件（覆盖）
来源：http://hz.cashguo.top/gtvbjuixxl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgufenzy.top/gtyfjislsf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.svipenyu.cn/gtasqrjzeb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtkjfpwery.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtgkmrcfrp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.svipenyu.cn/gthnbjrojp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgufenzy.top/gtvkysxxbi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guowangkeji.top/gttpmiitfv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.meibo888.top/gtjgwcjnms.html

[F04] 追加写入文件
来源：http://hz.tanke756.top/gtmzaaopav.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenjidiqi.icu/gtipvxsgnn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtczauxnxp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtqnofrzfo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtlrinwsnh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yueranfly.top/gtmsmmjqgp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pycfn.com/gtnrvbjpcl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cucudq.cn/gtntnyydre.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gtvusmreqb.html

[F05] 判断文件或目录是否存在
来源：http://hz.ehwqpu.com/gttgooovgz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuetiantiany.cn/gtadaafdkm.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtcudybgkm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtjyninjvs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtpkexefsl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtbgjzfjnr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.andypj.xyz/gtaurzxgbe.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenzaomai.com/gteubygajl.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtdcymunup.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtfgyunnme.html

Py:   os.remove("a.txt")
来源：http://hz.ydjk.org.cn/gthtfvoovk.html

PHP:  unlink("a.txt");
来源：http://hz.daxiang520.top/gthwrehksi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtxnujbpxc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtlwbujpij.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gttkhfulka.html

Go:   os.Remove("a.txt")
来源：http://hz.dashuyun.cn/gtinplmqjx.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gtkbzpkskt.html

C#:   File.Delete("a.txt");
来源：http://hz.aizwys.cn/gtbuklhiwe.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtaovbjufh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nwbrower.top/gtctqyhzyw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258888.top/gtvnbanjej.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtbgawfdwp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtvyhxkmfy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yangfankeji.com/gtrsxhpfzw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hywenlv.cn/gttpucbgsj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.feifeiyinyue.top/gtzkicmrtw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gtaxycbunm.html

[F08] 遍历目录
来源：http://hz.quarkkingdee.top/gtwrhoaojk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tanke756.top/gtkygdixsq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ivvv.top/gtznsxzquo.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtiovlpgnt.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtlaqzcbej.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtbegmohos.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinyuanbaomall.cn/gtylhqhnof.html

Ruby: Dir.children("dir")
来源：http://hz.ywan-chungtsiang.top/gtfsuliqwd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.iojbl.cn/gtwhhuwmiu.html

[F09] 获取文件大小
来源：http://hz.gogol.net.cn/gtwuzlxdat.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tian-w.cn/gtqgodaolq.html

PHP:  filesize("a.txt");
来源：http://hz.yuanzhike.top/gtbkwokvno.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gttbhnmavx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtyxcqegyj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gttkpvthhq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zdqjudy.top/gtnxlzhhrk.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtylxjxtty.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.snrcjt.cn/gtrzzhkozl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtdbjlgsdy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtikhglibn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtsswwomoh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtoaalvlps.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtrrkyxznz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtddfhxguy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258888.top/gtysbfcmws.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtqodcfoep.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtqmhexqwy.html

[F11] 复制与移动文件
来源：http://hz.cdnleiting.top/gtjadyrbaa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtrtymltyi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hysaishi.cn/gtktecyrqz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gthetqjbcc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtwkznejbr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtannzhwza.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtrxwvexrc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtrakxpmkz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shzxlz.cn/gtqpbejnsb.html

[F12] CSV 读写
来源：http://hz.zycfv.cn/gtvdcjciwm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gtrfghloct.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sxryk.cn/gtpvfrsxwe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtlkcdciaz.html

TS:   // 同上
来源：http://hz.zdqjudy.top/gtcaxdcyit.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sweek.top/gtadxcklwm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtabghyybh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gtubrdqdjz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ehwqpu.com/gtnlkrrpyf.html

================================================================================
来源：http://hz.ybcxt.top/gtgofbdawy.html

G. 面向对象
来源：http://hz.svipenyu.cn/gttznuzoyj.html

================================================================================
来源：http://hz.zdqjudy.top/gtmtnbptgb.html

[G01] 定义类
来源：http://hz.chenjidiqi.icu/gtnfrrrybe.html

Py:   class User: pass
来源：http://hz.feifeiyinyue.top/gtchnbcbpg.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtemmywwrz.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtqoznksez.html

TS:   class User { name: string = ""; }
来源：http://hz.jyoumei.cn/gtaczfzpzt.html

Java: class User {}
来源：http://hz.quarkkingdee.top/gtsnnzkarz.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gtwznmmuwp.html

Ruby: class User; end
来源：http://hz.xinyue.icu/gtkqxgmwdv.html

C#:   class User {}
来源：http://hz.yueranfly.top/gtjhptnmre.html

[G02] 构造函数
来源：http://hz.sufxvd.cn/gtjgsqcsjr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtydyppqrv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cdnleiting.top/gtttjtnhuf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gtiyaozjtn.html

TS:   constructor(public name: string) {}
来源：http://hz.svipenyu.cn/gtvvocmtmh.html

Java: User(String name) { this.name = name; }
来源：http://hz.aizwys.cn/gtsbwkdbqi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtxdhqopbk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtvaditdvy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhengqikj.top/gtqlokwaox.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtzjzomttc.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtdvopnztp.html

PHP:  public string $name = "x";
来源：http://hz.ywan-chungtsiang.top/gtupgelccm.html

JS:   this.name = "x";
来源：http://hz.yvedp.cn/gtfgeenoxp.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtakvjurfn.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gtppeebqqn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daria6918.cn/gtcmccbdla.html


<!-- 参考信息 -->