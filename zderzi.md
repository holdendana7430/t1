代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fengsongda.top/gtkyoaawox.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtsajoaitf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangshuangyany.cn/gtjatbtscq.html

Go:   // 手写循环累加
来源：http://hz.yj20258.top/gtkhcxzcbl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.snrcjt.cn/gtvrfnrazh.html

C#:   list.Sum();  list.Average()
来源：http://hz.316326.xyz/gtkrfxujdi.html

[D17] 最大值与最小值
来源：http://hz.jqgufenzy.top/gtbzqunyjp.html

Py:   max(arr);  min(arr)
来源：http://hz.shuidangran.top/gtamjypmss.html

PHP:  max($arr);  min($arr);
来源：http://hz.fengsongda.top/gttqkfhehe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cdnleiting.top/gtraftvvus.html

TS:   Math.max(...arr);
来源：http://hz.smart0.xyz/gtsbnwmbxf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.pycfn.com/gttgvscigf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ybcxt.top/gtfamluhvk.html

Ruby: arr.max;  arr.min
来源：http://hz.yuxming.cn/gtzjvdjyrs.html

C#:   list.Max();  list.Min()
来源：http://hz.cqqwz.cn/gturupwpro.html

[D18] 扁平化嵌套数组
来源：http://hz.sweek.top/gtomhvnvqf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtsuuyrbzy.html

PHP:  array_merge(...$nested);
来源：http://hz.chenzaomai.com/gtzhnueslt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pengpengdd.cyou/gtfsepmmlt.html

TS:   nested.flat();
来源：http://hz.mhx1999.top/gtekhjsimj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ywan-chungtsiang.top/gtmiofapak.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtzeznborf.html

Ruby: nested.flatten
来源：http://hz.aibaodan.cn/gtzgaopvfo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jiagoushi.top/gtoeqbkhio.html

[D19] 按字段分组
来源：http://hz.mhx1999.top/gtbnipcipz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtasmbrcqu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.quarkkingdee.top/gtagsaghdq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yueranfly.top/gtgiqwbrpz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtunovpldp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtcslwfdzc.html

Go:   // 手写 map[string][]T
来源：http://hz.xuanzx.com/gtquntnvpe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gttmawgejn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.haohaochexian.top/gtijwywmdk.html

[D20] 统计每个元素出现次数
来源：http://hz.ppjwa.cn/gtwmaegltv.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtdgsryteg.html

PHP:  array_count_values($arr);
来源：http://hz.nanxuanxn.top/gtorxccefi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gthiyukmfz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gteoyhrick.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ehwqpu.com/gtpreuinir.html

Go:   // 手写 map[T]int
来源：http://hz.yonumen.top/gtkqvvnlyr.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtmwkeqjbu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.c1oappe.top/gtmvelmisi.html

[D21] 判断是否包含某元素
来源：http://hz.ppjwa.cn/gtgipprkqe.html

Py:   x in arr
来源：http://hz.hnqzz.top/gtqogbwvoh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shangyingyoupin.top/gtnqiifggx.html

JS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtlmrdbkka.html

TS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtmxoupdgh.html

Java: list.contains(x)
来源：http://hz.gogol.net.cn/gtybnzfyio.html

Go:   slices.Contains(arr, x)
来源：http://hz.cheryme.top/gtklejshwj.html

Ruby: arr.include?(x)
来源：http://hz.shuidangran.top/gthdixknpk.html

C#:   list.Contains(x)
来源：http://hz.zhongyouzk.top/gtzztthyxh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.52xcode.cn/gtfvlrhbwy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dianchejie.cn/gtscjhqznj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nanxinkj.top/gtipeqvfwu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gogol.net.cn/gtlognlvwh.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gthxuakgjh.html

Java: new ArrayList<>(list);
来源：http://hz.xingfuxueyuan.xyz/gtzikjoihc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sufxvd.cn/gtblnlkohy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.redwolf501.top/gtlnuituif.html

C#:   new List<int>(list);
来源：http://hz.shangyingyoupin.top/gtryusakwi.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gtdhqlfvjs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhengqikj.top/gtakayloga.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.havefunace.top/gtbjbniokh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtsacmkysf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtwxdhnmht.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigfzy.top/gtsbsuzfld.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtofrzgpcw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.daria6918.cn/gtqxuedpbq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xingfuxueyuan.xyz/gtydohuawh.html

[D24] 字典 / Map 基本操作
来源：http://hz.tianlin.xyz/gtvfgkylls.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenjidiqi.icu/gtnbyffuvq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gtzhkrkjzi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guannengcc.top/gtvzhplzaa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgufenzy.top/gtdupsgixa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ppjwa.cn/gtmurhzfwy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.vqdsnc.cn/gtgyruozqb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydzc1.top/gtcnpukyys.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gtakffeasv.html

[D25] Set 集合去重与交并差
来源：http://hz.xylfe.cn/gtkeujrvfs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.andypj.xyz/gtogmxyxdg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinyuanbaomall.cn/gtzialpwoj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.smart0.xyz/gtbsyvoanz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhongyouzk.top/gtohbislst.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtqynofvmv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj202588.top/gtkarmmkns.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xingfuxueyuan.xyz/gtkljpbyft.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.snrcjt.cn/gtkjiwpxmy.html

[D26] 数组转字符串
来源：http://hz.zhoulong.xyz/gtqrhfhrkn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xinyue.icu/gtwiloyukm.html

PHP:  implode(", ", $arr);
来源：http://hz.jlsjyb.cn/gtrfqzvhdp.html

JS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtklorycai.html

TS:   arr.join(", ")
来源：http://hz.haohaochexian.top/gtpunndmgm.html

Java: String.join(", ", list)
来源：http://hz.fengsongda.top/gthiyqtfgo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtisgtvaei.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gtcnraulry.html

C#:   string.Join(", ", list)
来源：http://hz.jqgufenzy.top/gtwyfzhmol.html

================================================================================
来源：http://hz.iojbl.cn/gtjkgczxxg.html

E. 字符串处理
来源：http://hz.zdqjudy.top/gtiyvyheqo.html

================================================================================
来源：http://hz.zycfv.cn/gtjqhgdnlm.html

[E01] 拼接字符串
来源：http://hz.nanxuanxn.top/gtaqajkyem.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuanzx.com/gtauiibthj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xziqi.cn/gtkqjddpeb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gtjuipjukz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtjgqfzvdg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.52xcode.cn/gtzmpzlgtc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gaohongyu789.top/gtozwauahc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sweek.top/gtwpaylolk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.smart0.xyz/gtkfpcvnnl.html

[E02] 重复字符串
来源：http://hz.dianchejie.cn/gtawmczuhp.html

Py:   "ab" * 3
来源：http://hz.52xcode.cn/gtpisahmwk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guowangkeji.top/gtexyzgiwb.html

JS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtkvujzhbi.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtbhprmyki.html

Java: "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtfkobdfwv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sxryk.cn/gtxwnrtwoo.html

Ruby: "ab" * 3
来源：http://hz.guowangkeji.top/gtmqvnuhjm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xinyue.icu/gtguoyekrg.html

[E03] 截取子串
来源：http://hz.mhx1999.top/gtottipnlf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuanzhike.top/gttlkjgoof.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sufxvd.cn/gtjbehtuco.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ydzc1.top/gtbzusgfsj.html

TS:   s.slice(1, 4)
来源：http://hz.pengpengdd.cyou/gtjgtpdwzn.html

Java: s.substring(1, 4)
来源：http://hz.hywenlv.cn/gtiihkcior.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gogol.net.cn/gtnzheqgns.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shzxlz.cn/gtlalzkudh.html

C#:   s.Substring(1, 3)
来源：http://hz.zycfv.cn/gtjmvsozxn.html

[E04] 查找子串位置
来源：http://hz.dianchejie.cn/gtgrkbvaiv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtushoifkx.html

PHP:  strpos($s, "x");
来源：http://hz.aizwys.cn/gtazjxnvmp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yvedp.cn/gtqbxmjaqj.html

TS:   s.indexOf("x")
来源：http://hz.hysaishi.cn/gtcjprbqvd.html

Java: s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtroqpyfni.html

Go:   strings.Index(s, "x")
来源：http://hz.bjfxy.top/gtbhnshgdm.html

Ruby: s.index("x")
来源：http://hz.wangdashe.top/gtrikbpbjo.html

C#:   s.IndexOf("x")
来源：http://hz.snrcjt.cn/gtyiyljboj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinyuanbaomall.cn/gtnmsewrsn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hammf.cn/gtigoprklx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.feifeiyinyue.top/gtuqwelatr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhiwuduotai.top/gtitszaapv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cashguo.top/gtokaipcvt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtuzuzslke.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shangyingyoupin.top/gtkpnjsuky.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenzaomai.com/gtvgqeyzez.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.smart0.xyz/gtciwsoofl.html

[E06] 替换子串
来源：http://hz.tian-w.cn/gtgkxhtjri.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhongyouzk.top/gtgcuuigjq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.0kj1m.cn/gtpgvuocau.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtnbfttahk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtpuatexil.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtyclfpqfu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tian-w.cn/gtaoeskpve.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gotoacloud.top/gtjmiqphnd.html

C#:   s.Replace("a", "b")
来源：http://hz.yanxiufei.cn/gtaoicbfls.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gtnzsyntzo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.mhx1999.top/gthqyqvxgg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yonumen.top/gtltkszbgt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.quarkkingdee.top/gtjyvofsjo.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gtpxyznmwr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.redwolf501.top/gtbxslhqki.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nwbrower.top/gtafilajcy.html

Ruby: s.split(",");  s.split
来源：http://hz.xinyue.icu/gtyvtcmlwz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jianghu66.top/gtadjcmfaq.html

[E08] 数组按分隔符合并
来源：http://hz.zhengqikj.top/gtvpweqwgf.html

Py:   ",".join(items)
来源：http://hz.shangyingyoupin.top/gthfayjfqa.html

PHP:  implode(",", $items);
来源：http://hz.sufxvd.cn/gtgaanazoj.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtkfegnmyo.html

TS:   items.join(",")
来源：http://hz.zdqjudy.top/gtehguyhjc.html

Java: String.join(",", items)
来源：http://hz.zhaomingkeji.xyz/gttvzjugqm.html

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gtjzlpsigz.html

Ruby: items.join(",")
来源：http://hz.bjfxy.top/gtfshodose.html

C#:   string.Join(",", items)
来源：http://hz.yj202588.top/gtylogzbtj.html

[E09] 去除所有空白字符
来源：http://hz.smart0.xyz/gtcgoxtwux.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258.top/gtsizigham.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtzqmxnlay.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtrrrqnnec.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtakwxrxww.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.havefunace.top/gtcxbvmgyb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.smart0.xyz/gtvyxkeisr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtjwfgslji.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jyoumei.cn/gtafpouhvg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtmlzsajjx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtuaaglcvo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtyjnvmhpq.html

JS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtvniahlqj.html

TS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtnonulumx.html

Java: String.format("%03d", 7)
来源：http://hz.zhoulong.xyz/gttfjgnifn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sysykeji.top/gtcaymwnbg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtqjambkca.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhongyouzk.top/gtoeveznki.html

[E11] 反转字符串
来源：http://hz.haohaochexian.top/gtnlzifivb.html

Py:   s[::-1]
来源：http://hz.yongpay.top/gtohqkigst.html

PHP:  strrev($s);
来源：http://hz.wangdashe.top/gtxilkxfub.html

JS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtfzalxhmx.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtfrsjrdad.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtdfbzvwpo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtylcftycz.html

Ruby: s.reverse
来源：http://hz.cheryme.top/gtokklpadr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtsjdtlrwz.html

[E12] 统计某字符出现次数
来源：http://hz.andypj.xyz/gtxqrnxnqz.html

Py:   s.count("a")
来源：http://hz.nwbrower.top/gtkjkomcla.html

PHP:  substr_count($s, "a");
来源：http://hz.cheryme.top/gtruikyhnu.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtayvmryqz.html

TS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtsudesxsg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gzhubu.top/gtugwafawg.html

Go:   strings.Count(s, "a")
来源：http://hz.hywenlv.cn/gtsztkrvgv.html

Ruby: s.count("a")
来源：http://hz.xziqi.cn/gtqjvljwvv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhaomingkeji.xyz/gtajurlqxt.html

[E13] 逐字符遍历
来源：http://hz.aizwys.cn/gtsrjcnzog.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gtbmplgwsz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sysykeji.top/gtagrvxfaw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtajaowapc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtrspwehkk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.quarkkingdee.top/gtshjukohh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtcfndiecg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gtjipwjxku.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtzfizrqva.html

[E14] URL 编码与 Base64
来源：http://hz.c1oappe.top/gtrzkobpxo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenjidiqi.icu/gtffjtokwe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gtvthgiwnb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gtmqfdroda.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ywan-chungtsiang.top/gtttjqnspa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinghuilouyu.cn/gtbpeixeyt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gtpcowxiic.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cheryme.top/gtojisbumz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.dashuyun.cn/gtnfypaasy.html

[E15] HTML 转义 / 反转义
来源：http://hz.hfpthk.cn/gtauypwobs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gtgaerylpk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtrqizgtlx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gotoacloud.top/gtffezyyby.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtohjlgasy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.andypj.xyz/gtitxvwzsy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtiwqvwriu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cdnleiting.top/gtsivgdqyb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydjk.org.cn/gtzjmjiopw.html

[E16] 数字千分位
来源：http://hz.jinyuanbaomall.cn/gtzishkzvy.html

Py:   f"{1234567:,}"
来源：http://hz.cdnleiting.top/gtzziqrrfe.html

PHP:  number_format(1234567);
来源：http://hz.ivvv.top/gtnpxenaec.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtvokxfxeh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtcdhizsiv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydjk.org.cn/gttyieytba.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtzbpojncj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hysaishi.cn/gtqqvwlwgt.html

C#:   1234567.ToString("N0")
来源：http://hz.hnxiangtu.top/gtsvzbkitw.html

[E17] 首字母大写
来源：http://hz.0kj1m.cn/gtpkrcvijd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtedtdiduq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.fzhhl.top/gtrchqeqdv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtcepxjdkw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtrbdgucjn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydzc1.top/gtnotvband.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtnpljndqn.html

Ruby: s.capitalize
来源：http://hz.sweek.top/gtsjfexmfr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aizwys.cn/gtbhtyknps.html

[E18] 模板占位符替换
来源：http://hz.c1oappe.top/gtykniztyx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.smart0.xyz/gtbirtpvwx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.svipenyu.cn/gtagxpsikp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtupmouyuk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtmphufcji.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cdnleiting.top/gtynybmxdh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yueranfly.top/gtutdepmvt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.0kj1m.cn/gtivsfjxzo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hongshengwenyu.top/gttxvqhrvu.html

[E19] 多行文本按行拆分
来源：http://hz.cdnleiting.top/gtfhheoxyh.html

Py:   s.splitlines()
来源：http://hz.jinyuanbaomall.cn/gtbylxstxp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gteunuebst.html

JS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtuhtxptsz.html

TS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtjsdgrlug.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gtpezdvytq.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gtgvxinevh.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gtfsolygij.html

C#:   s.Split('\n')
来源：http://hz.sxryk.cn/gtqnfvstrg.html

[E20] 判断字符串是否为空
来源：http://hz.daria6918.cn/gtstcfyaug.html

Py:   if not s:
来源：http://hz.tianlin.xyz/gtfghsufzr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gaohongyu789.top/gtfjzzytey.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pengpengdd.cyou/gtnvjshbiw.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gtotizjbwy.html

Java: if (s.isEmpty()) {}
来源：http://hz.andypj.xyz/gtfmuzecfl.html

Go:   if s == "" {}
来源：http://hz.zycfv.cn/gteybtxibv.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gtkyaankfz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gtcvbeyqlb.html

[E21] 超长截断加省略号
来源：http://hz.gotoacloud.top/gtahvwsxwy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhixingplan.top/gtfsvfpigs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aizwys.cn/gtdyjfvjgj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtvgcyyqpt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtkovlpdbz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtlbemimoz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydjk.org.cn/gticilqryo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jiagoushi.top/gtbhcezqwb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtygbluxas.html

[E22] 字节长度与字符长度
来源：http://hz.aibaodan.cn/gtecqsrbby.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.snrcjt.cn/gthdvwqlhb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtdflzghxp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtcgjdxufd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtklatmzog.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtsdqgttvf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gtqdslaozx.html

Ruby: s.bytesize;  s.length
来源：http://hz.jyoumei.cn/gtatuiggvg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.kuanghao11.cn/gtguxroqwi.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtuxbpvuyi.html

F. 文件与目录
来源：http://hz.shuidangran.top/gtkgyqiuue.html

================================================================================
来源：http://hz.tanke756.top/gtrtyylqyi.html


<!-- 参考信息 -->