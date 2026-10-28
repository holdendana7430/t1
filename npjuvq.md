代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gtyzxajizk.html

[D24] 字典 / Map 基本操作
来源：http://hz.yvedp.cn/gtdsxjldyc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtddippxwb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnxiangtu.top/gtzhruwmak.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yangfankeji.com/gtgpqigrsz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jlsjyb.cn/gtqomjwlia.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuxming.cn/gtdimgeuaj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.birdmap.top/gteurwqyzf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtszfgjdsa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj202588.top/gtzcsrrjta.html

[D25] Set 集合去重与交并差
来源：http://hz.hnqzz.top/gtgwjprdht.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtxulsdrrs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yueranfly.top/gtejgntzft.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cucudq.cn/gttrngseer.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangkeji.top/gtclskkmji.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gttwbezxeh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhengqikj.top/gtmpsxocef.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhengqikj.top/gtncufwahj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.316326.xyz/gtwmgaesuf.html

[D26] 数组转字符串
来源：http://hz.aizwys.cn/gtmnmfrkek.html

Py:   ", ".join(map(str, arr))
来源：http://hz.svipenyu.cn/gtpockgsrg.html

PHP:  implode(", ", $arr);
来源：http://hz.jinghuilouyu.cn/gtipvmzoov.html

JS:   arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtzpfuqfnx.html

TS:   arr.join(", ")
来源：http://hz.xziqi.cn/gttkwpnmvr.html

Java: String.join(", ", list)
来源：http://hz.fzhhl.top/gtejfintql.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtmeogwbib.html

Ruby: arr.join(", ")
来源：http://hz.yonumen.top/gtgjcveodh.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtkvlqqeip.html

================================================================================
来源：http://hz.jlsjyb.cn/gthkbxjntn.html

E. 字符串处理
来源：http://hz.vqdsnc.cn/gtovzwdaav.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjkspkaje.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gtnijkclym.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtbdnvfcdx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sweek.top/gtrmbsqohk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtnllvfzpe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtrgaahpvi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtbmhsdupl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnqzz.top/gtpiiwjpak.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hfpthk.cn/gtnbusgwhn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gzhubu.top/gtticycwel.html

[E02] 重复字符串
来源：http://hz.pycfn.com/gthnjwnjem.html

Py:   "ab" * 3
来源：http://hz.jyoumei.cn/gtcfxeufaz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtmxuzhqse.html

JS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gttmqzidkw.html

TS:   "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtivuvvods.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gtaubbtykn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shzxlz.cn/gtufwkxhmc.html

Ruby: "ab" * 3
来源：http://hz.xuetiantiany.cn/gtvqljhcqc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gaohongyu789.top/gtsckhcocg.html

[E03] 截取子串
来源：http://hz.shanyushiyangtech.top/gtjzlzcdtu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tianlin.xyz/gtblehnydm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.redwolf501.top/gtdzurklnn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtgsymdvib.html

TS:   s.slice(1, 4)
来源：http://hz.zhengqikj.top/gtbmybdmvs.html

Java: s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtuuvmyuqo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhixingplan.top/gtvrmukmlv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yueranfly.top/gtcrjgohca.html

C#:   s.Substring(1, 3)
来源：http://hz.shuidangran.top/gtyirvnutl.html

[E04] 查找子串位置
来源：http://hz.yuxming.cn/gtkvnxwylz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtnmaevzqq.html

PHP:  strpos($s, "x");
来源：http://hz.mhx1999.top/gtbbbamzjg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hongshengwenyu.top/gtjkjvqytg.html

TS:   s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtygweffta.html

Java: s.indexOf("x")
来源：http://hz.hysaishi.cn/gtglrlxtwl.html

Go:   strings.Index(s, "x")
来源：http://hz.yvedp.cn/gtnzimrllf.html

Ruby: s.index("x")
来源：http://hz.ydjk.org.cn/gtfyyfpojh.html

C#:   s.IndexOf("x")
来源：http://hz.hywenlv.cn/gtobxtdeue.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hfpthk.cn/gtmxbsfxln.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xingfuxueyuan.xyz/gtsxvxglro.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gtpbactodh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtgsfumxog.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dianchejie.cn/gtirdinomq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gtnkvisfqx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj20258888.top/gtknwitzhz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gotoacloud.top/gtjdhjdehl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xziqi.cn/gterwnivjx.html

[E06] 替换子串
来源：http://hz.aibaodan.cn/gtywfxewwz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.quarkkingdee.top/gtwzbtwufi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hammf.cn/gtvpftawgl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtjafjuhrd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gthlkazanm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtxhrkgnkb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.iojbl.cn/gtvmdkvwhb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.wangdashe.top/gtlmpnbzpk.html

C#:   s.Replace("a", "b")
来源：http://hz.svipenyu.cn/gtpldyflnf.html

[E07] 按分隔符拆分
来源：http://hz.jianghu66.top/gtpjlbjfhk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jianghu66.top/gtqyqmmtlk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zycfv.cn/gtczttxpzh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xinyue.icu/gtnnjpcbwc.html

TS:   s.split(",")
来源：http://hz.fengsongda.top/gtdgohnvdp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxinkj.top/gtvnxfmats.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gotoacloud.top/gtrlhzznpq.html

Ruby: s.split(",");  s.split
来源：http://hz.redwolf501.top/gtdvbyfdzl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daria6918.cn/gtefklrjxo.html

[E08] 数组按分隔符合并
来源：http://hz.cqqwz.cn/gtqjifmysl.html

Py:   ",".join(items)
来源：http://hz.shangyingyoupin.top/gtkyiayjos.html

PHP:  implode(",", $items);
来源：http://hz.cheryme.top/gtwinzbvwb.html

JS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtmipfdxct.html

TS:   items.join(",")
来源：http://hz.zycfv.cn/gtevdsuqiq.html

Java: String.join(",", items)
来源：http://hz.andypj.xyz/gtueglxyjz.html

Go:   strings.Join(items, ",")
来源：http://hz.gaohongyu789.top/gtuirfjrhu.html

Ruby: items.join(",")
来源：http://hz.vqdsnc.cn/gtgvzcksao.html

C#:   string.Join(",", items)
来源：http://hz.meibo888.top/gticirwfxa.html

[E09] 去除所有空白字符
来源：http://hz.sufxvd.cn/gtpakltwgw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hywenlv.cn/gtjriehxen.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gthskgtanp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtyujukgvz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinghuilouyu.cn/gtqxzswnbv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigfzy.top/gtvzkpjfta.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtxgodqssn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.snrcjt.cn/gtdwykfrvo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gthryvwjdd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yonumen.top/gtteohwjuv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gogol.net.cn/gtlvxzeofm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtfzplqsld.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtrtrhjzdm.html

TS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtgmcxgfnz.html

Java: String.format("%03d", 7)
来源：http://hz.shuidangran.top/gtlfpkrecl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jyoumei.cn/gtjyphzlgr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hywenlv.cn/gtvewldrxe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhongyouzk.top/gtisxbccwp.html

[E11] 反转字符串
来源：http://hz.cqqwz.cn/gtkhantmzw.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtngbafwam.html

PHP:  strrev($s);
来源：http://hz.pengpengdd.cyou/gtcgylnbyu.html

JS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtwxlojkhk.html

TS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtkwrqvdnq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aizwys.cn/gtowjcfjzr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sysykeji.top/gtxpjinaac.html

Ruby: s.reverse
来源：http://hz.nwbrower.top/gtbhrtcicr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhixingplan.top/gtrdktxllx.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258888.top/gtnnjuklmp.html

Py:   s.count("a")
来源：http://hz.gzhubu.top/gtpwkbxxul.html

PHP:  substr_count($s, "a");
来源：http://hz.xuetiantiany.cn/gtvkbzzayg.html

JS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtiiiqtuou.html

TS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtbphwnwhr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hfpthk.cn/gtfpyiddfq.html

Go:   strings.Count(s, "a")
来源：http://hz.hnxiangtu.top/gtxfgvmhav.html

Ruby: s.count("a")
来源：http://hz.redwolf501.top/gtvozmojau.html

C#:   s.Count(c => c == 'a')
来源：http://hz.svipenyu.cn/gtdqamnhlr.html

[E13] 逐字符遍历
来源：http://hz.daria6918.cn/gthcshgqjp.html

Py:   for ch in s: print(ch)
来源：http://hz.jiagoushi.top/gtdghnwnnf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aizwys.cn/gtpnhwuaqa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtntjzgyxg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtvuzjmcna.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhaomingkeji.xyz/gtysbvvslj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.9152youxi.cn/gtwuannnoq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinyuanbaomall.cn/gtqckuhudz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhaomingkeji.xyz/gtlbfspdve.html

[E14] URL 编码与 Base64
来源：http://hz.bjfxy.top/gtwnoackkw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.wangdashe.top/gtxilgtlzf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuxming.cn/gtrnbpggmm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangkeji.top/gtsrigsnll.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtipumwpig.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yueranfly.top/gtqunphsrl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtddpwmbmq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pycfn.com/gtxjwaqlzc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sufxvd.cn/gtdopauqgc.html

[E15] HTML 转义 / 反转义
来源：http://hz.haohaochexian.top/gtkvmxbtkt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dianchejie.cn/gtcmtzrsjt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yonumen.top/gtyvayxjms.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gtvjvqtrxg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtdioqclho.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigufen.top/gtpqwxjxqf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ppjwa.cn/gtzhvmpvqz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yueranfly.top/gtxfwkeezo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gtxafpyznp.html

[E16] 数字千分位
来源：http://hz.fzhhl.top/gtcchhdcnb.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gtjtnttbea.html

PHP:  number_format(1234567);
来源：http://hz.dianchejie.cn/gtoqkwiawf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cdnleiting.top/gtokxweege.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtnugackwe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtfqohccau.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuxming.cn/gtdxscwmpp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258888.top/gtpfwfbgiu.html

C#:   1234567.ToString("N0")
来源：http://hz.iojbl.cn/gtqxdueosm.html

[E17] 首字母大写
来源：http://hz.quarkkingdee.top/gtbmnagnpp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.redwolf501.top/gtuomtsvwq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtommhbjbb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtesnzplho.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.havefunace.top/gtlxrkixjl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fengsongda.top/gthclqazyf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hongshengwenyu.top/gtcfxjflsm.html

Ruby: s.capitalize
来源：http://hz.zhaomingkeji.xyz/gtpouqimnn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigufen.top/gthfbzdazt.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gtsikrnhcq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cucudq.cn/gtxkrtikar.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gtgczowqkf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtrkkxruqq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gtohneluns.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtvevsvsvw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxuanxn.top/gtrvjvcgps.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.andypj.xyz/gthqvfqair.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gttgzjylxb.html

[E19] 多行文本按行拆分
来源：http://hz.cqqwz.cn/gtuzwrzlwx.html

Py:   s.splitlines()
来源：http://hz.snrcjt.cn/gtsuchwypx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgufenzy.top/gtiegzfnhq.html

JS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtyytaxsjo.html

TS:   s.split(/\r?\n/)
来源：http://hz.gzhubu.top/gtbszwhywu.html

Java: s.lines().toList()
来源：http://hz.ivvv.top/gtscdbdddw.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtoutbjtek.html

Ruby: s.lines
来源：http://hz.shzxlz.cn/gtangexyhk.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtasrybvkv.html

[E20] 判断字符串是否为空
来源：http://hz.ydzc1.top/gtkizrarkw.html

Py:   if not s:
来源：http://hz.jyoumei.cn/gtkpysykiv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daria6918.cn/gtssavmzwm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gttjbasmrg.html

TS:   if (s === "") {}
来源：http://hz.jinghuilouyu.cn/gttddqtsnd.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtqqvlfgpk.html

Go:   if s == "" {}
来源：http://hz.ydzc1.top/gtckbtaqgo.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtqjchwvog.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jyoumei.cn/gtlfygkufn.html

[E21] 超长截断加省略号
来源：http://hz.nanxuanxn.top/gtoaivdfla.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shzxlz.cn/gthavialie.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zycfv.cn/gtirucdxqr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtfzdqimil.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gthugyyiol.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtcflzoalt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.kuanghao11.cn/gttmiclzmi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgfzy.top/gtkouiaika.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tianlin.xyz/gtrzqchwml.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gtlzujrugr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cucudq.cn/gtjshrgtxh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtykaanymk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtypucwelz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtsibbecqw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sufxvd.cn/gttbeghrog.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtfduwuyrj.html

Ruby: s.bytesize;  s.length
来源：http://hz.pycfn.com/gtmsnuxhyc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gttipsqmfv.html

================================================================================
来源：http://hz.gzhubu.top/gttulihsem.html

F. 文件与目录
来源：http://hz.gzhubu.top/gtdfuuepfr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpizdgznk.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtphseqckv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtrcrnrewq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hammf.cn/gtqsvdymda.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hysaishi.cn/gtyjcbfbaz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtizhshnir.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtqmxrqdgl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yongpay.top/gtnnxojuts.html

Ruby: File.read("a.txt")
来源：http://hz.sweek.top/gtyzbblhgo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtbhnfdkxc.html

[F02] 逐行读取文件
来源：http://hz.daria6918.cn/gtaidntqmt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangdashe.top/gthsaxmvkk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hongshengwenyu.top/gtxmzrlmky.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtnnwzrjvr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gteglencto.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gttujmfvdx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xziqi.cn/gttbvqwtbp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangkeji.top/gtnywqttuv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnqzz.top/gtuzqxpxel.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gtcwlofixq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gtiokkkzlt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtykdysjsx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtdzfhharp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtxeiuqogp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pengpengdd.cyou/gtfpyulbkz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ppjwa.cn/gtifmghlrn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangtech.top/gtkvzafedk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nanxuanxn.top/gtbjuadqgj.html

[F04] 追加写入文件
来源：http://hz.tanke756.top/gtzkdifdfe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtzjrxqqok.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cashguo.top/gtrngnyidr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gtmtxuhesi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gthtdkhpzu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daria6918.cn/gtidtszetr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangdashe.top/gtgvpndipl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtakprvbkb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hywenlv.cn/gtryfgwoam.html

[F05] 判断文件或目录是否存在
来源：http://hz.feifeiyinyue.top/gtnwtcahfp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.havefunace.top/gtyodxbsgv.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxinkj.top/gtplzhqxev.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtmmojrhhr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtvbdxztiq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtckkitjgt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sxryk.cn/gtnqespjlz.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gtonutnthr.html

C#:   File.Exists("a.txt")
来源：http://hz.shzxlz.cn/gtdzpcjmen.html

[F06] 删除文件
来源：http://hz.cucudq.cn/gtbcazkfre.html

Py:   os.remove("a.txt")
来源：http://hz.sxryk.cn/gtmnuukthh.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtyjmqpzhc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtgmibqoan.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtilmdjbjd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtcriytmbl.html

Go:   os.Remove("a.txt")
来源：http://hz.zycfv.cn/gtpgkvytxr.html

Ruby: File.delete("a.txt")
来源：http://hz.redwolf501.top/gtxjlutavm.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtvejusxif.html

[F07] 创建目录（含多级）
来源：http://hz.hywenlv.cn/gtizzlvakj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gtntlleivn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sufxvd.cn/gtdsdtkdmu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gtazevnmfg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtcxrhicsb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gtyqejwfty.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cucudq.cn/gtwbbrixcz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtphjbieiz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jyoumei.cn/gtgqaxtzeo.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtynfzlxyv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.mhx1999.top/gtslwentba.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gthfxqmzmv.html

JS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtztbobnoa.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtnhovkkth.html


<!-- 参考信息 -->