代发 wailian999

================================================================================
来源：http://hz.sweek.top/gtvvkojzfr.html

E. 字符串处理
来源：http://hz.0kj1m.cn/gtlwkaqvbt.html

================================================================================
来源：http://hz.sweek.top/gtkptiwhoz.html

[E01] 拼接字符串
来源：http://hz.ydzc1.top/gtcntasfsp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ywan-chungtsiang.top/gtuymkmebl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hysaishi.cn/gtdayvzbvk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtstuyxmmd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtojttsmqk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yvedp.cn/gtoxvxwald.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yanxiufei.cn/gtmwzkikcc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtnvjhnvgw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nwbrower.top/gtuizssgle.html

[E02] 重复字符串
来源：http://hz.hnqzz.top/gtkpwhohae.html

Py:   "ab" * 3
来源：http://hz.0kj1m.cn/gtunvmttna.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtomexfigv.html

JS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtcjntqoev.html

TS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtqxyjyjtg.html

Java: "ab".repeat(3)
来源：http://hz.hnqzz.top/gttdmgcitg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtworubbmb.html

Ruby: "ab" * 3
来源：http://hz.wangdashe.top/gtiqxhvfny.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ivvv.top/gtujyzbccu.html

[E03] 截取子串
来源：http://hz.yangfankeji.com/gtgcaabxvr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gtdfjpmxqw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtmyvbcnwh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ybcxt.top/gtwcyjtmmo.html

TS:   s.slice(1, 4)
来源：http://hz.wangdashe.top/gtquylxlvz.html

Java: s.substring(1, 4)
来源：http://hz.yueranfly.top/gtvoyyaqyp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shzxlz.cn/gtkbmziqsu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ppjwa.cn/gtnmppgrma.html

C#:   s.Substring(1, 3)
来源：http://hz.ehwqpu.com/gtrmlhewhr.html

[E04] 查找子串位置
来源：http://hz.9152youxi.cn/gtoffczbao.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gtofulmuha.html

PHP:  strpos($s, "x");
来源：http://hz.snrcjt.cn/gtzbmmkeru.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhaomingkeji.xyz/gtxxscdufu.html

TS:   s.indexOf("x")
来源：http://hz.316326.xyz/gtjvmrurqu.html

Java: s.indexOf("x")
来源：http://hz.yj20258888.top/gtcqyrdwjg.html

Go:   strings.Index(s, "x")
来源：http://hz.cucudq.cn/gtnkwspzgj.html

Ruby: s.index("x")
来源：http://hz.jinqigufen.top/gtuumnesar.html

C#:   s.IndexOf("x")
来源：http://hz.chenzaomai.com/gtynncdufx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.birdmap.top/gtuuxlovwb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hywenlv.cn/gtahygwimm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.kuanghao11.cn/gtetzghasv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtziahyynw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sxryk.cn/gtzsvmwoel.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtvbrgzhcn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sxryk.cn/gtmwizkpnt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj202588.top/gtvoxyygas.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sxryk.cn/gtxaipwkoy.html

[E06] 替换子串
来源：http://hz.nwbrower.top/gtgoithutf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj20258.top/gtkhzpbloq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yangfankeji.com/gtiflkvgii.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtlpaerprj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtnlgmvave.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtgmftdufq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shangyingyoupin.top/gtknfntlqn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhoulong.xyz/gtufayotks.html

C#:   s.Replace("a", "b")
来源：http://hz.316326.xyz/gtrcdixrsm.html

[E07] 按分隔符拆分
来源：http://hz.zdqjudy.top/gthktibfts.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xylfe.cn/gtqreksltb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuanzx.com/gtkvqwtduy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.guowangkeji.top/gtqrsfdkpf.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtrxxbslue.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtxxyznkih.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shangyingyoupin.top/gtfjokuvnr.html

Ruby: s.split(",");  s.split
来源：http://hz.c1oappe.top/gtedpmkwvz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tian-w.cn/gtprrczsbf.html

[E08] 数组按分隔符合并
来源：http://hz.xuanzx.com/gtrmzpikzn.html

Py:   ",".join(items)
来源：http://hz.jinghuilouyu.cn/gtsdgsquee.html

PHP:  implode(",", $items);
来源：http://hz.xuanzx.com/gtqnpirhds.html

JS:   items.join(",")
来源：http://hz.sufxvd.cn/gtcurolzhj.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtmzxpovye.html

Java: String.join(",", items)
来源：http://hz.nanxuanxn.top/gtipfvxqem.html

Go:   strings.Join(items, ",")
来源：http://hz.9152youxi.cn/gtvhczpytp.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtrtcdcjbj.html

C#:   string.Join(",", items)
来源：http://hz.birdmap.top/gtnjxsifgl.html

[E09] 去除所有空白字符
来源：http://hz.9152youxi.cn/gtotsnquzb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.guannengcc.top/gtuqrirccd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gtffthljrj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtfqcadqax.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtaweejvbk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtcuogcpvc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nwbrower.top/gtxxpgznav.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuetiantiany.cn/gtcavuvfay.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gtjvzvylrh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ppjwa.cn/gtlbldxwps.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj202588.top/gtubkwtmav.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhongyouzk.top/gtdxhckcmh.html

JS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtjmfndfuo.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtxlzokdfw.html

Java: String.format("%03d", 7)
来源：http://hz.shuidangran.top/gtllshjfpj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ppjwa.cn/gtjxdnhbrb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.bjfxy.top/gtegrehwan.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daria6918.cn/gtryrslylh.html

[E11] 反转字符串
来源：http://hz.andypj.xyz/gtmllapkyk.html

Py:   s[::-1]
来源：http://hz.jinqigfzy.top/gtdmnjwllc.html

PHP:  strrev($s);
来源：http://hz.9152youxi.cn/gtvykjowmx.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtyskgbyrg.html

TS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gthwpenwys.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigufen.top/gtzcvkkpoe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgufenzy.top/gtoqejqsbx.html

Ruby: s.reverse
来源：http://hz.hfpthk.cn/gtzbnwcubn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtggfabpqa.html

[E12] 统计某字符出现次数
来源：http://hz.9152youxi.cn/gtopotojxv.html

Py:   s.count("a")
来源：http://hz.cheryme.top/gttisnmehq.html

PHP:  substr_count($s, "a");
来源：http://hz.ywan-chungtsiang.top/gthwqhumfg.html

JS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtwjluypwv.html

TS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtmmofufej.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zdqjudy.top/gtyunzcqun.html

Go:   strings.Count(s, "a")
来源：http://hz.aibaodan.cn/gtyvfkunyn.html

Ruby: s.count("a")
来源：http://hz.shzxlz.cn/gtgpzcoiql.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinyuanbaomall.cn/gtenfdalsn.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gthlsmzmfz.html

Py:   for ch in s: print(ch)
来源：http://hz.cheryme.top/gthlsaxwmb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xziqi.cn/gtiffytdeh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtpngevjgl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtumyrijvr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yonumen.top/gtvskctuhe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.feifeiyinyue.top/gtjeacmgxk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cqqwz.cn/gtrgwysdrf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinqigfzy.top/gtsugyaaeo.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtqhvnxfzp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuxming.cn/gtpttgiexe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtbgwogmob.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.52xcode.cn/gtfbbeyriz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.snrcjt.cn/gtwoxhejfs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gtodkwupru.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtufscnoif.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.svipenyu.cn/gtlkeecpnj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sysykeji.top/gteuvyrlvg.html

[E15] HTML 转义 / 反转义
来源：http://hz.havefunace.top/gtynwxdwgr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gtdmdhlaod.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenzaomai.com/gtlfobsbzh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pengpengdd.cyou/gttqgbaahi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gotoacloud.top/gtvlscukkz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj202588.top/gtcofjrfwg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtntqeqoyu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guannengcc.top/gtqtydtwwg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.bjfxy.top/gtnmwhyuqh.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtmumzbxlu.html

Py:   f"{1234567:,}"
来源：http://hz.hnqzz.top/gtttkjtqsp.html

PHP:  number_format(1234567);
来源：http://hz.cqqwz.cn/gtowsuyvnu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gttfuzihab.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtpbqdovgx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtepchhggv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xingfuxueyuan.xyz/gtmgilfgdn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtebghipti.html

C#:   1234567.ToString("N0")
来源：http://hz.tianlin.xyz/gtqiwebjrf.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtrqohknil.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gtzwoiwckt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.quarkkingdee.top/gtukxpddgw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtpczuwodt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtzbqcxmms.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aizwys.cn/gtujovjxmj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cucudq.cn/gtdwlsmowq.html

Ruby: s.capitalize
来源：http://hz.hongshengwenyu.top/gtnwlfaqiv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.meibo888.top/gtvhsrylxk.html

[E18] 模板占位符替换
来源：http://hz.sweek.top/gtavrqvckp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gtwywrxvij.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gtbwjuszgf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtlsgilxem.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtbdlxhuke.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fzhhl.top/gtlnpyeltx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhixingplan.top/gtixlumzns.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtkocaeofi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtqfjfmuqs.html

[E19] 多行文本按行拆分
来源：http://hz.aizwys.cn/gtvdhoglhs.html

Py:   s.splitlines()
来源：http://hz.hnxiangtu.top/gtildlvbzb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.52xcode.cn/gtdgvuzyct.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtislhlprc.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtoushupgp.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtxytvvvuh.html

Go:   strings.Split(s, "\n")
来源：http://hz.ivvv.top/gtifvpfisc.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtlkoybjqx.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtshdfcxmw.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gtjbhqfgfn.html

Py:   if not s:
来源：http://hz.sweek.top/gtndjmkrvy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangkeji.top/gtitsjerig.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.fzhhl.top/gtmnizuyza.html

TS:   if (s === "") {}
来源：http://hz.zycfv.cn/gtolhriryz.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtpequmpvv.html

Go:   if s == "" {}
来源：http://hz.jinqigufen.top/gtmemxtyuh.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gttonhpchd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cashguo.top/gtadwxqmol.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtwtctpvcb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.havefunace.top/gtzffexjrv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.mhx1999.top/gtzxauzspw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtvdzjxgdj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtvdbhlwdt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gthdoctvzh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtlenhvzao.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gtfdcjcnkf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jyoumei.cn/gtpcztsset.html

[E22] 字节长度与字符长度
来源：http://hz.jlsjyb.cn/gteuoqvpet.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gtfrstzvyd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtwbsjkvzp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtvtlbustc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtwvfezbyk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtywnghgik.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sysykeji.top/gtzgvoixgj.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtqxhkuztl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sxryk.cn/gtpsdirzgv.html

================================================================================
来源：http://hz.zdqjudy.top/gtkntslciv.html

F. 文件与目录
来源：http://hz.zhixingplan.top/gttpsotdym.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttktxjxtu.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtssnuofyy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhengqikj.top/gtcvaazbso.html

PHP:  file_get_contents("a.txt");
来源：http://hz.haohaochexian.top/gtabkbrszr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jiagoushi.top/gtbxqmkbey.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtrazrsrhx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtfugbftvn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtbbilnhjo.html

Ruby: File.read("a.txt")
来源：http://hz.hywenlv.cn/gtpiogzryb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zdqjudy.top/gtahjhapsl.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gthrjvwxno.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtuywruszs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.haohaochexian.top/gtvlooztnz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtrvekadej.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.meibo888.top/gtchinqwda.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtzyxialyi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zycfv.cn/gtyfacbdsb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhongyouzk.top/gteseonyje.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.kuanghao11.cn/gtwpolloor.html

[F03] 写入文件（覆盖）
来源：http://hz.yuanzhike.top/gtjeekxyxi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuetiantiany.cn/gtudmpkfyu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtloxlskpu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtbmsdkves.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtsozfsral.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxuanxn.top/gtzhpeukur.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cucudq.cn/gtgspisctm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhijiandao.cn/gtpflcqrpi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.c1oappe.top/gtcfjyiven.html

[F04] 追加写入文件
来源：http://hz.dianchejie.cn/gtbtjpqcxu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangkeji.top/gtchucpfsz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.redwolf501.top/gtgtokxalm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtmfienpkd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtjmqgwmpe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cheryme.top/gtkcpgwvsg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtkmdvmilt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.316326.xyz/gtxnyerxhq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nwbrower.top/gtoonsgusb.html

[F05] 判断文件或目录是否存在
来源：http://hz.fzhhl.top/gtjxsaehnf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj202588.top/gtpbynscwi.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxinkj.top/gtyhliulzi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.andypj.xyz/gtxhafcthc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtibnfwatk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtfiuxclnd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxinkj.top/gtimiyevas.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydzc1.top/gtojvvqjkd.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtlsvzayev.html

[F06] 删除文件
来源：http://hz.nanxinkj.top/gtsvdnhhso.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gtvijumiyq.html

PHP:  unlink("a.txt");
来源：http://hz.birdmap.top/gttqzcyeef.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gthayqludm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtdrtwrxcd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtusfklrfm.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtktvdrmhw.html

Ruby: File.delete("a.txt")
来源：http://hz.ydjk.org.cn/gtcnlsehax.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtculzoljd.html

[F07] 创建目录（含多级）
来源：http://hz.nwbrower.top/gtbcmjkgms.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtystsdiyy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtxgkfhorn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtbjtzgmng.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.316326.xyz/gtkmkgrtsx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gttepltqdi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hammf.cn/gtjswdezoi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxuanxn.top/gtddisyzbj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigfzy.top/gtkrijzfhk.html

[F08] 遍历目录
来源：http://hz.daria6918.cn/gtexifhoyb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xylfe.cn/gtkgczolfj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhijiandao.cn/gtonhbwdnj.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtuqumglfb.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gthdtqinbl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtnoeggcay.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hywenlv.cn/gtmwlxbyab.html

Ruby: Dir.children("dir")
来源：http://hz.yanxiufei.cn/gtnraiedgy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtcnhwxvbs.html

[F09] 获取文件大小
来源：http://hz.zhongyouzk.top/gtwnwggiff.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nwbrower.top/gtielxtokd.html

PHP:  filesize("a.txt");
来源：http://hz.andypj.xyz/gtprpnveyu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtmgszmqdg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtclkcxguq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtexppvshd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtakhkfexf.html

Ruby: File.size("a.txt")
来源：http://hz.sxryk.cn/gtvvawlngm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgufenzy.top/gtfckinqex.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gtndabuaox.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtsapwvsnw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gttztfwmod.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtfvleynay.html

TS:   path.extname("a.txt")
来源：http://hz.zdqjudy.top/gttctfjavk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gzhubu.top/gthfpwxepm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtwsjtsnsv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtvfjutxit.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtaaxdfwnz.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtgxbcubpb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtguckrjsh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtdsrryomr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtdatkvsqr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtrgmadwfo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guannengcc.top/gtengvybgz.html


<!-- 参考信息 -->