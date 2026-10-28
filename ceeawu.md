代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yanxiufei.cn/gtszcxdipa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hammf.cn/gtzwcxxkbn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zdqjudy.top/gtcqnwudtb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pengpengdd.cyou/gtilxxjsig.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhoulong.xyz/gtxyzvhvcu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aibaodan.cn/gtemocmrwv.html

[D25] Set 集合去重与交并差
来源：http://hz.xuanzx.com/gtbjjsepjp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxinkj.top/gtikmzijve.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.svipenyu.cn/gtypjphpob.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sweek.top/gtjacecnak.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgfzy.top/gtvlzwzkzi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ehwqpu.com/gtlqqdofqj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenzaomai.com/gtvgyphlbf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnqzz.top/gtbbhaweuu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhaomingkeji.xyz/gtvxwnptdg.html

[D26] 数组转字符串
来源：http://hz.snrcjt.cn/gtxagfwdco.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ivvv.top/gtspqkzbiw.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtfrgjqnjv.html

JS:   arr.join(", ")
来源：http://hz.xylfe.cn/gtzzxdkgui.html

TS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtfaqohxqy.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gthcttdnmq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtwhrlbfib.html

Ruby: arr.join(", ")
来源：http://hz.iojbl.cn/gtnqkmkvvx.html

C#:   string.Join(", ", list)
来源：http://hz.52xcode.cn/gtlxwvwlun.html

================================================================================
来源：http://hz.xylfe.cn/gteehwesgx.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtrsberumz.html

================================================================================
来源：http://hz.chenlongwang.top/gtorbqtlvu.html

[E01] 拼接字符串
来源：http://hz.jlsjyb.cn/gtqpfcagmh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sxryk.cn/gtcbbykvbp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xingfuxueyuan.xyz/gthgjesvbq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtkowoganw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtyzmsgboz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gthcntkwpp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jlsjyb.cn/gthhsjvaxw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnxiangtu.top/gtipfgvksb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.feifeiyinyue.top/gtwrtnwpyr.html

[E02] 重复字符串
来源：http://hz.cheryme.top/gtruuodnng.html

Py:   "ab" * 3
来源：http://hz.tanke756.top/gtnpkxmahq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yvedp.cn/gtdqptpjnd.html

JS:   "ab".repeat(3)
来源：http://hz.chenzaomai.com/gtsicdammv.html

TS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtxhvgyppd.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtwqmezbbx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.vqdsnc.cn/gtlzjefpfg.html

Ruby: "ab" * 3
来源：http://hz.gogol.net.cn/gthshunsyd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangdashe.top/gtzzohgfuu.html

[E03] 截取子串
来源：http://hz.havefunace.top/gtwmgmahni.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gtynpecrow.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pycfn.com/gtjrcpmoyt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hongshengwenyu.top/gtgbpiyamp.html

TS:   s.slice(1, 4)
来源：http://hz.guannengcc.top/gtkltgbyzc.html

Java: s.substring(1, 4)
来源：http://hz.shuidangran.top/gtzzgkvnpt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.316326.xyz/gtqmijamjh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hywenlv.cn/gtauyumcaw.html

C#:   s.Substring(1, 3)
来源：http://hz.yuxming.cn/gtjcqfklql.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gteifowbvw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgfzy.top/gtaeuyvprk.html

PHP:  strpos($s, "x");
来源：http://hz.kuanghao11.cn/gtrsifqvkg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sxryk.cn/gteehnkark.html

TS:   s.indexOf("x")
来源：http://hz.iojbl.cn/gtkzkqmjqj.html

Java: s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gttjyqcaxl.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gtrbaqxlwv.html

Ruby: s.index("x")
来源：http://hz.nwbrower.top/gtkntylpow.html

C#:   s.IndexOf("x")
来源：http://hz.cheryme.top/gtufpfalnt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangdashe.top/gtztzkvplz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.wangdashe.top/gtooxkcxfz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenjidiqi.icu/gtqadtagao.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtibkdvwpk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtaplkiwzv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtxkpgqxwi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnxiangtu.top/gtmwldbxkt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigfzy.top/gtpcqsthou.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hammf.cn/gtoqlwjoix.html

[E06] 替换子串
来源：http://hz.quarkkingdee.top/gtlyzkxeka.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gogol.net.cn/gtcviraflm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtbavnsldl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtbzxhcdba.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtlvurvekn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtqbjeucca.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gthdbvkrln.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zycfv.cn/gtpazwboge.html

C#:   s.Replace("a", "b")
来源：http://hz.kuanghao11.cn/gtikehjril.html

[E07] 按分隔符拆分
来源：http://hz.zhixingplan.top/gtebbzddja.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.snrcjt.cn/gtnkmnnsig.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pengpengdd.cyou/gtkhrndcke.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gaohongyu789.top/gtgnfqupsx.html

TS:   s.split(",")
来源：http://hz.gotoacloud.top/gtxxfgqlmt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhijiandao.cn/gtbsffxjmu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yvedp.cn/gtfzayvylv.html

Ruby: s.split(",");  s.split
来源：http://hz.pengpengdd.cyou/gtsyklsqyq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sweek.top/gtfvumzdya.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtcqxrfija.html

Py:   ",".join(items)
来源：http://hz.zdqjudy.top/gtkchdryab.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtrxtphblx.html

JS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtvsosjbss.html

TS:   items.join(",")
来源：http://hz.chenzaomai.com/gtiypkrsss.html

Java: String.join(",", items)
来源：http://hz.yanxiufei.cn/gtqfaxfudd.html

Go:   strings.Join(items, ",")
来源：http://hz.ybcxt.top/gtnkvmwkwz.html

Ruby: items.join(",")
来源：http://hz.jlsjyb.cn/gtqsehgqgi.html

C#:   string.Join(",", items)
来源：http://hz.jqgfzy.top/gtjuhzyedw.html

[E09] 去除所有空白字符
来源：http://hz.9152youxi.cn/gtyzldnqau.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sysykeji.top/gtrvfcaais.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jiagoushi.top/gtrezdsonl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtmggryufv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtlkxtskkv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtjterhjhg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtprtvuwem.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangshuangyany.cn/gtpqukwbmi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.bjfxy.top/gtvcawzpvv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gtbaqvqaym.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xinyue.icu/gtuvoqcefp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhongyouzk.top/gtajcxhbqs.html

JS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtlwrayyez.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtjjngxyxe.html

Java: String.format("%03d", 7)
来源：http://hz.jianghu66.top/gtkzdvhqzo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gzhubu.top/gtmmcipchc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenzaomai.com/gtobgtqdjj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.snrcjt.cn/gtcivrddvm.html

[E11] 反转字符串
来源：http://hz.ehwqpu.com/gtnwtthker.html

Py:   s[::-1]
来源：http://hz.shanyushiyangkeji.top/gtzgxujcxv.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtcfculidn.html

JS:   [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtuflvemvx.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtzzyrwjrn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guowangkeji.top/gtirakalmo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tanke756.top/gtzgncrwul.html

Ruby: s.reverse
来源：http://hz.cheryme.top/gtqvhzmmni.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gtptxmintv.html

[E12] 统计某字符出现次数
来源：http://hz.jqgufenzy.top/gteruqjwes.html

Py:   s.count("a")
来源：http://hz.quarkkingdee.top/gtnkfdzqxf.html

PHP:  substr_count($s, "a");
来源：http://hz.cashguo.top/gtkqeylwkw.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gthhoxmiqc.html

TS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtptztysrj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sweek.top/gtfhqeermk.html

Go:   strings.Count(s, "a")
来源：http://hz.meibo888.top/gtdgvivebd.html

Ruby: s.count("a")
来源：http://hz.sufxvd.cn/gtkyvbsvot.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgfzy.top/gtwhrxrcdj.html

[E13] 逐字符遍历
来源：http://hz.52xcode.cn/gtrubbmrah.html

Py:   for ch in s: print(ch)
来源：http://hz.fzhhl.top/gtaewbzabw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tian-w.cn/gteqnclrrw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtblkngthq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtbajhjknw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhixingplan.top/gtmgrppwsk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj20258.top/gtywlzrkgl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yonumen.top/gtixcanfhm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gtitzdmxlc.html

[E14] URL 编码与 Base64
来源：http://hz.yvedp.cn/gtpauowiyu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hammf.cn/gthkmigfik.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtvekqcvsb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jianghu66.top/gtgnlkmzfk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.0kj1m.cn/gtpkrqqvgl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtcoxzowxe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtcqnbhiyy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jyoumei.cn/gtylqfqsec.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydjk.org.cn/gtjexlzghl.html

[E15] HTML 转义 / 反转义
来源：http://hz.gogol.net.cn/gtpvdelcit.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yvedp.cn/gtifkuhune.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zycfv.cn/gtebteafvo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gaohongyu789.top/gteskjsypt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtmgjjretp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.0kj1m.cn/gtwomrtyuu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtwrgkavnq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xylfe.cn/gtvnxlnpig.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhongyouzk.top/gtyvzdxena.html

[E16] 数字千分位
来源：http://hz.zdqjudy.top/gthjqneyzc.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gttugvsveq.html

PHP:  number_format(1234567);
来源：http://hz.haohaochexian.top/gtazefsvhp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtstdduyxp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtaskdtjdq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtckowvxfw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtmugnlzxs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuanzhike.top/gtafrrqlhf.html

C#:   1234567.ToString("N0")
来源：http://hz.wangdashe.top/gtvfufcidt.html

[E17] 首字母大写
来源：http://hz.jinqigfzy.top/gtoqikexcl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtfynksyor.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuetiantiany.cn/gtaxyyvzob.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtqezdflvb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtrqvktfhv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.feifeiyinyue.top/gtnhsehvsi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jyoumei.cn/gtvihrjsal.html

Ruby: s.capitalize
来源：http://hz.tanke756.top/gtshkbpetb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yongpay.top/gtkcdwcdrp.html

[E18] 模板占位符替换
来源：http://hz.havefunace.top/gtqwclyurw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gtijaoaweg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.iojbl.cn/gtpwkrrigz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtrudaommo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtsozurwhu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj202588.top/gtcfgweeym.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangshuangyany.cn/gtkbmkxsxw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yonumen.top/gtedgyqewv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuanzx.com/gtfngwyhrd.html

[E19] 多行文本按行拆分
来源：http://hz.mhx1999.top/gtusjewfau.html

Py:   s.splitlines()
来源：http://hz.andypj.xyz/gtegbuaqah.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhoulong.xyz/gthsekxpxt.html

JS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtfazhgyop.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gthpgndvqn.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtmzosbymd.html

Go:   strings.Split(s, "\n")
来源：http://hz.iojbl.cn/gtzigpjtvi.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gtjxqefsdo.html

C#:   s.Split('\n')
来源：http://hz.guowangkeji.top/gtjpnfpoah.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtjdleogdq.html

Py:   if not s:
来源：http://hz.haohaochexian.top/gtarntdxua.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinghuilouyu.cn/gtwlwwymys.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yonumen.top/gtimwqwzga.html

TS:   if (s === "") {}
来源：http://hz.shzxlz.cn/gtcbjdldgu.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtfkksmaae.html

Go:   if s == "" {}
来源：http://hz.tian-w.cn/gtmtvkjylh.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtmgnscnwz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sysykeji.top/gteytuyqhi.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gtlokyzjph.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shangyingyoupin.top/gtzozhwspm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cucudq.cn/gtkggrhmcm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gticuheksx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gteqtmlqhx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtruhjzryi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gaohongyu789.top/gthupegydl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pycfn.com/gtpyvywxfz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtutgqhfwq.html

[E22] 字节长度与字符长度
来源：http://hz.xylfe.cn/gtiwuawuxb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jianghu66.top/gtbttqfron.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dashuyun.cn/gtamxwcsjv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yueranfly.top/gtxolwpbdb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtccltaexe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aizwys.cn/gtdmvilbrw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.iojbl.cn/gtkoeyzawc.html

Ruby: s.bytesize;  s.length
来源：http://hz.52xcode.cn/gtkcxdlfff.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shangyingyoupin.top/gtkbykoepz.html

================================================================================
来源：http://hz.0kj1m.cn/gteoyjsfix.html

F. 文件与目录
来源：http://hz.nwbrower.top/gtedjqclje.html

================================================================================
来源：http://hz.gzhubu.top/gtterwnynz.html

[F01] 读取整个文件
来源：http://hz.sufxvd.cn/gtahgtjhfg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fzhhl.top/gtwpxhyvbt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtrgoqgmff.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhijiandao.cn/gtehamtydt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pengpengdd.cyou/gtanfduneh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtfhuvgmas.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.havefunace.top/gtxwmluuqe.html

Ruby: File.read("a.txt")
来源：http://hz.jiagoushi.top/gthelstjjg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dashuyun.cn/gtyjtrsltw.html

[F02] 逐行读取文件
来源：http://hz.daria6918.cn/gtsyqlefca.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.0kj1m.cn/gtihjppzge.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhongyouzk.top/gtgigxricp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtqfusxvtn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtsaszonkp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtfywqunum.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhijiandao.cn/gthknveefo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gthuiizhhf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gthvtelzhl.html

[F03] 写入文件（覆盖）
来源：http://hz.pengpengdd.cyou/gtkkpxodvz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shuidangran.top/gtsolubkba.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.bjfxy.top/gtfhplnqoo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtlsaqtres.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtsyeobfxb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aibaodan.cn/gtdjrgdqix.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gotoacloud.top/gtelgpeiwl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gtcwtjdbek.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtzgkqptfs.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtrokstxzi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tianlin.xyz/gtpssynlna.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gthmybsnst.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtdarorfku.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtusbspftn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pycfn.com/gtvzrnvnyt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aibaodan.cn/gtnzibundw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jiagoushi.top/gtoyoxnubc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxuanxn.top/gtgpgiqrau.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuanzhike.top/gtmomnctbg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.c1oappe.top/gtwsicfjng.html

PHP:  file_exists("a.txt");
来源：http://hz.zhijiandao.cn/gtiqosdthy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtlavynwhc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtxymyophg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtvaujjeee.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtyuomuvmb.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258.top/gtnilpwohc.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtgsoscluc.html

[F06] 删除文件
来源：http://hz.9152youxi.cn/gttisyogmo.html

Py:   os.remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtzskpskdw.html

PHP:  unlink("a.txt");
来源：http://hz.jqgfzy.top/gtjbsmlcdx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtcpimogdr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtonavhibd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtpuingliz.html

Go:   os.Remove("a.txt")
来源：http://hz.yuanzhike.top/gtdrrvbiwi.html

Ruby: File.delete("a.txt")
来源：http://hz.smart0.xyz/gtaetwwuju.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtvcfjhezi.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gttwxwftgt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gttbycwrdg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuxming.cn/gtitskhqaw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtooicyhrm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtyhsebnmd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtgaqjisax.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnxiangtu.top/gtsqhllovh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.bjfxy.top/gtsamoclfo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigufen.top/gtlhfqmpwu.html

[F08] 遍历目录
来源：http://hz.cdnleiting.top/gtcxzpbuyn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gtdgetaujz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.vqdsnc.cn/gtbxwyyvzs.html

JS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtjchslecy.html

TS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangtech.top/gtcjbuzdgt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.birdmap.top/gthrtuquyw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daxiang520.top/gtjewsnicf.html

Ruby: Dir.children("dir")
来源：http://hz.xingfuxueyuan.xyz/gtazuuaegh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtevisoigo.html


<!-- 参考信息 -->