代发 wailian999

[E02] 重复字符串
来源：http://hz.quarkkingdee.top/gtywtqluit.html

Py:   "ab" * 3
来源：http://hz.yuxming.cn/gtfqdhijvg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nanxinkj.top/gtmmdupkoo.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtymaisnsp.html

TS:   "ab".repeat(3)
来源：http://hz.tanke756.top/gtyassmdfu.html

Java: "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtsjjngnao.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jianghu66.top/gttvdrorof.html

Ruby: "ab" * 3
来源：http://hz.ydzc1.top/gttcxurryc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.52xcode.cn/gtncvjzyjr.html

[E03] 截取子串
来源：http://hz.sweek.top/gthhcrrgys.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydjk.org.cn/gtjbczpbix.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhoulong.xyz/gtbadxjdpr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtqgmbkupv.html

TS:   s.slice(1, 4)
来源：http://hz.9152youxi.cn/gtcmalwtpr.html

Java: s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtnviqvllg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shanyushiyangkeji.top/gtxqjrfnax.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cashguo.top/gtjghnvcfh.html

C#:   s.Substring(1, 3)
来源：http://hz.fengsongda.top/gtsbxptyqm.html

[E04] 查找子串位置
来源：http://hz.52xcode.cn/gtassuoiei.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydjk.org.cn/gtnstnntjn.html

PHP:  strpos($s, "x");
来源：http://hz.hysaishi.cn/gtxriyowro.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gogol.net.cn/gtmtaueren.html

TS:   s.indexOf("x")
来源：http://hz.yuanzhike.top/gtnhbayexj.html

Java: s.indexOf("x")
来源：http://hz.ehwqpu.com/gtjoejrqdc.html

Go:   strings.Index(s, "x")
来源：http://hz.yuanzhike.top/gtqglhcscd.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtbziyesbm.html

C#:   s.IndexOf("x")
来源：http://hz.tian-w.cn/gtzkyesxyz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.smart0.xyz/gthegrfvda.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigufen.top/gtunaxmffj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.52xcode.cn/gtossisaet.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtsfdsauyq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.vqdsnc.cn/gtcxadokgn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtmszfxepf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yuxming.cn/gthqhfkthj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.bjfxy.top/gtuajbquxo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuanzhike.top/gtiivawndx.html

[E06] 替换子串
来源：http://hz.tianlin.xyz/gtywvvwwsx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.andypj.xyz/gtthcblrfh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xziqi.cn/gtrdzwbhkz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtgjljgnop.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtkbflntjj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtcwhilpkx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sxryk.cn/gtxmnrshpt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenzaomai.com/gtqnzelbix.html

C#:   s.Replace("a", "b")
来源：http://hz.jiagoushi.top/gtemkafzhh.html

[E07] 按分隔符拆分
来源：http://hz.fengsongda.top/gttdrmyybr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yueranfly.top/gtlkgifyaf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hammf.cn/gtgghginrh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydzc1.top/gtmegkawdd.html

TS:   s.split(",")
来源：http://hz.yuanzhike.top/gtsiotgglz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhoulong.xyz/gtuekbqbkc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.mhx1999.top/gtxtskaxdz.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtdruxmvxo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tian-w.cn/gtjychaqwq.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gtevseeudl.html

Py:   ",".join(items)
来源：http://hz.cheryme.top/gttiwzdecr.html

PHP:  implode(",", $items);
来源：http://hz.316326.xyz/gtqxgpiftn.html

JS:   items.join(",")
来源：http://hz.xuanzx.com/gtyckibzgc.html

TS:   items.join(",")
来源：http://hz.nwbrower.top/gtycvdyatb.html

Java: String.join(",", items)
来源：http://hz.jiagoushi.top/gtfovdqwja.html

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gtgascxnzp.html

Ruby: items.join(",")
来源：http://hz.hfpthk.cn/gtyuewmldk.html

C#:   string.Join(",", items)
来源：http://hz.gogol.net.cn/gturmkiaki.html

[E09] 去除所有空白字符
来源：http://hz.hammf.cn/gtayxpqibu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.316326.xyz/gtkgdwvxtp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xinyue.icu/gthgbuqiap.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhaomingkeji.xyz/gtipzwgtxr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gtrgxsksal.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtyhxuprnk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgufenzy.top/gtctziarxf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.iojbl.cn/gtcodxidua.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fengsongda.top/gtdnltwtye.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtxxduhvfr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gtohhuuwyh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nwbrower.top/gtuklwusxn.html

JS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtgratxkgc.html

TS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtykesytys.html

Java: String.format("%03d", 7)
来源：http://hz.jqgfzy.top/gtqnqgfpvc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xziqi.cn/gtnqopofut.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtglzmkzfg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtoqapbqzn.html

[E11] 反转字符串
来源：http://hz.xuetiantiany.cn/gtoixhivrn.html

Py:   s[::-1]
来源：http://hz.hnxiangtu.top/gtdfufitfc.html

PHP:  strrev($s);
来源：http://hz.0kj1m.cn/gtaoywvbyo.html

JS:   [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtydomdqzv.html

TS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtaiyvnynv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yangfankeji.com/gtppvpxhja.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258.top/gteeqaewax.html

Ruby: s.reverse
来源：http://hz.feifeiyinyue.top/gtnbayqljk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtvvhxpzmu.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtwqdqzbas.html

Py:   s.count("a")
来源：http://hz.aibaodan.cn/gtstrrhffj.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgfzy.top/gtvgfebqrb.html

JS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtoyhaqfoo.html

TS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtaptvjave.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.birdmap.top/gtfnzbbhpf.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgufenzy.top/gttnztkoto.html

Ruby: s.count("a")
来源：http://hz.sufxvd.cn/gtiahsyutz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yuxming.cn/gtshmtbleq.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtflcjxqjg.html

Py:   for ch in s: print(ch)
来源：http://hz.wangshuangyany.cn/gtdjwrzner.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cdnleiting.top/gtwkvlekuo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtbvbxdejq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtlgejyvgo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gtxjtqufag.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtkbpljryt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtzqfgsazg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cheryme.top/gtkjwnhehv.html

[E14] URL 编码与 Base64
来源：http://hz.yongpay.top/gtdosbadel.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.svipenyu.cn/gtwmnvxwtb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yvedp.cn/gtsejxhctk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.svipenyu.cn/gtddjprqkf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenjidiqi.icu/gtqinoqhmx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sweek.top/gtuameqklq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.haohaochexian.top/gtevrgsnmd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.vqdsnc.cn/gtgnvcwhfo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aibaodan.cn/gtuqytxcyk.html

[E15] HTML 转义 / 反转义
来源：http://hz.sweek.top/gtzoatjwfx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xinyue.icu/gtppvbfqlr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.quarkkingdee.top/gtkcalfimq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hammf.cn/gtekyxahlw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gteekqrxea.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtaefeiutl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tianlin.xyz/gtulqdmpss.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtvoznckaj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jqgfzy.top/gthfgmztee.html

[E16] 数字千分位
来源：http://hz.kuanghao11.cn/gtdozgiuay.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gtiddilvxs.html

PHP:  number_format(1234567);
来源：http://hz.zhiwuduotai.top/gtsiywfohf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtgqtlhqwn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtfvvbncao.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gttrveflyo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daria6918.cn/gtyqopxzup.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cucudq.cn/gtztjzyyze.html

C#:   1234567.ToString("N0")
来源：http://hz.yangfankeji.com/gtrdboghcx.html

[E17] 首字母大写
来源：http://hz.kuanghao11.cn/gtooywdsac.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guannengcc.top/gtvnbisscw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zdqjudy.top/gtqfwkeenn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtcqifgznl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtorpturhp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gthjckahbf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnxiangtu.top/gtgjpghfuw.html

Ruby: s.capitalize
来源：http://hz.hongshengwenyu.top/gtnqydjhjy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxuanxn.top/gtvtgndavq.html

[E18] 模板占位符替换
来源：http://hz.gotoacloud.top/gtclcwiipk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtudbtpywf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ywan-chungtsiang.top/gtzftsuicf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtduchsilw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtralruxkb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.pengpengdd.cyou/gthexenicw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydjk.org.cn/gteeftojug.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xylfe.cn/gtyhbzdtyn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenzaomai.com/gttcydrjjf.html

[E19] 多行文本按行拆分
来源：http://hz.svipenyu.cn/gtoovnlslf.html

Py:   s.splitlines()
来源：http://hz.fzhhl.top/gtgzrcjcrw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ywan-chungtsiang.top/gtcfucivzj.html

JS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtqeqjaslw.html

TS:   s.split(/\r?\n/)
来源：http://hz.nanxuanxn.top/gtgkeamvog.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtczjroiqa.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtvgzoeayr.html

Ruby: s.lines
来源：http://hz.zhixingplan.top/gtdarwnijl.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gtiiugkqkf.html

[E20] 判断字符串是否为空
来源：http://hz.jiagoushi.top/gtoqeyxnod.html

Py:   if not s:
来源：http://hz.jinqigufen.top/gteqtntoan.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cqqwz.cn/gteonneazr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtuybzjzju.html

TS:   if (s === "") {}
来源：http://hz.iojbl.cn/gtgpbzgzth.html

Java: if (s.isEmpty()) {}
来源：http://hz.bjfxy.top/gtihykgrkw.html

Go:   if s == "" {}
来源：http://hz.snrcjt.cn/gtmdfbhech.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gtrhmljrhq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtobmrxtbh.html

[E21] 超长截断加省略号
来源：http://hz.aizwys.cn/gtyzdinbln.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtjrgtwcru.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtiyemvoze.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gttzjpswne.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gttwsipelm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtbxhvsqit.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daxiang520.top/gtsngvorji.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtvpqdioea.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ppjwa.cn/gtwedgfgdq.html

[E22] 字节长度与字符长度
来源：http://hz.yuxming.cn/gtvmevjzlu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258.top/gtthrgfkjv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtwdeubxef.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtwllgordv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtaqpktcbi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinghuilouyu.cn/gtgjsbarzi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gtoapefpcm.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangkeji.top/gtxkiyyleq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtmrkkwuwi.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnpucffdh.html

F. 文件与目录
来源：http://hz.gaohongyu789.top/gtslbwwwhn.html

================================================================================
来源：http://hz.andypj.xyz/gthzyjnqkq.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gtfktthncm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shuidangran.top/gtcnmxxhyp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xinyue.icu/gtvgufcbgw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guannengcc.top/gtxikorvwx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ybcxt.top/gtvjrhydmo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtrlnigqja.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuetiantiany.cn/gtckwrbzbh.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gtjyektsrf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cashguo.top/gtpgiwzqmk.html

[F02] 逐行读取文件
来源：http://hz.yangfankeji.com/gtizpxsqmr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigfzy.top/gttmeikxlf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258888.top/gtaukbmvas.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtpdpxdeav.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtpuzhsesc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtudzazvnt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.iojbl.cn/gtbkfmvfiu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sysykeji.top/gtkyvnfyab.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hammf.cn/gtbkwvpdtu.html

[F03] 写入文件（覆盖）
来源：http://hz.xinyue.icu/gtmezkpvqs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenzaomai.com/gtvrcmwdya.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zdqjudy.top/gtmhhpgrdq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtqabysotx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gttunpwrrz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yongpay.top/gtxeqiqwbh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtgextmjvt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dianchejie.cn/gtnojjqzal.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tianlin.xyz/gtexljoeib.html

[F04] 追加写入文件
来源：http://hz.iojbl.cn/gthhpalfed.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sweek.top/gticwbwpsm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtdmxplutc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtzwpzrzky.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtmhltzsdk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cucudq.cn/gtjptklciw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuxming.cn/gtfgtabato.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gtachafbuh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtlmmwnfmy.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtclwawfsw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zdqjudy.top/gtcqcmtypd.html

PHP:  file_exists("a.txt");
来源：http://hz.chenlongwang.top/gttnkpclhq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gterqvfhee.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtormrfrhw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtgnfisjvf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.snrcjt.cn/gtzndinybh.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtoozhyawf.html

C#:   File.Exists("a.txt")
来源：http://hz.chenlongwang.top/gtmlnicthr.html

[F06] 删除文件
来源：http://hz.ybcxt.top/gthmwuxtql.html

Py:   os.remove("a.txt")
来源：http://hz.9152youxi.cn/gthvzudack.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gtqpxlzenk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtecjiqzcz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtfwhwgqqb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gteufaqrce.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gtydoqtsfh.html

Ruby: File.delete("a.txt")
来源：http://hz.havefunace.top/gtwhhzowya.html

C#:   File.Delete("a.txt");
来源：http://hz.redwolf501.top/gtphxbyryx.html

[F07] 创建目录（含多级）
来源：http://hz.gogol.net.cn/gtrkvhrlow.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenzaomai.com/gtjozjbokl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.haohaochexian.top/gtjpepwbdg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtydikefnd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtqmhrvsju.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenjidiqi.icu/gtrrrzkuzn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hammf.cn/gtoppfbzlb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangkeji.top/gtsluafohs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtdvegeihk.html

[F08] 遍历目录
来源：http://hz.jqgfzy.top/gthywkhbuf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guannengcc.top/gtlosomsro.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gturyarxrz.html

JS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gthazyrsuh.html

TS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtwfbvnhwa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtvcgfpekk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgfzy.top/gtjekqsziy.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtnbqwahco.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gteenfbnre.html

[F09] 获取文件大小
来源：http://hz.jinyuanbaomall.cn/gtnzxrthme.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gtyyslgsjq.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258.top/gtawmjsbaz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtjrwocxns.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtdptlycve.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtwdstsaxs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cheryme.top/gtwkosqsxu.html

Ruby: File.size("a.txt")
来源：http://hz.cucudq.cn/gtpadptbol.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gtszklhhwg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtxgkvkgtt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtrlftdvne.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.meibo888.top/gttjzaujej.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtajvswxil.html

TS:   path.extname("a.txt")
来源：http://hz.yonumen.top/gtihayrvzq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xinyue.icu/gtyuyoelkn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.iojbl.cn/gtluntolnb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtkdfvldmd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.iojbl.cn/gtlcbxqswz.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtadxwxrom.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtpijvdugb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenjidiqi.icu/gtihxsrxlc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtxapkiyaf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtpwkqebis.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.redwolf501.top/gtcdbobbrs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtiypskuja.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtqcjgmekf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gttmawvmgg.html

[F12] CSV 读写
来源：http://hz.yj20258.top/gtuwgoyvha.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gtopzsammk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fengsongda.top/gtdbmmkbzy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.52xcode.cn/gthjrqqfmq.html

TS:   // 同上
来源：http://hz.hammf.cn/gtmgszrycw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj202588.top/gtloukedxl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yonumen.top/gtvwblhyek.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtcfqqchwi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zdqjudy.top/gtftzsjruf.html


<!-- 参考信息 -->