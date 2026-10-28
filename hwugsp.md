代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtsehwifiu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cdnleiting.top/gtfajnoecq.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtihbjwhfx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shangyingyoupin.top/gtudffiggu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cucudq.cn/gtnbdjgjqq.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gtxlsyqmzw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.snrcjt.cn/gtsktvqdjj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtwjxxkmef.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhijiandao.cn/gtapaeqvau.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtsvyhzqky.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.iojbl.cn/gtqsecmela.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tianlin.xyz/gtfzmcrova.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jyoumei.cn/gtppqdqdlz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tanke756.top/gtsaojixlj.html

[D25] Set 集合去重与交并差
来源：http://hz.shangyingyoupin.top/gtpcdraazd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhengqikj.top/gtkjhelgya.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shzxlz.cn/gtqbrmwgmo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aizwys.cn/gtonfwyqiy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pycfn.com/gtqwahmrwu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cheryme.top/gtkhhjhacs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhiwuduotai.top/gtiekcfktr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj20258.top/gtzxdgmeiv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnxiangtu.top/gtjfbajkyi.html

[D26] 数组转字符串
来源：http://hz.shuidangran.top/gtvvgthrvo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinghuilouyu.cn/gtsraybbkw.html

PHP:  implode(", ", $arr);
来源：http://hz.feifeiyinyue.top/gteltbggzh.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtrknojerf.html

TS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtciqjkhtj.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtjilhwtls.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhengqikj.top/gtwubrnbny.html

Ruby: arr.join(", ")
来源：http://hz.bjfxy.top/gtoeqqdlpo.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gtpnyoljnp.html

================================================================================
来源：http://hz.zycfv.cn/gtwcfbaqhf.html

E. 字符串处理
来源：http://hz.0kj1m.cn/gtshnhyqah.html

================================================================================
来源：http://hz.hysaishi.cn/gtdyfoagts.html

[E01] 拼接字符串
来源：http://hz.ivvv.top/gtpyvkbida.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangtech.top/gthbkxzmqm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dashuyun.cn/gtewmnfleo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.316326.xyz/gtiqxrghuq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtmlchjeoi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnqzz.top/gtacoekvlz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinghuilouyu.cn/gtyauuacpj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.guowangkeji.top/gtfbbdblch.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hywenlv.cn/gteztalajg.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gtwfojzdim.html

Py:   "ab" * 3
来源：http://hz.jyoumei.cn/gtbzlxxqio.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jianghu66.top/gtsonsipht.html

JS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtasddnmvj.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gthupgdiop.html

Java: "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtesyeiymy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtizzlcdfu.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gtcuehiyyn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tianlin.xyz/gtaqkyamzn.html

[E03] 截取子串
来源：http://hz.redwolf501.top/gtxbozkkqh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhongyouzk.top/gttcjrcdsv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sufxvd.cn/gtehdhxxbn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtofkfmxls.html

TS:   s.slice(1, 4)
来源：http://hz.ydzc1.top/gtjaayaect.html

Java: s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtowmtworm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xylfe.cn/gtrizfkhnp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cucudq.cn/gtkqhxeaxm.html

C#:   s.Substring(1, 3)
来源：http://hz.aizwys.cn/gtozjvqsse.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtojtyefsd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hysaishi.cn/gtkayjzeuq.html

PHP:  strpos($s, "x");
来源：http://hz.chenlongwang.top/gtffrlcdjn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xuetiantiany.cn/gtpmvoheuj.html

TS:   s.indexOf("x")
来源：http://hz.zhixingplan.top/gtsmaeyeix.html

Java: s.indexOf("x")
来源：http://hz.gotoacloud.top/gtpslrdtja.html

Go:   strings.Index(s, "x")
来源：http://hz.yuanzhike.top/gtojkuhrih.html

Ruby: s.index("x")
来源：http://hz.hnqzz.top/gtasuyidcq.html

C#:   s.IndexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtxetxorfj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj202588.top/gtbowqterw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daria6918.cn/gtzrppxqic.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.birdmap.top/gtwoffxoax.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtcqqsoltg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xylfe.cn/gtwrymhirc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtgxknohjk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangtech.top/gtpqpkeoxf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ehwqpu.com/gtppbbgavm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yangfankeji.com/gtniltjbfr.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtsbyvdlgb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pycfn.com/gtyhybahvd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cqqwz.cn/gtaywagkrd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtnehjwzno.html

TS:   s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtmzalfuwp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gthrigtndr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hongshengwenyu.top/gtudynlxrt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shanyushiyangtech.top/gtvaqryxic.html

C#:   s.Replace("a", "b")
来源：http://hz.birdmap.top/gthioiwabx.html

[E07] 按分隔符拆分
来源：http://hz.xingfuxueyuan.xyz/gtqvvmkton.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hammf.cn/gttmloykjh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nwbrower.top/gtylwhyxxk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuetiantiany.cn/gtfzfavtao.html

TS:   s.split(",")
来源：http://hz.cucudq.cn/gtnmtidaeo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxinkj.top/gtomwwlsdf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gotoacloud.top/gtcwymhumm.html

Ruby: s.split(",");  s.split
来源：http://hz.yueranfly.top/gthlxydswq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtaoqyjkhu.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtuxloaloe.html

Py:   ",".join(items)
来源：http://hz.xuanzx.com/gthypwivds.html

PHP:  implode(",", $items);
来源：http://hz.gotoacloud.top/gtjwzhsitm.html

JS:   items.join(",")
来源：http://hz.zycfv.cn/gtpswastff.html

TS:   items.join(",")
来源：http://hz.mhx1999.top/gtwhpwsbyr.html

Java: String.join(",", items)
来源：http://hz.birdmap.top/gtdxcuurfe.html

Go:   strings.Join(items, ",")
来源：http://hz.yvedp.cn/gtlexferqx.html

Ruby: items.join(",")
来源：http://hz.mhx1999.top/gtjiuzyynf.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtwfmizxgv.html

[E09] 去除所有空白字符
来源：http://hz.pycfn.com/gtatlddktp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gtkwvljkim.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ivvv.top/gtgndtydcn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtofcdeggo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhixingplan.top/gtobrpkvha.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.quarkkingdee.top/gtgmuuufyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.meibo888.top/gtggzksanr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.iojbl.cn/gtvzpqifci.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj20258.top/gtefahluoo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenzaomai.com/gtuxzjezab.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtoadevmpq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhengqikj.top/gtjbqmvfrq.html

JS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gteppnngll.html

TS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtzwotmqcw.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gtoaimxdge.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuanzx.com/gtffcdyihn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cdnleiting.top/gtjnmkqslt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yanxiufei.cn/gtbcscwkys.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gtvzwqdgby.html

Py:   s[::-1]
来源：http://hz.shuidangran.top/gtbaiqpiao.html

PHP:  strrev($s);
来源：http://hz.jlsjyb.cn/gtktiymbfz.html

JS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtsraidqty.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtmkzwqqgc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hammf.cn/gtnzrgcywa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhijiandao.cn/gtuofaehve.html

Ruby: s.reverse
来源：http://hz.mhx1999.top/gtlxdamjbs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtpsolczrz.html

[E12] 统计某字符出现次数
来源：http://hz.fengsongda.top/gtqbfbmojt.html

Py:   s.count("a")
来源：http://hz.xingfuxueyuan.xyz/gtdpmwllpx.html

PHP:  substr_count($s, "a");
来源：http://hz.jlsjyb.cn/gtgrecdhok.html

JS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtdngwfjeb.html

TS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtvvbuaehj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jiagoushi.top/gtzlyqjntu.html

Go:   strings.Count(s, "a")
来源：http://hz.c1oappe.top/gtyraizijd.html

Ruby: s.count("a")
来源：http://hz.aibaodan.cn/gtoebfzpza.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuetiantiany.cn/gtpbwkjeik.html

[E13] 逐字符遍历
来源：http://hz.sxryk.cn/gtvipnrupk.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258888.top/gtydpscdzb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tian-w.cn/gtfrhdpikh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtiloiyusm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtkgbahvhg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtyhqlqkhp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenzaomai.com/gtnscdqnrp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hongshengwenyu.top/gtflkxwmuv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtkzjhcizz.html

[E14] URL 编码与 Base64
来源：http://hz.0kj1m.cn/gtbvlowxbr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxinkj.top/gtzxkjeuag.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangshuangyany.cn/gtoxtdbsxj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yongpay.top/gtnistcmta.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.smart0.xyz/gtatgdxwho.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dianchejie.cn/gtohqgaozt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhengqikj.top/gtwbljhyzc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hnqzz.top/gtgzcoyzns.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtmzxrjfar.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuetiantiany.cn/gtodajiuso.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shzxlz.cn/gttztvblaf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ivvv.top/gtnfranwob.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtcysftrwa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xylfe.cn/gticzjatbk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.smart0.xyz/gtfurwmybm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.havefunace.top/gtwaoudyry.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenzaomai.com/gtytehpdzp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuetiantiany.cn/gtfylxmsts.html

[E16] 数字千分位
来源：http://hz.gogol.net.cn/gtbnadtdzk.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gtiprbmqmt.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gteehxfarw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtydefqqsa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.pycfn.com/gttovswpys.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.snrcjt.cn/gtdwrgvpxc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gtsbbssqce.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhixingplan.top/gtsvsxyhmb.html

C#:   1234567.ToString("N0")
来源：http://hz.yuxming.cn/gtexcwtfyd.html

[E17] 首字母大写
来源：http://hz.zhoulong.xyz/gtxygbxzbf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.haohaochexian.top/gtxoyevpno.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.9152youxi.cn/gtunxrgrpc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtqkzfruwk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtqvgejkei.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.smart0.xyz/gtqgthoaak.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.c1oappe.top/gteglflhwi.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtysoyaont.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daria6918.cn/gtxruxrgoh.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtnkqvaiea.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtpneondvm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yonumen.top/gtmpemtvtu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtjxyfhdzh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtowwharhd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtsudpdmpf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtkndiailu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gtivvmqemz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fzhhl.top/gthxhabigc.html

[E19] 多行文本按行拆分
来源：http://hz.yuanzhike.top/gtvzmatidu.html

Py:   s.splitlines()
来源：http://hz.yonumen.top/gtwnfadbtq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hongshengwenyu.top/gtlwavnzco.html

JS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtbhuwppml.html

TS:   s.split(/\r?\n/)
来源：http://hz.xinyue.icu/gtolcbsytn.html

Java: s.lines().toList()
来源：http://hz.bjfxy.top/gttgtyrfnu.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtlkfmxznv.html

Ruby: s.lines
来源：http://hz.tianlin.xyz/gtsmdzykzt.html

C#:   s.Split('\n')
来源：http://hz.svipenyu.cn/gthgdejtvb.html

[E20] 判断字符串是否为空
来源：http://hz.zhoulong.xyz/gteopfyjgm.html

Py:   if not s:
来源：http://hz.zhoulong.xyz/gtbwqacjcm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtrsnopipk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jianghu66.top/gtvyarhvho.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gtgfefcihi.html

Java: if (s.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtetccyahy.html

Go:   if s == "" {}
来源：http://hz.jiagoushi.top/gtimsqukng.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtucrgpjuu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hysaishi.cn/gtdyuejbyp.html

[E21] 超长截断加省略号
来源：http://hz.wangshuangyany.cn/gtalistgbm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhongyouzk.top/gtuqqwgnut.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yvedp.cn/gthpqzssgt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtjsxgwlyj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtovtyshqg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtwwckgyng.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenlongwang.top/gtakennijg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hammf.cn/gtxvaqjskr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgufenzy.top/gtfgrjwufl.html

[E22] 字节长度与字符长度
来源：http://hz.kuanghao11.cn/gtgojxmrbb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guowangkeji.top/gtpimislkn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtxdxazgdd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gtwyjvldop.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtosbtreec.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtzsouurrs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ybcxt.top/gtdgokhpzi.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenjidiqi.icu/gtenzsqdfx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gtxvhjtens.html

================================================================================
来源：http://hz.smart0.xyz/gtofsbqage.html

F. 文件与目录
来源：http://hz.cucudq.cn/gtyodtznng.html

================================================================================
来源：http://hz.9152youxi.cn/gtdwlgrtve.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtsotpksir.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtdzvdfpqf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.haohaochexian.top/gtdjmdtahs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenlongwang.top/gttvhhbdwt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.smart0.xyz/gtigbthpox.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtdmrdbgpc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hnxiangtu.top/gteyhasqtc.html

Ruby: File.read("a.txt")
来源：http://hz.feifeiyinyue.top/gtpwngfndb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtbdmwojdc.html

[F02] 逐行读取文件
来源：http://hz.jinyuanbaomall.cn/gtwbgxqgvv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhoulong.xyz/gtliueouqr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.andypj.xyz/gthqgmisyh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtthvicksh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtovkppuqh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtktiscvph.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnqzz.top/gtzjhduvec.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydzc1.top/gtfgzumzdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sxryk.cn/gtqssqtwng.html

[F03] 写入文件（覆盖）
来源：http://hz.aizwys.cn/gtcmliqzzl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yonumen.top/gtvsbleray.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtqzimrgpn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtxslfnztf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gtkbpqktnn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hongshengwenyu.top/gtftjaalke.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yuanzhike.top/gtrvctvlmr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guannengcc.top/gtyoghkrth.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yvedp.cn/gtnptujtuo.html

[F04] 追加写入文件
来源：http://hz.pengpengdd.cyou/gtbuhkaqps.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtxwnjuoql.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gtyuakkjek.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtsszwqpao.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtxrrkqlza.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shuidangran.top/gtunopvflw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yueranfly.top/gttcktnyeh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yanxiufei.cn/gtygsgpmud.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gaohongyu789.top/gtaoddmxzl.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhaomingkeji.xyz/gtssodlqtj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xylfe.cn/gtyauztvzt.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtjgetusgu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtbqqgjfra.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtiqspfjfh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtigeebqdd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gtfygqmmmv.html

Ruby: File.exist?("a.txt")
来源：http://hz.zycfv.cn/gtxewekpme.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangtech.top/gtfndqyfht.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtqixarrrg.html

Py:   os.remove("a.txt")
来源：http://hz.zdqjudy.top/gtfvcdlobt.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gttcafvnco.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtymurfyir.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.316326.xyz/gtfzdzcxbj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gthfpfgmzk.html

Go:   os.Remove("a.txt")
来源：http://hz.mhx1999.top/gtxgvoyyaz.html

Ruby: File.delete("a.txt")
来源：http://hz.sufxvd.cn/gtpcfjfmwz.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtjeaqcnlr.html

[F07] 创建目录（含多级）
来源：http://hz.yonumen.top/gtgnmpwwdf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtoqnokfmo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtlvtmzyho.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtxrgjdgsy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gtnlovegcr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xinyue.icu/gtkcvdxtff.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xingfuxueyuan.xyz/gtxzwgkmil.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtuusgdyph.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jianghu66.top/gtxruyvmib.html

[F08] 遍历目录
来源：http://hz.mhx1999.top/gtyvgxqwda.html


<!-- 参考信息 -->