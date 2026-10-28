代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xylfe.cn/gtmsytqvju.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtnaakrcmf.html

C#:   list.Max();  list.Min()
来源：http://hz.zhengqikj.top/gtkiumkpzu.html

[D18] 扁平化嵌套数组
来源：http://hz.guowangkeji.top/gtdnijiryx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cdnleiting.top/gtrosastny.html

PHP:  array_merge(...$nested);
来源：http://hz.zhengqikj.top/gtjmzqttiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhiwuduotai.top/gtefahpppc.html

TS:   nested.flat();
来源：http://hz.smart0.xyz/gtyurulili.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnxiangtu.top/gtgvluxavt.html

Go:   // 手写双层循环
来源：http://hz.jinyuanbaomall.cn/gtdknqghlq.html

Ruby: nested.flatten
来源：http://hz.nanxuanxn.top/gtjffwyaoa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pengpengdd.cyou/gtnxarmtkc.html

[D19] 按字段分组
来源：http://hz.zdqjudy.top/gtjjjqocqw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtgnekihze.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.birdmap.top/gtryfyupxc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yanxiufei.cn/gthtyaorko.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dianchejie.cn/gtiobfahqi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenlongwang.top/gtzwdswdrb.html

Go:   // 手写 map[string][]T
来源：http://hz.zycfv.cn/gttibagahf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hywenlv.cn/gtpbpjgcqo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jianghu66.top/gtuudyznwn.html

[D20] 统计每个元素出现次数
来源：http://hz.fzhhl.top/gtrbbotkxs.html

Py:   Counter(arr)
来源：http://hz.bjfxy.top/gtggykuegs.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtxdffmyre.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gthvfpzshn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtulvmjixc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sysykeji.top/gtyxtkjjgu.html

Go:   // 手写 map[T]int
来源：http://hz.yuanzhike.top/gtojwnekfo.html

Ruby: arr.tally
来源：http://hz.chenjidiqi.icu/gteboaijxz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yongpay.top/gttbfxtjuj.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtnobnwssq.html

Py:   x in arr
来源：http://hz.wangshuangyany.cn/gtxruhilwb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zdqjudy.top/gtesmxvqhz.html

JS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtozjdujot.html

TS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtaoktjfsd.html

Java: list.contains(x)
来源：http://hz.ywan-chungtsiang.top/gtdquruczr.html

Go:   slices.Contains(arr, x)
来源：http://hz.nwbrower.top/gthapkxpqj.html

Ruby: arr.include?(x)
来源：http://hz.wangdashe.top/gtearnwnld.html

C#:   list.Contains(x)
来源：http://hz.sysykeji.top/gtjfyzdivr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydjk.org.cn/gtehybmosp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtqzzyazok.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.52xcode.cn/gtfmlidyac.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxuanxn.top/gtexyotdvj.html

TS:   [...arr];
来源：http://hz.zhiwuduotai.top/gtvvoudqqp.html

Java: new ArrayList<>(list);
来源：http://hz.yuanzhike.top/gtasnavxfp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xinyue.icu/gtmqhmdxsz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangtech.top/gthpeasohj.html

C#:   new List<int>(list);
来源：http://hz.xinyue.icu/gtcehoefsx.html

[D23] reduce 累积计算
来源：http://hz.zhoulong.xyz/gtxepauoqy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhengqikj.top/gtzhxdwrhl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cucudq.cn/gtjukjtgex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtyndbzaka.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj202588.top/gtjgnvjioj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangkeji.top/gtfkmobnch.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtcawucdzg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenjidiqi.icu/gttjgbopja.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nanxinkj.top/gtpooxoolw.html

[D24] 字典 / Map 基本操作
来源：http://hz.hnxiangtu.top/gtpepeazzv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.wangdashe.top/gterpzjowh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guannengcc.top/gtjvnlddny.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.316326.xyz/gtfxngnqtg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.dianchejie.cn/gtjnbofedk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258.top/gtvjaerezh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuanzx.com/gtoyuaxkdb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtsuowytzb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gtppgyypsq.html

[D25] Set 集合去重与交并差
来源：http://hz.c1oappe.top/gtrjcliaqw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtamqjhvzc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangkeji.top/gtjweoqwxv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gttnyakzux.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ivvv.top/gtcdomjnxn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.0kj1m.cn/gtxqmanwjr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fengsongda.top/gtqnjzimjq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shangyingyoupin.top/gttlvjgpkf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ivvv.top/gthtgejulq.html

[D26] 数组转字符串
来源：http://hz.ywan-chungtsiang.top/gtimbeokxb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yvedp.cn/gtaxjrilor.html

PHP:  implode(", ", $arr);
来源：http://hz.nanxinkj.top/gtphtqqwgc.html

JS:   arr.join(", ")
来源：http://hz.yonumen.top/gtbxqmemji.html

TS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtivltsnaj.html

Java: String.join(", ", list)
来源：http://hz.ivvv.top/gtwintvkha.html

Go:   strings.Join(strs, ", ")
来源：http://hz.9152youxi.cn/gtikrtuwfe.html

Ruby: arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtnqfxxdlf.html

C#:   string.Join(", ", list)
来源：http://hz.shuidangran.top/gtotmbxyos.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtidaejevt.html

E. 字符串处理
来源：http://hz.jinyuanbaomall.cn/gtrebqefem.html

================================================================================
来源：http://hz.xuanzx.com/gtvpjievzq.html

[E01] 拼接字符串
来源：http://hz.316326.xyz/gtqxytquap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxuanxn.top/gthgkydfoe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangkeji.top/gthikuoacy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtlgyvpmqw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtnvnrdfam.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daxiang520.top/gtahjrgcoy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jianghu66.top/gtabshaopz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258888.top/gtkyhsciux.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gtdwmtoruj.html

[E02] 重复字符串
来源：http://hz.gotoacloud.top/gtxviacywe.html

Py:   "ab" * 3
来源：http://hz.aibaodan.cn/gtqdngopip.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zdqjudy.top/gtbpbmdczz.html

JS:   "ab".repeat(3)
来源：http://hz.zhixingplan.top/gthnwbgzgi.html

TS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gteumhdiqj.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gtnaypmdov.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ybcxt.top/gtqhmfxqfq.html

Ruby: "ab" * 3
来源：http://hz.andypj.xyz/gtbqepvijt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gotoacloud.top/gtfjzmuwwm.html

[E03] 截取子串
来源：http://hz.nanxinkj.top/gtwqwjyvhe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sufxvd.cn/gtkvtfutwc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhoulong.xyz/gticbhwphj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtabhtwpod.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gteldbcdpn.html

Java: s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtepacybpl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shanyushiyangtech.top/gtdszjsjsq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigfzy.top/gtjrohbpgy.html

C#:   s.Substring(1, 3)
来源：http://hz.jianghu66.top/gtwkatjjum.html

[E04] 查找子串位置
来源：http://hz.jlsjyb.cn/gtillepmhj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtufzvrgaa.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigfzy.top/gtzwialzlp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.feifeiyinyue.top/gtbutmpcrj.html

TS:   s.indexOf("x")
来源：http://hz.shzxlz.cn/gtjqjngwfn.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangtech.top/gtzictaoxu.html

Go:   strings.Index(s, "x")
来源：http://hz.ydzc1.top/gtpoaplawy.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtmekvyltm.html

C#:   s.IndexOf("x")
来源：http://hz.zhengqikj.top/gtzvucwntb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jyoumei.cn/gtswxoaftd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zycfv.cn/gtocajlesz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jqgfzy.top/gtmkucaaff.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtpqtzyvhg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xziqi.cn/gtpckdvwlg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtziitjecy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hongshengwenyu.top/gtxwdqtugc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtdozqssep.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.guannengcc.top/gtpynjllqw.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtgxnmphdq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtcmcfyfse.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.c1oappe.top/gtowllnofz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtzglinekg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtwcywrvwc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gturcgejqh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tian-w.cn/gtknsiwmtx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.mhx1999.top/gtiavlbmgv.html

C#:   s.Replace("a", "b")
来源：http://hz.gzhubu.top/gtndtuhhif.html

[E07] 按分隔符拆分
来源：http://hz.dashuyun.cn/gtahhxrqqq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dianchejie.cn/gtdroferyv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtiybxncbp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.smart0.xyz/gtemmijpnt.html

TS:   s.split(",")
来源：http://hz.ydjk.org.cn/gtwgflgaoa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guowangkeji.top/gtnxcyfvzp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shzxlz.cn/gtqaxpuzam.html

Ruby: s.split(",");  s.split
来源：http://hz.jiagoushi.top/gtoynxyfff.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtzqwjbeos.html

[E08] 数组按分隔符合并
来源：http://hz.hfpthk.cn/gtbursocfm.html

Py:   ",".join(items)
来源：http://hz.xingfuxueyuan.xyz/gthpotfkop.html

PHP:  implode(",", $items);
来源：http://hz.xuanzx.com/gtamzojjpb.html

JS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtoebbnjky.html

TS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtswgekhsi.html

Java: String.join(",", items)
来源：http://hz.jqgfzy.top/gtcdfunqgk.html

Go:   strings.Join(items, ",")
来源：http://hz.tianlin.xyz/gtfcwmamxz.html

Ruby: items.join(",")
来源：http://hz.zhiwuduotai.top/gtivkhopnb.html

C#:   string.Join(",", items)
来源：http://hz.ppjwa.cn/gtokaaksqn.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtcblzcxjg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hfpthk.cn/gtrzkfcyqy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhijiandao.cn/gtyudwpluk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtstvyhvlz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhoulong.xyz/gtvovsuhzq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hysaishi.cn/gteqniiysj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangshuangyany.cn/gtykvwdpss.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guowangkeji.top/gtzudfodzw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnqzz.top/gtiacfcfxl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ppjwa.cn/gtrnoksans.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gtvvcbptom.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xingfuxueyuan.xyz/gtukxgpeeh.html

JS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtbyntxjbh.html

TS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtuittctde.html

Java: String.format("%03d", 7)
来源：http://hz.zhixingplan.top/gtbskavpnu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aizwys.cn/gtsgsemmhk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtppaesdwi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yj20258.top/gtvbezbwlw.html

[E11] 反转字符串
来源：http://hz.yangfankeji.com/gtdxnislbk.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtdsmdjpcd.html

PHP:  strrev($s);
来源：http://hz.meibo888.top/gtysnvphmq.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtegaazpke.html

TS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtjdtxbony.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fzhhl.top/gtuzygyrtp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zycfv.cn/gtessmwkmz.html

Ruby: s.reverse
来源：http://hz.yuxming.cn/gtrznuwhna.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtwhoixtrm.html

[E12] 统计某字符出现次数
来源：http://hz.pengpengdd.cyou/gtqsiqxgod.html

Py:   s.count("a")
来源：http://hz.pengpengdd.cyou/gtzcxwfxwp.html

PHP:  substr_count($s, "a");
来源：http://hz.yanxiufei.cn/gtxndswnxi.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtixwyypnw.html

TS:   s.split("a").length - 1
来源：http://hz.dashuyun.cn/gtsrxqoyle.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gtnknadxvz.html

Go:   strings.Count(s, "a")
来源：http://hz.birdmap.top/gtctqzuwjf.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtvqteujqx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtoihueuiu.html

[E13] 逐字符遍历
来源：http://hz.guowangkeji.top/gtmcwmtaka.html

Py:   for ch in s: print(ch)
来源：http://hz.ydzc1.top/gtcujbipxu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jianghu66.top/gtbjsfinhy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtrbakzlhy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtabeqvozc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtbopjaqbi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigufen.top/gtylfvqoaj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhixingplan.top/gtkrkxeuou.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xylfe.cn/gtoxvozqay.html

[E14] URL 编码与 Base64
来源：http://hz.52xcode.cn/gtgefoexyj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenlongwang.top/gtebrxkwuf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sysykeji.top/gtdmflxqkt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigufen.top/gtpnjpqjow.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hammf.cn/gtqspmzkak.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.iojbl.cn/gtmxksqmfx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtzgphfcff.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yongpay.top/gtwbcjdyrc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtwyroscqk.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtsddfnlht.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinghuilouyu.cn/gtlowoplbj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cheryme.top/gtbmznhwbo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhiwuduotai.top/gtdsdgpcsc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gtotjkabfy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtjuqdpgbs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuanzhike.top/gtatxprtfo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cheryme.top/gtshoicjnm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cdnleiting.top/gtqwtnrbsy.html

[E16] 数字千分位
来源：http://hz.svipenyu.cn/gtatqxtzsg.html

Py:   f"{1234567:,}"
来源：http://hz.ivvv.top/gthobtgbmo.html

PHP:  number_format(1234567);
来源：http://hz.quarkkingdee.top/gtdfgmatxi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtqylqezrc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtgtpjiros.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.andypj.xyz/gtqnxnrhrj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenlongwang.top/gthnfmbtsz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtzemezfbi.html

C#:   1234567.ToString("N0")
来源：http://hz.hfpthk.cn/gtaefztiyt.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gtxtijhmos.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtwvydkbzg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.9152youxi.cn/gtnmjhfxml.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtmbxoxahq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtqfvoshxj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtihycytoc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gtfbedhbmb.html

Ruby: s.capitalize
来源：http://hz.shzxlz.cn/gtkdkdkcyw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dianchejie.cn/gtmxrjxvdy.html

[E18] 模板占位符替换
来源：http://hz.shanyushiyangtech.top/gtubhgnwms.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.redwolf501.top/gtyjfszvqg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinghuilouyu.cn/gtqidsgxrj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtxpztewjz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtvjvyhgxj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhengqikj.top/gtvtrqkbyg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtajiwhpzp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ivvv.top/gtorfzfhlq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cheryme.top/gtytyqkkot.html

[E19] 多行文本按行拆分
来源：http://hz.zdqjudy.top/gtneebswvd.html

Py:   s.splitlines()
来源：http://hz.jinqigufen.top/gtsvncpulo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtjfippcpi.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtavpjmtmt.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtvrxjthwr.html

Java: s.lines().toList()
来源：http://hz.hammf.cn/gtjlsnpzju.html

Go:   strings.Split(s, "\n")
来源：http://hz.yongpay.top/gtkliewkoa.html

Ruby: s.lines
来源：http://hz.0kj1m.cn/gtbfidivmt.html

C#:   s.Split('\n')
来源：http://hz.redwolf501.top/gtfjiagrrp.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gtupmhkmqf.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gtmoxliion.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenzaomai.com/gtzbtidytd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xingfuxueyuan.xyz/gtbktynfnu.html

TS:   if (s === "") {}
来源：http://hz.hysaishi.cn/gtcrhqxlvs.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtjfaraisa.html

Go:   if s == "" {}
来源：http://hz.dianchejie.cn/gtrxtkqugi.html

Ruby: if s.empty?
来源：http://hz.yanxiufei.cn/gtmlradcmt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yueranfly.top/gtqyldsbwz.html

[E21] 超长截断加省略号
来源：http://hz.xylfe.cn/gtnsatzvsv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhixingplan.top/gtlmuaqppg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtxwacctun.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtuieemkcg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtnsnenpfx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtdurqmtzz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtqaasqhqx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangdashe.top/gtrusyxyih.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtranohxre.html

[E22] 字节长度与字符长度
来源：http://hz.52xcode.cn/gtlquhhyhc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aibaodan.cn/gtilljpsie.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtmnaqrdmd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtfevkwkce.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtjsiyoeei.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.bjfxy.top/gtwpgfxron.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgfzy.top/gtkbyuykle.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenzaomai.com/gtzactxyru.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aibaodan.cn/gtmrrtkcqr.html

================================================================================
来源：http://hz.hywenlv.cn/gtobfjdllj.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtaeosmfxu.html

================================================================================
来源：http://hz.shuidangran.top/gtumjuywir.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtwyvogywy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tianlin.xyz/gtqnuwmwzf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gtruslbsif.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cashguo.top/gtpbvuqbnj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtrsaluyru.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtvzpctiid.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.52xcode.cn/gtkcptvbkr.html

Ruby: File.read("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtcdgrpjho.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hfpthk.cn/gtnclqdiwe.html

[F02] 逐行读取文件
来源：http://hz.nanxuanxn.top/gtjtivoixo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtqhgxprbz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtaeseodyy.html


<!-- 参考信息 -->