代发 wailian999

Ruby: arr.tally
来源：http://hz.shanyushiyangtech.top/gtyojgeelr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ppjwa.cn/gtiavnyjvx.html

[D21] 判断是否包含某元素
来源：http://hz.meibo888.top/gttqgzoxii.html

Py:   x in arr
来源：http://hz.daxiang520.top/gtwhsggrzx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinqigufen.top/gtfybchaju.html

JS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gturhkokrw.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gthcrrxwyl.html

Java: list.contains(x)
来源：http://hz.ywan-chungtsiang.top/gtpwjnzsoh.html

Go:   slices.Contains(arr, x)
来源：http://hz.0kj1m.cn/gtimcvdxej.html

Ruby: arr.include?(x)
来源：http://hz.yueranfly.top/gttltxbijf.html

C#:   list.Contains(x)
来源：http://hz.sysykeji.top/gtaksfwqbn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258.top/gtplgqbgqf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtyjdjcqid.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgufenzy.top/gtyctkgyra.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj20258.top/gtkmkwrogg.html

TS:   [...arr];
来源：http://hz.yonumen.top/gtzctlhzkw.html

Java: new ArrayList<>(list);
来源：http://hz.hnqzz.top/gtlmaxnlvs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.redwolf501.top/gtgzxujhmp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.quarkkingdee.top/gtnpydrada.html

C#:   new List<int>(list);
来源：http://hz.zhiwuduotai.top/gtknqdhbxw.html

[D23] reduce 累积计算
来源：http://hz.nwbrower.top/gtzprdopjh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangshuangyany.cn/gtcrbfxvbg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.guannengcc.top/gttxotaftj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtuqocxsfy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtgghcbcms.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtvgrkmtpq.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtabaqszol.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sysykeji.top/gtoshffwny.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gtwqxhesqx.html

[D24] 字典 / Map 基本操作
来源：http://hz.tianlin.xyz/gtyebccbgi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtobxogbmn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hongshengwenyu.top/gtttgrkfal.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yonumen.top/gtxxyfjqoi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnqzz.top/gtiewhmhcu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gzhubu.top/gtajqrwbtq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hnqzz.top/gtgthxiglo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtkudochej.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pycfn.com/gtqxugkrcg.html

[D25] Set 集合去重与交并差
来源：http://hz.316326.xyz/gtinkjykmp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jlsjyb.cn/gtbephuqop.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.pengpengdd.cyou/gtmsoawzdd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ivvv.top/gtdsiotcaq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj202588.top/gtrhdfgvla.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.meibo888.top/gtkmaesdpm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.meibo888.top/gteovlblpg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dianchejie.cn/gtxrdrhler.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cashguo.top/gtswqxccqb.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtahpjhbsr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cdnleiting.top/gtnakgzvfe.html

PHP:  implode(", ", $arr);
来源：http://hz.xuetiantiany.cn/gtzldgdmef.html

JS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtbjrwafrn.html

TS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtqseesghv.html

Java: String.join(", ", list)
来源：http://hz.cheryme.top/gtmqmzxqrg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yonumen.top/gtcguuwewb.html

Ruby: arr.join(", ")
来源：http://hz.sysykeji.top/gtkkhbyafx.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gtostvekpm.html

================================================================================
来源：http://hz.havefunace.top/gtudsbznzh.html

E. 字符串处理
来源：http://hz.nanxinkj.top/gtibcjdxvt.html

================================================================================
来源：http://hz.fzhhl.top/gtgynqxscl.html

[E01] 拼接字符串
来源：http://hz.jyoumei.cn/gtikxoaufv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yuanzhike.top/gtusymabta.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daria6918.cn/gtlggupyir.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtxycsgddo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtdtlumnfp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gaohongyu789.top/gtasgfoyfg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.feifeiyinyue.top/gtgopupcdv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tanke756.top/gtkettlaan.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.andypj.xyz/gtvjsonqxt.html

[E02] 重复字符串
来源：http://hz.aibaodan.cn/gtqjydrnen.html

Py:   "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtpthztxev.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hysaishi.cn/gtqiseimyk.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gturvloihx.html

TS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtfeqhbjme.html

Java: "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtmkkhcbnj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fengsongda.top/gtzmyqjhbt.html

Ruby: "ab" * 3
来源：http://hz.jinqigufen.top/gtvnlyahma.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yanxiufei.cn/gtsuyagmzc.html

[E03] 截取子串
来源：http://hz.cucudq.cn/gtrlybqxbz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gtoljylzyx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yangfankeji.com/gtlefqmhxx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuxming.cn/gtvojqyxcc.html

TS:   s.slice(1, 4)
来源：http://hz.jianghu66.top/gtvkfxzhfw.html

Java: s.substring(1, 4)
来源：http://hz.sxryk.cn/gthjqpvenb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xinyue.icu/gtjsfskvzl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhaomingkeji.xyz/gtshcdjuve.html

C#:   s.Substring(1, 3)
来源：http://hz.quarkkingdee.top/gtbjojskfp.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gtrznclcvv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.52xcode.cn/gthbrckani.html

PHP:  strpos($s, "x");
来源：http://hz.hnqzz.top/gtagukujeo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tianlin.xyz/gttapwfbso.html

TS:   s.indexOf("x")
来源：http://hz.yvedp.cn/gtjnnlafrg.html

Java: s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtkmsghcny.html

Go:   strings.Index(s, "x")
来源：http://hz.meibo888.top/gtcbattksl.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtgvtxgzme.html

C#:   s.IndexOf("x")
来源：http://hz.haohaochexian.top/gtpbdvmegp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ppjwa.cn/gtfoyyahaq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuanzhike.top/gtaokocdbt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yonumen.top/gthjidibje.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtweclvxvc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shangyingyoupin.top/gtddxadrsx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtalpvggrp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhongyouzk.top/gtlfvwmpir.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gthrrtllbt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.guowangkeji.top/gtywmsidow.html

[E06] 替换子串
来源：http://hz.sweek.top/gtnpyctdul.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.birdmap.top/gtnugbrbvx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jqgufenzy.top/gterzmdsrp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtxgenblxk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtqwzoieft.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gthutavavp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sxryk.cn/gtpzlyoejh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.meibo888.top/gtuunkmuns.html

C#:   s.Replace("a", "b")
来源：http://hz.ydjk.org.cn/gtqbcrxplw.html

[E07] 按分隔符拆分
来源：http://hz.ywan-chungtsiang.top/gtxmujdoph.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hywenlv.cn/gtzbporhch.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fengsongda.top/gtpqqlcgel.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.guowangkeji.top/gtionrpntc.html

TS:   s.split(",")
来源：http://hz.chenjidiqi.icu/gtahusqrvm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yangfankeji.com/gtzdilnyiz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jyoumei.cn/gtgbenvleo.html

Ruby: s.split(",");  s.split
来源：http://hz.ydjk.org.cn/gtbapdrdtq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yvedp.cn/gtifmqskol.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gtkhbsnybr.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangtech.top/gtcgaekiut.html

PHP:  implode(",", $items);
来源：http://hz.yanxiufei.cn/gtimwilwsp.html

JS:   items.join(",")
来源：http://hz.shuidangran.top/gtjrwxtfnb.html

TS:   items.join(",")
来源：http://hz.zhijiandao.cn/gthclhxzgv.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gtkbjpfdit.html

Go:   strings.Join(items, ",")
来源：http://hz.ivvv.top/gtxvnbvmal.html

Ruby: items.join(",")
来源：http://hz.vqdsnc.cn/gtsfqlzgff.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtynlqykkx.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangtech.top/gtbhvqarys.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.andypj.xyz/gtmcruitky.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.quarkkingdee.top/gtquwrkdgv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtymhhcuun.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtspogsywj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xylfe.cn/gtlrriuqnz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenzaomai.com/gtlrluztjy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gogol.net.cn/gtngfpjhef.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hywenlv.cn/gtqmluzhey.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dianchejie.cn/gtrhpqchzw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gtjsphcukl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuanzhike.top/gtqndahqsr.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gteeqeloyo.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtrmocgnqq.html

Java: String.format("%03d", 7)
来源：http://hz.ivvv.top/gtexkephlq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtrimetvyy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gzhubu.top/gtmnkqtzuo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhongyouzk.top/gtrpetuhhb.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gtdknoxjpy.html

Py:   s[::-1]
来源：http://hz.sufxvd.cn/gtjkdrifen.html

PHP:  strrev($s);
来源：http://hz.zhixingplan.top/gtxmioozjb.html

JS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtxhrnkwsm.html

TS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gttnfekfsn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hysaishi.cn/gtaosxwkjx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.kuanghao11.cn/gtipstdols.html

Ruby: s.reverse
来源：http://hz.jiagoushi.top/gtynyvsvdy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtucrcqtel.html

[E12] 统计某字符出现次数
来源：http://hz.ppjwa.cn/gtfdiczlon.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtgunvgcmn.html

PHP:  substr_count($s, "a");
来源：http://hz.fengsongda.top/gtkvlrckzw.html

JS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gthgxwwxgz.html

TS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtefddjuwi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.smart0.xyz/gtyotwdfsc.html

Go:   strings.Count(s, "a")
来源：http://hz.yuxming.cn/gtznnwbpcb.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtitxaudqs.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtedmpolhr.html

[E13] 逐字符遍历
来源：http://hz.ybcxt.top/gtfujxwepl.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxinkj.top/gtqgzqytvz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnxiangtu.top/gtpumyvcvs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gaohongyu789.top/gtcysthzoq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtduuowmto.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtjmsxjjio.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.c1oappe.top/gtvfceiotf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tian-w.cn/gtbpqouxfa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxinkj.top/gtmyiujxkh.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtgzisghsy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.quarkkingdee.top/gtwfreybsq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gtxospouxq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgufenzy.top/gtmvouabnb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gtplkjcjzf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258.top/gtoeamoiic.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtrbpzsmpp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ehwqpu.com/gtqlljucty.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jiagoushi.top/gtujeidjlz.html

[E15] HTML 转义 / 反转义
来源：http://hz.hnqzz.top/gtokokrmwm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hysaishi.cn/gtldqkzqxn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtkntsotee.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj202588.top/gtzpcuvyur.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhiwuduotai.top/gtqkgidikx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hammf.cn/gtcvxluzje.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zdqjudy.top/gtaghvqiwv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtpibzlgje.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtphpxwbub.html

[E16] 数字千分位
来源：http://hz.jqgfzy.top/gtwadvtnsb.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gtppkpxrog.html

PHP:  number_format(1234567);
来源：http://hz.xingfuxueyuan.xyz/gtxzvedlqx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gthozasymb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtavszfete.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shangyingyoupin.top/gtnaevmadq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.0kj1m.cn/gtcemcvbdd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ppjwa.cn/gtzfhgnznq.html

C#:   1234567.ToString("N0")
来源：http://hz.hnxiangtu.top/gtnayxopnl.html

[E17] 首字母大写
来源：http://hz.zhiwuduotai.top/gtuawpxadz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gotoacloud.top/gtlrenbmjk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gtkqigxjvt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gthgpdiwfn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtmnxwkqqy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dashuyun.cn/gthjtijsto.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxuanxn.top/gttvtbtrby.html

Ruby: s.capitalize
来源：http://hz.zhiwuduotai.top/gtcfgjeobk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtzgwdbtba.html

[E18] 模板占位符替换
来源：http://hz.zhixingplan.top/gtlxlpioim.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.feifeiyinyue.top/gtgmvmiyar.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gtzermqfzd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtiixuhdla.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtkwlguurn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtufgehvxx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtekgircwd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sweek.top/gtmxjntlln.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gtvmudopxt.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtcgoqsdnp.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtpfqggglc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cqqwz.cn/gtcryxxzlx.html

JS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtcqfspkfa.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtbfoaoasj.html

Java: s.lines().toList()
来源：http://hz.cheryme.top/gtfkdfgktj.html

Go:   strings.Split(s, "\n")
来源：http://hz.mhx1999.top/gtybjgmrwp.html

Ruby: s.lines
来源：http://hz.yj202588.top/gtyesppxtj.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtafwzhmdy.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtxuyyziya.html

Py:   if not s:
来源：http://hz.ivvv.top/gttchrmkju.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cashguo.top/gtthndtgss.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtpckjdmgs.html

TS:   if (s === "") {}
来源：http://hz.daria6918.cn/gtbklixqmz.html

Java: if (s.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtqefkcixu.html

Go:   if s == "" {}
来源：http://hz.0kj1m.cn/gtjhzzpaai.html

Ruby: if s.empty?
来源：http://hz.yj20258888.top/gtxspvuxpn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cucudq.cn/gtsysqrayj.html

[E21] 超长截断加省略号
来源：http://hz.hnxiangtu.top/gtvmvmwsgz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tianlin.xyz/gtjgsugyfy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sysykeji.top/gtgrdfrzas.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtkkmcxuwa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtxdkrqkgm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtfiwzskka.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dashuyun.cn/gtjmjorvmi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gtnicvvhld.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yongpay.top/gtgtwmcehy.html

[E22] 字节长度与字符长度
来源：http://hz.jianghu66.top/gtuuxxpbll.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jianghu66.top/gttfxsjubu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtuvgxyvsg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtpwezjgqk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtkzkgswgu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhijiandao.cn/gtmbcafrjv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgfzy.top/gteztnqddv.html

Ruby: s.bytesize;  s.length
来源：http://hz.shuidangran.top/gtmgdiidwi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.52xcode.cn/gtzwlvuhid.html

================================================================================
来源：http://hz.tanke756.top/gtgnhprxnd.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtbnhkkvrs.html

================================================================================
来源：http://hz.zhijiandao.cn/gttmagaaib.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gtjkkcjqqo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tian-w.cn/gtfnamtkiv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtliujrras.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cucudq.cn/gtwrsplkbf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gttkzghoeh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtkkxufruv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtodplrlcb.html

Ruby: File.read("a.txt")
来源：http://hz.daxiang520.top/gtqxkcgjgh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgufenzy.top/gtemvccibh.html

[F02] 逐行读取文件
来源：http://hz.nwbrower.top/gtymqodqaj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gtynkzjqrd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.52xcode.cn/gtkkcjizia.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtusixhbax.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sufxvd.cn/gtfadhmpbl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtbtoeyzaa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gtnkspeaig.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtqniqcqyj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zycfv.cn/gtwkjgmbpy.html

[F03] 写入文件（覆盖）
来源：http://hz.ydjk.org.cn/gtcnqllyrt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yueranfly.top/gtjautvkpc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtprgrzjbj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtufbwnycq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtxepesyrn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gtehprsgab.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangshuangyany.cn/gtkclkzmsa.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gtwcqvirkt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtdkwlvdsn.html

[F04] 追加写入文件
来源：http://hz.quarkkingdee.top/gtdvyzhnoo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aibaodan.cn/gtrasgrqez.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.andypj.xyz/gttkhfuvig.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtfhqtrlvm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtaskxuqiz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gzhubu.top/gtpzvufexy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangtech.top/gtnlmnqzza.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gtsbrsobye.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigfzy.top/gtrigelzej.html

[F05] 判断文件或目录是否存在
来源：http://hz.aibaodan.cn/gtydcnujkl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.9152youxi.cn/gtlxyzblsr.html

PHP:  file_exists("a.txt");
来源：http://hz.hfpthk.cn/gtkhxbqpzc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtmvgrvzas.html


<!-- 参考信息 -->