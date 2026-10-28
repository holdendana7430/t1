代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xylfe.cn/gtsajwwjek.html

[D20] 统计每个元素出现次数
来源：http://hz.jiagoushi.top/gtrkpbeflt.html

Py:   Counter(arr)
来源：http://hz.sxryk.cn/gtzfhrjdhi.html

PHP:  array_count_values($arr);
来源：http://hz.zhengqikj.top/gtsdiucthj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtdpfgxhrx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtcqeksisk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenjidiqi.icu/gtypcxuauc.html

Go:   // 手写 map[T]int
来源：http://hz.tianlin.xyz/gteppdhchh.html

Ruby: arr.tally
来源：http://hz.hongshengwenyu.top/gtcpqptejd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.kuanghao11.cn/gtjxoycevi.html

[D21] 判断是否包含某元素
来源：http://hz.zhijiandao.cn/gtfmnnedae.html

Py:   x in arr
来源：http://hz.yvedp.cn/gteehwnkva.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhongyouzk.top/gtnosyxjvv.html

JS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtlybusdze.html

TS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtturithyn.html

Java: list.contains(x)
来源：http://hz.xziqi.cn/gtuyeeqzts.html

Go:   slices.Contains(arr, x)
来源：http://hz.yongpay.top/gtrbtgpory.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtvxetpzry.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtzquzzems.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtuiomvkmp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jlsjyb.cn/gtcaljzxcr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yueranfly.top/gtfgdkmftj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hammf.cn/gtawvawkud.html

TS:   [...arr];
来源：http://hz.aibaodan.cn/gtgqnxkali.html

Java: new ArrayList<>(list);
来源：http://hz.sufxvd.cn/gtpfbqvymv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nwbrower.top/gtplufhmue.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yvedp.cn/gtcsnywxof.html

C#:   new List<int>(list);
来源：http://hz.guowangkeji.top/gtmverilot.html

[D23] reduce 累积计算
来源：http://hz.shzxlz.cn/gtdmwrouha.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigfzy.top/gtakdaxqbb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.guowangkeji.top/gtpsnruehd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtlljiqfgp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenzaomai.com/gtjerokvti.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.bjfxy.top/gtfpvgaxzr.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gtiabvmpcf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gtjtjomzic.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yangfankeji.com/gtdesiufpq.html

[D24] 字典 / Map 基本操作
来源：http://hz.tanke756.top/gtqcygmcfd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinyuanbaomall.cn/gtfaljkvqk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daria6918.cn/gtcsxbtsyl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.quarkkingdee.top/gtigxmobrf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangdashe.top/gtuofgmfhm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhengqikj.top/gtwrhuwugs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yvedp.cn/gtuktchxqn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.c1oappe.top/gtitvvqozb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.c1oappe.top/gtvclwzzpw.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gttpmpgynv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.52xcode.cn/gtvtjdznsa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhaomingkeji.xyz/gtotifoyxu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cheryme.top/gtzxkvrnmx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gtubktaobr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ywan-chungtsiang.top/gtkpweipso.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hysaishi.cn/gtzekmimjh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxinkj.top/gtwmflavet.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.bjfxy.top/gtznvyskqc.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gthliszqcr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yvedp.cn/gtzlwigznk.html

PHP:  implode(", ", $arr);
来源：http://hz.iojbl.cn/gtbfefcnzi.html

JS:   arr.join(", ")
来源：http://hz.yj20258888.top/gteyegbxvu.html

TS:   arr.join(", ")
来源：http://hz.dashuyun.cn/gtybsnbrck.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtftrnzgeg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinyuanbaomall.cn/gtqmroyvpe.html

Ruby: arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtntuqhctp.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtvglywota.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqbzbhnlw.html

E. 字符串处理
来源：http://hz.cqqwz.cn/gtxcqzwnpq.html

================================================================================
来源：http://hz.snrcjt.cn/gtnuvjodpy.html

[E01] 拼接字符串
来源：http://hz.dashuyun.cn/gtkapkcveq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.haohaochexian.top/gtoljrvixo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnxiangtu.top/gthoblnnty.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtmwupxfpa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtshyiwcov.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydjk.org.cn/gtwymllbkn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cdnleiting.top/gthvxluejm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zycfv.cn/gtpumdokvm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.redwolf501.top/gtgyclspcb.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtqepfpfox.html

Py:   "ab" * 3
来源：http://hz.yj20258.top/gtumybsfku.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinghuilouyu.cn/gtyppdzgwo.html

JS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtjwrzirqk.html

TS:   "ab".repeat(3)
来源：http://hz.xylfe.cn/gtpgdqqnaz.html

Java: "ab".repeat(3)
来源：http://hz.xylfe.cn/gtrzxoxqel.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangshuangyany.cn/gtqrmfcrgv.html

Ruby: "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gtstlpmriw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tianlin.xyz/gtqbrogyga.html

[E03] 截取子串
来源：http://hz.jinqigufen.top/gtmgjakmeq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.iojbl.cn/gtqtvusyen.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gotoacloud.top/gthktelxer.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zycfv.cn/gtfaqenqbo.html

TS:   s.slice(1, 4)
来源：http://hz.pycfn.com/gtlafclney.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtinritxms.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shanyushiyangtech.top/gtbggsnunj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuanzx.com/gtrwghdzkp.html

C#:   s.Substring(1, 3)
来源：http://hz.xinyue.icu/gtbxsetkti.html

[E04] 查找子串位置
来源：http://hz.iojbl.cn/gtwalegcgm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yuxming.cn/gtalifbkvi.html

PHP:  strpos($s, "x");
来源：http://hz.aibaodan.cn/gtjpkeunqy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nwbrower.top/gtfniyakir.html

TS:   s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtzrphrfgi.html

Java: s.indexOf("x")
来源：http://hz.cdnleiting.top/gtjjsjkdyg.html

Go:   strings.Index(s, "x")
来源：http://hz.jinghuilouyu.cn/gtvivrwejk.html

Ruby: s.index("x")
来源：http://hz.hnqzz.top/gtqklzryfy.html

C#:   s.IndexOf("x")
来源：http://hz.cheryme.top/gtxodbqorv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtoneldkdc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hywenlv.cn/gtyouohcnc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pycfn.com/gtveukcatz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtvpqhckeq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xziqi.cn/gtxgvmwfxj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gtuazppftp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.smart0.xyz/gtmlywfmqs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgfzy.top/gtjlfsxuns.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.daria6918.cn/gtylkujuve.html

[E06] 替换子串
来源：http://hz.jlsjyb.cn/gtvohzxjhy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.iojbl.cn/gtbumlrxoe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.c1oappe.top/gtjqlehxiz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtctzenffs.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtqptxqybe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gthlhbhnrn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ivvv.top/gtgddawiuz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhongyouzk.top/gtfsrjjeuw.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtlwpztfzx.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gtravozuyg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.andypj.xyz/gtybuahkox.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.feifeiyinyue.top/gtzegirmqr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hammf.cn/gtwyeeevkw.html

TS:   s.split(",")
来源：http://hz.jqgfzy.top/gtpspqwlzs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shzxlz.cn/gtjmtzjbbb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtvjliwvlj.html

Ruby: s.split(",");  s.split
来源：http://hz.cqqwz.cn/gtctrtxhjt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtrdonnwjk.html

[E08] 数组按分隔符合并
来源：http://hz.havefunace.top/gtvlcgqxsp.html

Py:   ",".join(items)
来源：http://hz.pycfn.com/gtijtqtkvg.html

PHP:  implode(",", $items);
来源：http://hz.zdqjudy.top/gtdupgbyav.html

JS:   items.join(",")
来源：http://hz.yueranfly.top/gtuinnujfc.html

TS:   items.join(",")
来源：http://hz.c1oappe.top/gtonbumzfn.html

Java: String.join(",", items)
来源：http://hz.nanxuanxn.top/gtblcovowp.html

Go:   strings.Join(items, ",")
来源：http://hz.meibo888.top/gtkailpknk.html

Ruby: items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtplqaxfoy.html

C#:   string.Join(",", items)
来源：http://hz.shzxlz.cn/gtgjvcrxhj.html

[E09] 去除所有空白字符
来源：http://hz.zhoulong.xyz/gtplmilnzl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sufxvd.cn/gtcocccley.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenzaomai.com/gtjkxtrbdi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtbucscalc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gthfmzoqxp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cdnleiting.top/gtmdmosqqs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.vqdsnc.cn/gttabytlmc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.bjfxy.top/gtltbinrvy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hongshengwenyu.top/gtunertyoy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.havefunace.top/gtmnytolfe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zdqjudy.top/gtoauprmfx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jqgfzy.top/gtbiwtsvag.html

JS:   "7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtvhkbwfqo.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtydgljjyw.html

Java: String.format("%03d", 7)
来源：http://hz.yj202588.top/gthfwciuzy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtjvhjotjn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtijvrocqz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinyuanbaomall.cn/gtqzdmjzbq.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtmrlwubxx.html

Py:   s[::-1]
来源：http://hz.chenlongwang.top/gtthntxjna.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtvarmlbju.html

JS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gthvjzoajy.html

TS:   [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtikspumuv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnqzz.top/gtlzfqihmw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258.top/gtalgskpwk.html

Ruby: s.reverse
来源：http://hz.zhixingplan.top/gthfvjgnna.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtmsddhgoo.html

[E12] 统计某字符出现次数
来源：http://hz.xingfuxueyuan.xyz/gtviwoxurl.html

Py:   s.count("a")
来源：http://hz.quarkkingdee.top/gttpxpbmqi.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtxhpgkbgj.html

JS:   s.split("a").length - 1
来源：http://hz.zhixingplan.top/gtsrxuyzye.html

TS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtttyzpysj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fengsongda.top/gtrpakycnz.html

Go:   strings.Count(s, "a")
来源：http://hz.sysykeji.top/gtticauabu.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gtlmxjcugp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj202588.top/gtkbvflvda.html

[E13] 逐字符遍历
来源：http://hz.jqgfzy.top/gtinpxzviy.html

Py:   for ch in s: print(ch)
来源：http://hz.jyoumei.cn/gtxxgogbsy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ybcxt.top/gtphphapmf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtbiogwlhw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtbuldsski.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tian-w.cn/gtywovmwhn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cheryme.top/gttkopzamq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.mhx1999.top/gttxcwghlf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtvevcjdai.html

[E14] URL 编码与 Base64
来源：http://hz.yongpay.top/gtsxakntyb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zycfv.cn/gtvovuhocc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cdnleiting.top/gtmkuikknx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.kuanghao11.cn/gtqrxilzwp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtchjnreaq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigufen.top/gtwnztwjxc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ywan-chungtsiang.top/gtbvltpnld.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tanke756.top/gtpfxbxgwz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.c1oappe.top/gtoiumkdpr.html

[E15] HTML 转义 / 反转义
来源：http://hz.ehwqpu.com/gtypwteeoi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gotoacloud.top/gtkvbkiwoz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhoulong.xyz/gtkgjsbpxq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nanxinkj.top/gtkaunmzes.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.snrcjt.cn/gtlozqcaiy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.svipenyu.cn/gtfynyswlg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.mhx1999.top/gtjlusaqej.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ehwqpu.com/gtqgrxcews.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtjubhfqrv.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtyvbzrbac.html

Py:   f"{1234567:,}"
来源：http://hz.xylfe.cn/gtrlfxwriz.html

PHP:  number_format(1234567);
来源：http://hz.yj20258.top/gtolmwzirq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtozjrxydn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtjpedntne.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtfjnbjuee.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xziqi.cn/gtlsuioyya.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtacexfasg.html

C#:   1234567.ToString("N0")
来源：http://hz.gzhubu.top/gtvqonsgau.html

[E17] 首字母大写
来源：http://hz.birdmap.top/gtncxbwfoj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.quarkkingdee.top/gtxvqbigxs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jiagoushi.top/gtnhmpclpj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtdljhgjva.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtvemtwbop.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhengqikj.top/gtxayuzgca.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shuidangran.top/gtehhydqwn.html

Ruby: s.capitalize
来源：http://hz.shanyushiyangtech.top/gtszikdyzk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cashguo.top/gtnacwclth.html

[E18] 模板占位符替换
来源：http://hz.gaohongyu789.top/gtxjbludyc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gogol.net.cn/gtrgkrjffh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.birdmap.top/gtgpakudsi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aizwys.cn/gtpqosgdze.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtamruokhx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtbdcfqvuo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shuidangran.top/gtlujbcgeg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtfyncizng.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zycfv.cn/gtzgovfcct.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gtdvkdxmju.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtxsrnqqta.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhijiandao.cn/gtrbjjhgim.html

JS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtajppvzyh.html

TS:   s.split(/\r?\n/)
来源：http://hz.jiagoushi.top/gtgfnaiith.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gtmejctxhn.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtyhaywokz.html

Ruby: s.lines
来源：http://hz.kuanghao11.cn/gtmvzhiuxr.html

C#:   s.Split('\n')
来源：http://hz.dashuyun.cn/gtgsfuojtq.html

[E20] 判断字符串是否为空
来源：http://hz.jqgufenzy.top/gtcfpeckmv.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtyzxnjsye.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydzc1.top/gttadoesku.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtewzwkrkl.html

TS:   if (s === "") {}
来源：http://hz.jianghu66.top/gtjdffahch.html

Java: if (s.isEmpty()) {}
来源：http://hz.fzhhl.top/gtngdunvmi.html

Go:   if s == "" {}
来源：http://hz.bjfxy.top/gteuqzefkj.html

Ruby: if s.empty?
来源：http://hz.svipenyu.cn/gtyuykcvsr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.9152youxi.cn/gtcwrehuov.html

[E21] 超长截断加省略号
来源：http://hz.jqgufenzy.top/gtoebnngxi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtipuassif.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gtdkmffeef.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtohqbynto.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtbfyvveno.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtefzofdot.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtswbizysy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangdashe.top/gtbdcqtxsw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtizimcrfc.html

[E22] 字节长度与字符长度
来源：http://hz.havefunace.top/gtgsoefucs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gtmnxtqita.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gthdbcriqa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtoyvyaxhy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtfejzpehn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ivvv.top/gtkrgycyzs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zdqjudy.top/gtoydaozzu.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuanzx.com/gtuctnknwr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dashuyun.cn/gtjjbulumq.html

================================================================================
来源：http://hz.cheryme.top/gtkfrohysj.html

F. 文件与目录
来源：http://hz.sysykeji.top/gtjkwzogmw.html

================================================================================
来源：http://hz.gzhubu.top/gtgyjchagg.html

[F01] 读取整个文件
来源：http://hz.shuidangran.top/gtxvbwnxwq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.haohaochexian.top/gtujscnfuk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.0kj1m.cn/gtziebsuhf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tanke756.top/gtfjwyencg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtxrnsmxjb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtbhmejtad.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigfzy.top/gtvcrsycut.html

Ruby: File.read("a.txt")
来源：http://hz.ydjk.org.cn/gtedoicffa.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhixingplan.top/gtzvisqggf.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gtewkghztm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenjidiqi.icu/gtzqtrswtj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cqqwz.cn/gtslfijzgl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtiplhstjv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtbqosqzxn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtnthszzqt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xylfe.cn/gtrjoznnzl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gthsqtkzji.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pengpengdd.cyou/gtwpferrkg.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtmqucszfj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sufxvd.cn/gtbnyrofvy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.iojbl.cn/gtowahovpb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtnodaqgyx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gteissrxat.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gthybcxhht.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.meibo888.top/gtsewugepd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtjiojtxjd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtxznmcuqj.html

[F04] 追加写入文件
来源：http://hz.jinqigufen.top/gtyhyhcuwl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nwbrower.top/gtsgpsfieq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtcgvsacmt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtzwfyacnh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gticnaghro.html


<!-- 参考信息 -->