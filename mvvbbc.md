代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fzhhl.top/gtsizotidl.html

[D24] 字典 / Map 基本操作
来源：http://hz.xziqi.cn/gtbbagokin.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.316326.xyz/gtvrnynjgx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cucudq.cn/gtmbepolie.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigfzy.top/gttvkvyjzu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.316326.xyz/gtcnesyqkc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtfjqkpjny.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gtdzqmcjtb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hammf.cn/gtbprrzqdv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pycfn.com/gtevmtfdsr.html

[D25] Set 集合去重与交并差
来源：http://hz.yonumen.top/gtzjkacenz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pengpengdd.cyou/gtnjyykgat.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuanzhike.top/gtfbtxtzzf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.redwolf501.top/gtliilispn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gtlrysylmw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yonumen.top/gtbayvgciq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shangyingyoupin.top/gtqxkgmcqj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenjidiqi.icu/gtwplpbpms.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.iojbl.cn/gtidwfzzks.html

[D26] 数组转字符串
来源：http://hz.cucudq.cn/gtuitrcjbv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zdqjudy.top/gtwfbwwqhg.html

PHP:  implode(", ", $arr);
来源：http://hz.hnxiangtu.top/gtmotmziam.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtmqxbkviu.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtdvgcorno.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gthzcqkmzp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtcacbxknq.html

Ruby: arr.join(", ")
来源：http://hz.chenzaomai.com/gtuyfmlzvm.html

C#:   string.Join(", ", list)
来源：http://hz.yj202588.top/gtjslryhuu.html

================================================================================
来源：http://hz.wangdashe.top/gtocxibpbn.html

E. 字符串处理
来源：http://hz.ppjwa.cn/gtusksjxrl.html

================================================================================
来源：http://hz.shzxlz.cn/gtjwmijiiv.html

[E01] 拼接字符串
来源：http://hz.smart0.xyz/gtrufmncci.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.mhx1999.top/gtlkpfscie.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ivvv.top/gtcslmhunt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtsxfbwcwc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gttmrracup.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xziqi.cn/gtnlcqhtbj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtrwbuxgkg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.haohaochexian.top/gtvrrtitbj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jianghu66.top/gtdevhwnff.html

[E02] 重复字符串
来源：http://hz.andypj.xyz/gtmqjugkvm.html

Py:   "ab" * 3
来源：http://hz.daria6918.cn/gtdixxybxc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cdnleiting.top/gtakrorsar.html

JS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtaxhzpayr.html

TS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtbkxmcilp.html

Java: "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtxjhorwao.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenzaomai.com/gtgfluzbhh.html

Ruby: "ab" * 3
来源：http://hz.yanxiufei.cn/gtgnkxjzxa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gttyhthaes.html

[E03] 截取子串
来源：http://hz.zhixingplan.top/gtuwnocgzj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtdhwhdrbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gtcffxsfko.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtqnfdkekl.html

TS:   s.slice(1, 4)
来源：http://hz.meibo888.top/gtjtjulhqt.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtiqawwcwy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sweek.top/gtncqnvtky.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.redwolf501.top/gtrusqnlug.html

C#:   s.Substring(1, 3)
来源：http://hz.tianlin.xyz/gtvnamjenl.html

[E04] 查找子串位置
来源：http://hz.jiagoushi.top/gtadbbwgqi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dianchejie.cn/gtgyazlvbp.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gtmwkzlnos.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ppjwa.cn/gtthljnshn.html

TS:   s.indexOf("x")
来源：http://hz.xylfe.cn/gtonismqtc.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gtcyoluhwk.html

Go:   strings.Index(s, "x")
来源：http://hz.sufxvd.cn/gtqtzunrmr.html

Ruby: s.index("x")
来源：http://hz.xinyue.icu/gtjjmirslc.html

C#:   s.IndexOf("x")
来源：http://hz.meibo888.top/gtcemjcrpm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxinkj.top/gtjxfxkdzg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xinyue.icu/gtaksilify.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.iojbl.cn/gtgyxlzadd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtabcwdlaf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtpkznrxmo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtlsebdrst.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuetiantiany.cn/gtkdkakjfw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cqqwz.cn/gtvijjgizk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.0kj1m.cn/gtlefcktgc.html

[E06] 替换子串
来源：http://hz.ybcxt.top/gtgyrpiwnx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.quarkkingdee.top/gtxvocfvvj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dashuyun.cn/gtchuvlpkg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gthmeazfzd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtrosbonds.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtyddiovbz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.haohaochexian.top/gttwvmalwo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daria6918.cn/gtkjivfmgt.html

C#:   s.Replace("a", "b")
来源：http://hz.zhiwuduotai.top/gtaammtyzk.html

[E07] 按分隔符拆分
来源：http://hz.chenjidiqi.icu/gtkfuwgimc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tianlin.xyz/gtsnhzuphk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuanzhike.top/gtsuzrkhzk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.iojbl.cn/gtqdkbwmnv.html

TS:   s.split(",")
来源：http://hz.vqdsnc.cn/gtugxclhxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gzhubu.top/gttlejxwam.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtzfmrrvzc.html

Ruby: s.split(",");  s.split
来源：http://hz.hfpthk.cn/gtehuhpjik.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhoulong.xyz/gtyqrkqmhp.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtbgwujukm.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtastpoacw.html

PHP:  implode(",", $items);
来源：http://hz.zhengqikj.top/gtsvgdeadv.html

JS:   items.join(",")
来源：http://hz.jyoumei.cn/gtggzidckb.html

TS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtjxohacxo.html

Java: String.join(",", items)
来源：http://hz.wangdashe.top/gthvbkohxl.html

Go:   strings.Join(items, ",")
来源：http://hz.svipenyu.cn/gtjmiixjut.html

Ruby: items.join(",")
来源：http://hz.jianghu66.top/gtqemtdopn.html

C#:   string.Join(",", items)
来源：http://hz.iojbl.cn/gtbzvhgzbw.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtywjjhtdx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ehwqpu.com/gtnpijzqtb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gogol.net.cn/gtsjdsdevh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gthzauptea.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtbafwiccl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.bjfxy.top/gtrqvtlmld.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shuidangran.top/gthcbwpcfw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daxiang520.top/gtnkqdjlmy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuxming.cn/gttyqhecov.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gogol.net.cn/gtuildphak.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cashguo.top/gtgkwsbone.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ydzc1.top/gtlqftjypj.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtojeopoxb.html

TS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtptappnmv.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtdailxhex.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtfnyaynhj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guannengcc.top/gtkfqhfwks.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhengqikj.top/gttidsoplv.html

[E11] 反转字符串
来源：http://hz.zhengqikj.top/gtlcfvnrdl.html

Py:   s[::-1]
来源：http://hz.yvedp.cn/gtdewyzxcx.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtvkvpiybc.html

JS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtgbqkhsvf.html

TS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtojutcigi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hfpthk.cn/gtjyukxynt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ybcxt.top/gtdpkdlyhe.html

Ruby: s.reverse
来源：http://hz.daxiang520.top/gtienqhlar.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtiowpwlxb.html

[E12] 统计某字符出现次数
来源：http://hz.pycfn.com/gtfrzwhqbz.html

Py:   s.count("a")
来源：http://hz.jianghu66.top/gtbuxgxays.html

PHP:  substr_count($s, "a");
来源：http://hz.hnxiangtu.top/gtilqbfget.html

JS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtkykvwwzk.html

TS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtaqrxwlzh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.redwolf501.top/gtouizrkfk.html

Go:   strings.Count(s, "a")
来源：http://hz.ydzc1.top/gthcuxdpdg.html

Ruby: s.count("a")
来源：http://hz.dashuyun.cn/gtcfzmzdpp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenzaomai.com/gtyezsugbr.html

[E13] 逐字符遍历
来源：http://hz.hywenlv.cn/gtrjgdyxut.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtxzzkylbq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pengpengdd.cyou/gtopfbqklg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhijiandao.cn/gtzguhntjt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtndyunqhw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jiagoushi.top/gtbiuejroi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.mhx1999.top/gtafvblztd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yueranfly.top/gtstxefsxh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangkeji.top/gtvmwejkuc.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtiwznvxoj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tanke756.top/gtpmvhcyfh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.haohaochexian.top/gtliqwvgqp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangshuangyany.cn/gtfemqshbv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.haohaochexian.top/gtgmwhnarh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gtpuhaerwb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj20258888.top/gtqdnkhnxq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gtkgdkaoft.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.mhx1999.top/gtbkxuhbvt.html

[E15] HTML 转义 / 反转义
来源：http://hz.jyoumei.cn/gtjuaqeutx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hongshengwenyu.top/gtijvxclfm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.haohaochexian.top/gtenwauuli.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gogol.net.cn/gtrvenetvr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hfpthk.cn/gtugjywmog.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtpllxgrrt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangshuangyany.cn/gtzvwzuunt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgfzy.top/gtxjdtkiqr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zycfv.cn/gtvzypwqhs.html

[E16] 数字千分位
来源：http://hz.daxiang520.top/gtxfqtfncd.html

Py:   f"{1234567:,}"
来源：http://hz.gotoacloud.top/gtifaqownq.html

PHP:  number_format(1234567);
来源：http://hz.zhijiandao.cn/gtpwyzvlxk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.pycfn.com/gtejgyqpsn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtskwteuhn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fzhhl.top/gtyrvkoqxl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtadyxfsel.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.birdmap.top/gtgnlchpfp.html

C#:   1234567.ToString("N0")
来源：http://hz.ydzc1.top/gtiruuhvoe.html

[E17] 首字母大写
来源：http://hz.quarkkingdee.top/gthqgklfyr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jiagoushi.top/gtuysdovgz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtipfwhlrq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtncivgnoz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhixingplan.top/gtljpjhtsr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pycfn.com/gtaebjwrcd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yueranfly.top/gtmmhawaul.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gtintuhpax.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenjidiqi.icu/gtaqgeddhm.html

[E18] 模板占位符替换
来源：http://hz.xingfuxueyuan.xyz/gtsfdruqjl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.mhx1999.top/gtmlzvlcjc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigufen.top/gtrqdarkie.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtddbwarhv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtpdmqfboi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtymrjirjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ivvv.top/gtjurpmtlm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ivvv.top/gtscxwklfm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtdbzoeadu.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtwpyhidsp.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gtxyfmcqml.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgufenzy.top/gtbhrayuxx.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtleoilpyi.html

TS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtrkfhklzs.html

Java: s.lines().toList()
来源：http://hz.jiagoushi.top/gtzkbfyyxf.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtykwnaika.html

Ruby: s.lines
来源：http://hz.daxiang520.top/gtlgvtfffk.html

C#:   s.Split('\n')
来源：http://hz.jinghuilouyu.cn/gtkegijywk.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtxwsczqor.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtckkxgbzb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jiagoushi.top/gtwzdpuopo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhiwuduotai.top/gtovltvjax.html

TS:   if (s === "") {}
来源：http://hz.haohaochexian.top/gtmdtwkewy.html

Java: if (s.isEmpty()) {}
来源：http://hz.mhx1999.top/gtdyntzxfm.html

Go:   if s == "" {}
来源：http://hz.yanxiufei.cn/gtuzshsjoq.html

Ruby: if s.empty?
来源：http://hz.jinyuanbaomall.cn/gtottwmsqf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ehwqpu.com/gtiywtvest.html

[E21] 超长截断加省略号
来源：http://hz.pengpengdd.cyou/gtdpqmpejn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hysaishi.cn/gtoohxcxbc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangdashe.top/gtfvqagtpv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtjwsnkpdc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtbduvfkmf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtcedhvxii.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ehwqpu.com/gtvebhozap.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtmplefbri.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtkheqbrds.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtzcavasxg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tianlin.xyz/gtarhsxlvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtwgdzdauj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtfhoawxxn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtwmdcqsqc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtlmyoohlr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cheryme.top/gtjykynkmv.html

Ruby: s.bytesize;  s.length
来源：http://hz.iojbl.cn/gtizbcxpaf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yonumen.top/gtkwbgvlrf.html

================================================================================
来源：http://hz.hfpthk.cn/gtfrejuppn.html

F. 文件与目录
来源：http://hz.meibo888.top/gtydbzaune.html

================================================================================
来源：http://hz.chenzaomai.com/gtgzuxxbkj.html

[F01] 读取整个文件
来源：http://hz.hywenlv.cn/gtynnqienr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtyzpxxkso.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aizwys.cn/gtzzlqrbrl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtelzwgihp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tian-w.cn/gtwupycvmt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gthdnhmdld.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jiagoushi.top/gterqzwtlk.html

Ruby: File.read("a.txt")
来源：http://hz.guowangkeji.top/gtcntgmbzv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jlsjyb.cn/gtkvkxmuro.html

[F02] 逐行读取文件
来源：http://hz.ehwqpu.com/gtuxkujoeh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhaomingkeji.xyz/gtwnvgbcwp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ywan-chungtsiang.top/gtacgodgip.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gteibrlvll.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtfivegyvr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gtmkmrjfvh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangkeji.top/gtzoicvspn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtlquwuklc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tian-w.cn/gtukgigyaa.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtkrombvom.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daxiang520.top/gtgtcecykn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtahsscktm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtoreamlfh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtbqdakncp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhengqikj.top/gtqepdmawu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhiwuduotai.top/gtpjgfphba.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhongyouzk.top/gttwpsnnnu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtilsptwub.html

[F04] 追加写入文件
来源：http://hz.dianchejie.cn/gtnltmoyrq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cqqwz.cn/gtzejaedup.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.quarkkingdee.top/gtwawhcizp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtsyceyfmm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtatmwzwez.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daxiang520.top/gtynqhxibq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gtalehrvaz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydzc1.top/gtuqvwwnxa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pengpengdd.cyou/gtcxlyupxy.html

[F05] 判断文件或目录是否存在
来源：http://hz.snrcjt.cn/gtqnkjtmef.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dianchejie.cn/gtzxyiflin.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtosysdrjx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtcerrjgwa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtidghjmde.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtmctbuulx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gtotouihdj.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtfvrpytlm.html

C#:   File.Exists("a.txt")
来源：http://hz.aizwys.cn/gthyewkyec.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtccbomzcw.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtovuwgwkk.html

PHP:  unlink("a.txt");
来源：http://hz.shuidangran.top/gtbrfwqrqd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtruvssjrz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtmfnkzmsb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtdzmntmer.html

Go:   os.Remove("a.txt")
来源：http://hz.zhongyouzk.top/gtkdokxmeg.html

Ruby: File.delete("a.txt")
来源：http://hz.mhx1999.top/gtgvaqrwkx.html

C#:   File.Delete("a.txt");
来源：http://hz.xuetiantiany.cn/gttdagibls.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtxvrhzzpk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhongyouzk.top/gtuavjigue.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydjk.org.cn/gtkogcdqiw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtjcvqwjqc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtvmfecxtu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydzc1.top/gtughvtcyy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daxiang520.top/gtxmlaplrg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jyoumei.cn/gtuowvzykk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shuidangran.top/gtxjkztayw.html

[F08] 遍历目录
来源：http://hz.sufxvd.cn/gtavxguueq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hfpthk.cn/gtwpaotnmu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ivvv.top/gtsgjnnkxj.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtznszammd.html

TS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtnkdeqfse.html


<!-- 参考信息 -->