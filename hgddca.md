代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenlongwang.top/gtvbartosi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hfpthk.cn/gtxqussuba.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtqkwenmjx.html

TS:   [...arr];
来源：http://hz.jianghu66.top/gtvvcfhdhk.html

Java: new ArrayList<>(list);
来源：http://hz.quarkkingdee.top/gtshzdnbyt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ehwqpu.com/gtppjgivdz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtinwjosrl.html

C#:   new List<int>(list);
来源：http://hz.vqdsnc.cn/gtqufzxndk.html

[D23] reduce 累积计算
来源：http://hz.gogol.net.cn/gtwnwrnrvr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydjk.org.cn/gtjcppxibi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtqwcjezpb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gthkxgxapg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtmflgefwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tianlin.xyz/gtffnvzygl.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtmkpfetzq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sweek.top/gtukdegxib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenjidiqi.icu/gtniluwnao.html

[D24] 字典 / Map 基本操作
来源：http://hz.hfpthk.cn/gtrunvznir.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guannengcc.top/gtyqdpdhdx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tianlin.xyz/gtplwzools.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yvedp.cn/gtunijypgo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.redwolf501.top/gtacmhxdyv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yonumen.top/gtfzqhgkev.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gtjfcyiqya.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.haohaochexian.top/gtkmhhxntk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sxryk.cn/gtkgskpxhn.html

[D25] Set 集合去重与交并差
来源：http://hz.chenjidiqi.icu/gttcfkohjk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhoulong.xyz/gtyizbdeal.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.vqdsnc.cn/gtcsivjaag.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cashguo.top/gtcuyqgybl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtrnbtorla.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ywan-chungtsiang.top/gtfamysgim.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xinyue.icu/gtegujzhuj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sxryk.cn/gtthrkcmvl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tanke756.top/gtfhyzcgaz.html

[D26] 数组转字符串
来源：http://hz.xuanzx.com/gtjneyfvqj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhixingplan.top/gteiofazun.html

PHP:  implode(", ", $arr);
来源：http://hz.zhijiandao.cn/gttfmdcjtq.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtknmauwud.html

TS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtclmogjfp.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtauqhpkmt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hammf.cn/gtqsrzfbdy.html

Ruby: arr.join(", ")
来源：http://hz.jinqigfzy.top/gtkjngkskf.html

C#:   string.Join(", ", list)
来源：http://hz.hywenlv.cn/gtovykevvy.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtypnnjhth.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gtbaytzndv.html

================================================================================
来源：http://hz.dashuyun.cn/gtzssvxqtj.html

[E01] 拼接字符串
来源：http://hz.zhijiandao.cn/gtccsssyze.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtufvisgvf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.iojbl.cn/gtbkjfvhco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtkctxvdhy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gtrkgivwlh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xuetiantiany.cn/gtvnvdycqt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhoulong.xyz/gtmrbfwhfb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.havefunace.top/gtfbvzcdkc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj20258888.top/gtprjdwcfj.html

[E02] 重复字符串
来源：http://hz.haohaochexian.top/gtovrgztaa.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtrwjqknjd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhixingplan.top/gtmodpwrsd.html

JS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtlbblgzfo.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtmtwmkiqu.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtujbcwuze.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yonumen.top/gtucporlhx.html

Ruby: "ab" * 3
来源：http://hz.hongshengwenyu.top/gtaagoehzd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtyaojvygb.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gtjowexjfm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daria6918.cn/gtmlnaywtu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtcbjcwfiv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shuidangran.top/gtobdgfvtk.html

TS:   s.slice(1, 4)
来源：http://hz.snrcjt.cn/gtrzplmgsl.html

Java: s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtruxmfuer.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.mhx1999.top/gtgsmevvde.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigfzy.top/gtkuaxphif.html

C#:   s.Substring(1, 3)
来源：http://hz.jyoumei.cn/gtkkixpuuo.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gtasnlbjdl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gogol.net.cn/gtogekmept.html

PHP:  strpos($s, "x");
来源：http://hz.cqqwz.cn/gtarpjaqlt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yvedp.cn/gtpbrnutyg.html

TS:   s.indexOf("x")
来源：http://hz.yueranfly.top/gtdmvtujcd.html

Java: s.indexOf("x")
来源：http://hz.0kj1m.cn/gtckeehmnl.html

Go:   strings.Index(s, "x")
来源：http://hz.xuanzx.com/gttvvfkeov.html

Ruby: s.index("x")
来源：http://hz.gzhubu.top/gtjtsgjxqk.html

C#:   s.IndexOf("x")
来源：http://hz.9152youxi.cn/gtspoundir.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.vqdsnc.cn/gtaqknuiaf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.dianchejie.cn/gtizoujbdf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.kuanghao11.cn/gtpuuvkukl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gtesblhsph.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhiwuduotai.top/gtcuqqvfty.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtuywvjswn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtfyqudweo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.aizwys.cn/gtzbcoxtal.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xuetiantiany.cn/gtposctznl.html

[E06] 替换子串
来源：http://hz.cucudq.cn/gtwkkqgfyf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.0kj1m.cn/gtmdsggexw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.feifeiyinyue.top/gticfqptvc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtwntjznnw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtigypezfj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtmousbshv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hnqzz.top/gtarghtwdb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinghuilouyu.cn/gthnskakwl.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtepumyzwm.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtricimcbc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nanxinkj.top/gtzzrkpqja.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtcamxvovv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhongyouzk.top/gtsstsxlqe.html

TS:   s.split(",")
来源：http://hz.yueranfly.top/gtxruhejql.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xylfe.cn/gtmykdsnie.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tanke756.top/gtselkstpf.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtngochzsv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtbesmbasa.html

[E08] 数组按分隔符合并
来源：http://hz.ydzc1.top/gtibebcmfa.html

Py:   ",".join(items)
来源：http://hz.chenjidiqi.icu/gtjkwluuob.html

PHP:  implode(",", $items);
来源：http://hz.guannengcc.top/gtdtfdsvwd.html

JS:   items.join(",")
来源：http://hz.jyoumei.cn/gtorlxvzln.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtsdlmeizx.html

Java: String.join(",", items)
来源：http://hz.iojbl.cn/gtydwfswpv.html

Go:   strings.Join(items, ",")
来源：http://hz.ppjwa.cn/gtvddxlgwj.html

Ruby: items.join(",")
来源：http://hz.jianghu66.top/gtrcldrlfi.html

C#:   string.Join(",", items)
来源：http://hz.zhengqikj.top/gticogsalu.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangkeji.top/gtvscccvot.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ppjwa.cn/gtytvhnbyd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhoulong.xyz/gtvlvluhkg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtmfdftkxj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xuanzx.com/gtvwaqiohc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.mhx1999.top/gtndugfaqe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.vqdsnc.cn/gtailsgiic.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ehwqpu.com/gtrdwbzdxe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtosbtuwvy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yueranfly.top/gtamntgvli.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtnmiwoyjg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.meibo888.top/gtrasoblvf.html

JS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtxdibkxsl.html

TS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtqmpdykrf.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtcjxkyepe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhixingplan.top/gtlsjocynn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtrxmpyxnm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.kuanghao11.cn/gtccywvwrn.html

[E11] 反转字符串
来源：http://hz.xziqi.cn/gtehrsteaw.html

Py:   s[::-1]
来源：http://hz.cucudq.cn/gtmcmobveq.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtjyvzijdw.html

JS:   [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtekhjpxeg.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtugcwynje.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gaohongyu789.top/gtbcdfmktm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuanzhike.top/gtjabhjdpw.html

Ruby: s.reverse
来源：http://hz.xylfe.cn/gthedrqqsy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gteqrqbhmr.html

[E12] 统计某字符出现次数
来源：http://hz.xinyue.icu/gthznuprqo.html

Py:   s.count("a")
来源：http://hz.zhongyouzk.top/gtjrvvtczx.html

PHP:  substr_count($s, "a");
来源：http://hz.kuanghao11.cn/gtddhrjyzp.html

JS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtfpetsqdp.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtnvynfksf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aibaodan.cn/gtktqdtatp.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtuhhyvuin.html

Ruby: s.count("a")
来源：http://hz.nanxuanxn.top/gtgverdice.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yongpay.top/gtwzopillo.html

[E13] 逐字符遍历
来源：http://hz.fengsongda.top/gtziyewwtd.html

Py:   for ch in s: print(ch)
来源：http://hz.shuidangran.top/gthmiyjlzm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gttyronoyh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtlsjgmzcs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnqzz.top/gtepueoejf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yanxiufei.cn/gtuhvsrkda.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fengsongda.top/gtsepwvbdi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtshecivzw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zycfv.cn/gtonbrurtz.html

[E14] URL 编码与 Base64
来源：http://hz.9152youxi.cn/gtnaughqlu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258888.top/gtjjlgrhan.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yangfankeji.com/gtscikwgsd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhoulong.xyz/gthjlkalbu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gtdawqxsmp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gtezmjhhar.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.quarkkingdee.top/gtvyrexnha.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuanzx.com/gtxzvuxsov.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yanxiufei.cn/gtjoslbwrs.html

[E15] HTML 转义 / 反转义
来源：http://hz.yanxiufei.cn/gtxqmhwiee.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.kuanghao11.cn/gtxalrogmu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daria6918.cn/gtqyjvuwfv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhijiandao.cn/gtplyrkfde.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenjidiqi.icu/gtngbrpfzi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258888.top/gtvulaihva.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.andypj.xyz/gtourozbdf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.feifeiyinyue.top/gtkloltxss.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuetiantiany.cn/gtzalkhgxi.html

[E16] 数字千分位
来源：http://hz.ywan-chungtsiang.top/gtsuaqwpxz.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtbazuwzqq.html

PHP:  number_format(1234567);
来源：http://hz.xingfuxueyuan.xyz/gtrcjtjhia.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtanfvkfxz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtcvtmujqv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.bjfxy.top/gtzncitgiv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xylfe.cn/gtromxglrg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.c1oappe.top/gtfsozpwfp.html

C#:   1234567.ToString("N0")
来源：http://hz.chenjidiqi.icu/gtjoyyrzdy.html

[E17] 首字母大写
来源：http://hz.nanxuanxn.top/gtefcxgdko.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pengpengdd.cyou/gtobvhnjwd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj20258.top/gtmyexgqlw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtlgyfhlqo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtvyuudtru.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtivcloisr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuanzx.com/gturkxgotk.html

Ruby: s.capitalize
来源：http://hz.kuanghao11.cn/gtysgzjlqa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtjsbzsdna.html

[E18] 模板占位符替换
来源：http://hz.sysykeji.top/gtnryvbrfs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gtjeiptlzs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.smart0.xyz/gtvjdnglbh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtoidimwun.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtlkyutztd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gotoacloud.top/gtaknckmjm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hywenlv.cn/gtrjvcvawy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhengqikj.top/gtrwbkmctm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xinyue.icu/gtujxhtitt.html

[E19] 多行文本按行拆分
来源：http://hz.aibaodan.cn/gtbamycdwn.html

Py:   s.splitlines()
来源：http://hz.ydjk.org.cn/gtawgannmq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.feifeiyinyue.top/gttolymljc.html

JS:   s.split(/\r?\n/)
来源：http://hz.ybcxt.top/gtgvzqtnzh.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtidnjktof.html

Java: s.lines().toList()
来源：http://hz.jinghuilouyu.cn/gtpzpiaykf.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtfygvxbjk.html

Ruby: s.lines
来源：http://hz.aibaodan.cn/gtareosrkw.html

C#:   s.Split('\n')
来源：http://hz.andypj.xyz/gtldkplggy.html

[E20] 判断字符串是否为空
来源：http://hz.zycfv.cn/gtrkgjneqs.html

Py:   if not s:
来源：http://hz.chenlongwang.top/gtasmuxjkb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gtutflfnyr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gtzjcvdlho.html

TS:   if (s === "") {}
来源：http://hz.yuxming.cn/gtaveyhnww.html

Java: if (s.isEmpty()) {}
来源：http://hz.zycfv.cn/gtcjvhhwhm.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtchbearhw.html

Ruby: if s.empty?
来源：http://hz.hysaishi.cn/gtqbkzmfsw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ivvv.top/gtovvopocs.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtfmkdfepl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnqzz.top/gthljkfiek.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aizwys.cn/gtjaijrcpe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtmjaitxpt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtfgmbfmlw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtoewcpjow.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gthksgtrct.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yanxiufei.cn/gtsavbdqrl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtcayrjhqj.html

[E22] 字节长度与字符长度
来源：http://hz.chenjidiqi.icu/gtdzjikjnx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daxiang520.top/gtroivuvjj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gtdmpnagae.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtbpnbjbxv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtgbnigwns.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigfzy.top/gthrhpyzwk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangdashe.top/gtxqyplkwy.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtskmwrryk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gtnqhrthxd.html

================================================================================
来源：http://hz.chenzaomai.com/gtcemnigyt.html

F. 文件与目录
来源：http://hz.gogol.net.cn/gtkmqoepdn.html

================================================================================
来源：http://hz.wangdashe.top/gtoyrmhlee.html

[F01] 读取整个文件
来源：http://hz.havefunace.top/gtfqprulfd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtwrcvhxsm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yueranfly.top/gtkbxlzrqv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinyuanbaomall.cn/gtqdwxflyt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtxjmeubum.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtjkuoqakp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.snrcjt.cn/gtslolihfx.html

Ruby: File.read("a.txt")
来源：http://hz.birdmap.top/gtdyyhilat.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuxming.cn/gtxhraemgh.html

[F02] 逐行读取文件
来源：http://hz.yj20258888.top/gtaebbujav.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtrsicwbld.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yvedp.cn/gtkkonzbwm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtqjrvymlp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtyzkglajz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtunxjhvrs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtfufrvdmx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gttnqnuxcv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ywan-chungtsiang.top/gtixlrtxxw.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtsvyhwufx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yongpay.top/gtiqsvdiol.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtvnpenocr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtriuaoyha.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtzvczvefo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jlsjyb.cn/gtmudgsswa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.kuanghao11.cn/gtropsblxt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tianlin.xyz/gtxmglccsq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj202588.top/gtifvwyxha.html

[F04] 追加写入文件
来源：http://hz.c1oappe.top/gtmixyguhs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gtfoqrbqlg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgufenzy.top/gtvogtakti.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtmwpnrjwi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtwwmfjknc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guannengcc.top/gtnmzffslw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgufenzy.top/gtxurvtghm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258.top/gtjrctvufp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nwbrower.top/gtkllqhfqf.html

[F05] 判断文件或目录是否存在
来源：http://hz.havefunace.top/gtsbwajcpt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hnxiangtu.top/gtrstilrgz.html

PHP:  file_exists("a.txt");
来源：http://hz.redwolf501.top/gtvbzfqfwg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtewstfsom.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtdsljibys.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtqzrnuivh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yueranfly.top/gtpcujgcfc.html

Ruby: File.exist?("a.txt")
来源：http://hz.kuanghao11.cn/gtozbspjyj.html

C#:   File.Exists("a.txt")
来源：http://hz.zycfv.cn/gtrqagmqzx.html

[F06] 删除文件
来源：http://hz.tian-w.cn/gtwndoyizf.html

Py:   os.remove("a.txt")
来源：http://hz.316326.xyz/gtcehqpwlj.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtqmjztlts.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtooacbtwn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtiavqocug.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gteafbxcyp.html

Go:   os.Remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtffqfuqsd.html


<!-- 参考信息 -->