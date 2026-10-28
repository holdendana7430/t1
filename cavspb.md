代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sufxvd.cn/gtvmhskqpr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ywan-chungtsiang.top/gtdxabwtay.html

[D25] Set 集合去重与交并差
来源：http://hz.yvedp.cn/gtfstzdqvb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cdnleiting.top/gtjjldboib.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.andypj.xyz/gtnmmxenim.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shzxlz.cn/gtudehaqod.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gtabpkfeap.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.c1oappe.top/gtdjigufxw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yvedp.cn/gtspyyibsz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtvvvhzncu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xinyue.icu/gtodyzdosq.html

[D26] 数组转字符串
来源：http://hz.hongshengwenyu.top/gtesvfyxjo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tanke756.top/gterdfsypo.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangkeji.top/gtlbawxwdm.html

JS:   arr.join(", ")
来源：http://hz.ivvv.top/gtoujjanbc.html

TS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtpbrhijtb.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtxeeijrvi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.c1oappe.top/gtifuvtaoq.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gtlmcnelcm.html

C#:   string.Join(", ", list)
来源：http://hz.snrcjt.cn/gtccipipez.html

================================================================================
来源：http://hz.zhoulong.xyz/gtahgdosif.html

E. 字符串处理
来源：http://hz.cqqwz.cn/gtuijasqkb.html

================================================================================
来源：http://hz.316326.xyz/gtixoxxscz.html

[E01] 拼接字符串
来源：http://hz.yonumen.top/gtrzyxqcny.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxuanxn.top/gtwzmtvgid.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtcmeenrdp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtudlypcvx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gtigbfnavo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtlyylizdm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aizwys.cn/gtogawonlb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.bjfxy.top/gtwsdwpngz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yvedp.cn/gtcaufodwp.html

[E02] 重复字符串
来源：http://hz.zhoulong.xyz/gtgihhvxex.html

Py:   "ab" * 3
来源：http://hz.yueranfly.top/gtrpiuizyz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.haohaochexian.top/gtcipcclcb.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtrguhfpza.html

TS:   "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtzvyjbvrm.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtexxpogxt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtfpqkszvr.html

Ruby: "ab" * 3
来源：http://hz.andypj.xyz/gtpufmiwuy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gtrcvmzdqv.html

[E03] 截取子串
来源：http://hz.9152youxi.cn/gtyruerxxd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.0kj1m.cn/gtlgnxraqa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtweqnrajz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ydzc1.top/gtwrgqsgat.html

TS:   s.slice(1, 4)
来源：http://hz.wangdashe.top/gtfpgfkgri.html

Java: s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtuzrcynrs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj202588.top/gtwjzczmzq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.kuanghao11.cn/gtwvirqvtj.html

C#:   s.Substring(1, 3)
来源：http://hz.jiagoushi.top/gtpeqehxlf.html

[E04] 查找子串位置
来源：http://hz.yangfankeji.com/gtcoarxiee.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtlbsicwoz.html

PHP:  strpos($s, "x");
来源：http://hz.yanxiufei.cn/gtjbhnlfom.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.iojbl.cn/gtoeztzkiw.html

TS:   s.indexOf("x")
来源：http://hz.zdqjudy.top/gtxcsobgpa.html

Java: s.indexOf("x")
来源：http://hz.yongpay.top/gttvrxksvo.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtztmrhrjx.html

Ruby: s.index("x")
来源：http://hz.yangfankeji.com/gttktfrutk.html

C#:   s.IndexOf("x")
来源：http://hz.cucudq.cn/gtzkmyxgug.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ehwqpu.com/gtwjtgbvaz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shzxlz.cn/gtxsnjgxcc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sufxvd.cn/gtaeddreem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtsfcwkdqm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.haohaochexian.top/gthhpxsytl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtgnhwupxh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shuidangran.top/gtlflqvldk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhijiandao.cn/gtbbviuchc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtsqnenxss.html

[E06] 替换子串
来源：http://hz.xziqi.cn/gtofeamicx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yonumen.top/gtvdpmzggo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuetiantiany.cn/gtqegcrrkr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtkvbcnmvp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtjxrjzumm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtyeuszqwe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgfzy.top/gtdxyduddw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jiagoushi.top/gttxlrpjeg.html

C#:   s.Replace("a", "b")
来源：http://hz.yj20258.top/gtjherxzav.html

[E07] 按分隔符拆分
来源：http://hz.zhoulong.xyz/gtqrkuwqie.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yvedp.cn/gtywrraxuy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tanke756.top/gtfypdjgdq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jianghu66.top/gtimdgsoxs.html

TS:   s.split(",")
来源：http://hz.hnqzz.top/gthstocxis.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gtvedocpen.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zdqjudy.top/gtkcyvaebx.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtrfoosjzd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.bjfxy.top/gtghefabwv.html

[E08] 数组按分隔符合并
来源：http://hz.jiagoushi.top/gtlulndqmj.html

Py:   ",".join(items)
来源：http://hz.haohaochexian.top/gtifotuhdr.html

PHP:  implode(",", $items);
来源：http://hz.cheryme.top/gteadozuai.html

JS:   items.join(",")
来源：http://hz.jlsjyb.cn/gteehzolis.html

TS:   items.join(",")
来源：http://hz.cashguo.top/gtimhzfznh.html

Java: String.join(",", items)
来源：http://hz.chenlongwang.top/gtrnykkmuz.html

Go:   strings.Join(items, ",")
来源：http://hz.jinyuanbaomall.cn/gtfmyqusfv.html

Ruby: items.join(",")
来源：http://hz.cucudq.cn/gtkqpsdaal.html

C#:   string.Join(",", items)
来源：http://hz.dianchejie.cn/gtledklruj.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gtxhbmokfi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xziqi.cn/gtknxvzryt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jiagoushi.top/gtstgqoldz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtcskusrvu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtfeggzunb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhengqikj.top/gtjvqibpim.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.mhx1999.top/gtwtzzqgzn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gtbjsgvqut.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cdnleiting.top/gtzmlidmda.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhengqikj.top/gtihnebhid.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pycfn.com/gtkdegoxdy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhijiandao.cn/gtxtolyscd.html

JS:   "7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtayvnpuob.html

TS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtedkkaqsl.html

Java: String.format("%03d", 7)
来源：http://hz.52xcode.cn/gtrbhlybev.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jlsjyb.cn/gtxizbxytg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtcbuqutdh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gtmdfskjvu.html

[E11] 反转字符串
来源：http://hz.fengsongda.top/gtqqgdmpfo.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtoafdfjry.html

PHP:  strrev($s);
来源：http://hz.52xcode.cn/gtwzigjokx.html

JS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gtetxjinvf.html

TS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtnsoynewl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtwysovkui.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtkbomziqk.html

Ruby: s.reverse
来源：http://hz.hammf.cn/gtqsydvsqw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gthsnnqjkx.html

[E12] 统计某字符出现次数
来源：http://hz.hongshengwenyu.top/gtxtpecbmd.html

Py:   s.count("a")
来源：http://hz.gogol.net.cn/gtbpfbwwaj.html

PHP:  substr_count($s, "a");
来源：http://hz.cucudq.cn/gthgurqahb.html

JS:   s.split("a").length - 1
来源：http://hz.ydjk.org.cn/gtntvbvwlv.html

TS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtbughtrti.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgfzy.top/gtxacfbwld.html

Go:   strings.Count(s, "a")
来源：http://hz.hywenlv.cn/gttoccgnvb.html

Ruby: s.count("a")
来源：http://hz.yonumen.top/gtexvjprop.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnqzz.top/gtquswcqbd.html

[E13] 逐字符遍历
来源：http://hz.hnqzz.top/gtvsgltbgr.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtdpwardln.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangshuangyany.cn/gtcipqztwd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnqzz.top/gtclhjkbjh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtlddfybih.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhongyouzk.top/gtngvsvjxx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pycfn.com/gtcdkkswvd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtvlpbjvwa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tian-w.cn/gtmdiaxgbx.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtkxjmeziw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gogol.net.cn/gtwxsdalts.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.redwolf501.top/gtavmrszig.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangdashe.top/gtomwtshyr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xylfe.cn/gtcgpcuszu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258.top/gtbysqbmzh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtjyhebzpm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gtwqedxnmz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.0kj1m.cn/gtphhdxmwe.html

[E15] HTML 转义 / 反转义
来源：http://hz.feifeiyinyue.top/gtzojmkakl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtwgxjqfnp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.dianchejie.cn/gtvrfdvisp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.c1oappe.top/gtfqkhcdnd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtzqzwhsyk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtvzikmnkk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhiwuduotai.top/gtfbknsvyo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhijiandao.cn/gtpcgmigam.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shangyingyoupin.top/gtadzdikgo.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gtncaywwzd.html

Py:   f"{1234567:,}"
来源：http://hz.pengpengdd.cyou/gttaybrqxo.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gtszltlqar.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.dashuyun.cn/gtwnskcqkt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtjuucvvue.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gtbcgrpoau.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtjwcyodrh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gogol.net.cn/gtefcwtgih.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxuanxn.top/gtxmbwuqkt.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtinvybzzl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtonchatzm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gtddbefrlp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.havefunace.top/gtvejswtgm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gtvjhmdtqh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cqqwz.cn/gtqmbrzdbq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhengqikj.top/gtbsoidxkv.html

Ruby: s.capitalize
来源：http://hz.shuidangran.top/gtrcsaunhc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhoulong.xyz/gtvaqeymbr.html

[E18] 模板占位符替换
来源：http://hz.jinqigfzy.top/gtqiojasnd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuanzhike.top/gtczvvmnad.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jyoumei.cn/gtkngdtbrk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtwoxxltdp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtpyalwkea.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.smart0.xyz/gtyetbxltf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.0kj1m.cn/gtxpgrbfxq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xziqi.cn/gtshjaplnq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.wangdashe.top/gtwudewqag.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtfpjbgirq.html

Py:   s.splitlines()
来源：http://hz.haohaochexian.top/gtvsgpeanp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ybcxt.top/gthiiaddor.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtzvtbkfim.html

TS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtddarmuqm.html

Java: s.lines().toList()
来源：http://hz.jyoumei.cn/gtfmoraxff.html

Go:   strings.Split(s, "\n")
来源：http://hz.9152youxi.cn/gtinnsmdif.html

Ruby: s.lines
来源：http://hz.andypj.xyz/gtpzrdayxb.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtvqcwadox.html

[E20] 判断字符串是否为空
来源：http://hz.fzhhl.top/gthclgoqyp.html

Py:   if not s:
来源：http://hz.zhoulong.xyz/gtdfmssjvz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ehwqpu.com/gtyrzvkrde.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xylfe.cn/gthhqkhrpm.html

TS:   if (s === "") {}
来源：http://hz.yj20258.top/gttecakvia.html

Java: if (s.isEmpty()) {}
来源：http://hz.shangyingyoupin.top/gtnuzgshxx.html

Go:   if s == "" {}
来源：http://hz.xuetiantiany.cn/gtglxdhnss.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtyokyzopn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xziqi.cn/gtbdbawfkl.html

[E21] 超长截断加省略号
来源：http://hz.birdmap.top/gtembugzdb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jiagoushi.top/gtokuwmmhy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gotoacloud.top/gtsttgumur.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtljfepore.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtmtopbxfj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtsvzkcaam.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtbqefbuny.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.bjfxy.top/gtrkhznalw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhiwuduotai.top/gtnacpifaa.html

[E22] 字节长度与字符长度
来源：http://hz.hnxiangtu.top/gtwmkuopjk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.feifeiyinyue.top/gtcyvpwpmp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtswctwzwf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtkbcfptwv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtlvzvrcsp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigfzy.top/gtxtcvzmbi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtzxykdlqb.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtpmdyclbq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gtigjrvfxi.html

================================================================================
来源：http://hz.cucudq.cn/gtsrwobqgk.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtwvmdrnbk.html

================================================================================
来源：http://hz.hnqzz.top/gtlscfitex.html

[F01] 读取整个文件
来源：http://hz.birdmap.top/gtbaeovcgh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sufxvd.cn/gtggpasifi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cashguo.top/gtwretqvat.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gttvvofqfa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtgdjofinw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtqgboopvd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shangyingyoupin.top/gtibdeztxu.html

Ruby: File.read("a.txt")
来源：http://hz.guannengcc.top/gtfywbahmv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtedbqpxkf.html

[F02] 逐行读取文件
来源：http://hz.yuxming.cn/gtdwtiohvj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cucudq.cn/gtuglulmrv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtyhkwqzpc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtvpnrllot.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtfwoddsyc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtjikvohnl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yonumen.top/gtenebafla.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pengpengdd.cyou/gtvlyvopby.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jianghu66.top/gtfprkjwok.html

[F03] 写入文件（覆盖）
来源：http://hz.aizwys.cn/gtlzlzkano.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.smart0.xyz/gtdalxlmdd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtiaarpjgp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtqssjmwgl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtugkhacpq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxuanxn.top/gtcqmtimxg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gzhubu.top/gtionffrmi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cashguo.top/gthyftakar.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ivvv.top/gtjjiciitb.html

[F04] 追加写入文件
来源：http://hz.yj202588.top/gtjheowtul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zycfv.cn/gtgcbpiqiu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cashguo.top/gtlekxkrwg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtfhbxyddl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtwwxpiybf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gtyyfrhnli.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hammf.cn/gtlzvpjvav.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shzxlz.cn/gttjugtfjx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtrmllyisq.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtjslimzqa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.birdmap.top/gtkagxwysc.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtalemfexd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtngkqubmi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtmyfnilby.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtuucbuvyz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtyyziqoju.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhijiandao.cn/gtirzfexyt.html

C#:   File.Exists("a.txt")
来源：http://hz.quarkkingdee.top/gtzcnaczbb.html

[F06] 删除文件
来源：http://hz.yueranfly.top/gtgbwbfaxi.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtxvpenzgg.html

PHP:  unlink("a.txt");
来源：http://hz.ivvv.top/gtxxcxdnrh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtefujgchk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gttcbjmcfx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtbslymqge.html

Go:   os.Remove("a.txt")
来源：http://hz.yongpay.top/gtkskjdefr.html

Ruby: File.delete("a.txt")
来源：http://hz.fengsongda.top/gtysxpwenc.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtdkmzmfsk.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258888.top/gtntkfnugt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dianchejie.cn/gtvpubqmgk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gogol.net.cn/gtxfdbqfgl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtpmehqxjc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangkeji.top/gtyzjoknop.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinghuilouyu.cn/gtgpgtxysv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shanyushiyangtech.top/gtebhvibac.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.smart0.xyz/gtwrbcddou.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.bjfxy.top/gthnwsuxrq.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtiarehkel.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xinyue.icu/gtiqscshem.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cucudq.cn/gtxfqsnitq.html

JS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtwggkomhw.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtfmcehmfe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtszrnotrr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zycfv.cn/gtyzssgtdv.html

Ruby: Dir.children("dir")
来源：http://hz.hysaishi.cn/gttwoizatp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtbacjywoj.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gtahigfkco.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtzvhexydy.html

PHP:  filesize("a.txt");
来源：http://hz.wangdashe.top/gtcbathdxb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtazxxdjce.html


<!-- 参考信息 -->