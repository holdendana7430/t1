代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.gzhubu.top/gtahiupyfa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.c1oappe.top/gtmcosaxbx.html

TS:   Math.max(...arr);
来源：http://hz.haohaochexian.top/gtlmvuxtwa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daxiang520.top/gtfvllfxeh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shzxlz.cn/gtftfshtzm.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gtwhaoypuv.html

C#:   list.Max();  list.Min()
来源：http://hz.guowangkeji.top/gtbmobdspx.html

[D18] 扁平化嵌套数组
来源：http://hz.fzhhl.top/gtldlminiw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydzc1.top/gtatjwhttc.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtbnznvdzk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jiagoushi.top/gtouiydqlx.html

TS:   nested.flat();
来源：http://hz.yongpay.top/gtiyarnqax.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aizwys.cn/gtyrlbejoz.html

Go:   // 手写双层循环
来源：http://hz.jinqigufen.top/gtfjkvjnkj.html

Ruby: nested.flatten
来源：http://hz.yanxiufei.cn/gtvqcslqak.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gtlucrkunc.html

[D19] 按字段分组
来源：http://hz.ehwqpu.com/gtfjytimim.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gtswbjgudi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xingfuxueyuan.xyz/gtdvwjoeca.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtwvzcoyyt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pengpengdd.cyou/gtsnbzfheg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jiagoushi.top/gtbqficsxo.html

Go:   // 手写 map[string][]T
来源：http://hz.sweek.top/gtohoduoob.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtjtnzvrkk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xingfuxueyuan.xyz/gtenlcxixr.html

[D20] 统计每个元素出现次数
来源：http://hz.gogol.net.cn/gtievjpizt.html

Py:   Counter(arr)
来源：http://hz.xylfe.cn/gtnoyaidxt.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtkohhtmek.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtypveljld.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtdfhedeug.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cdnleiting.top/gtpzumcnfn.html

Go:   // 手写 map[T]int
来源：http://hz.dianchejie.cn/gttlydezat.html

Ruby: arr.tally
来源：http://hz.jyoumei.cn/gtsnxofuny.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ppjwa.cn/gtxgyfebrr.html

[D21] 判断是否包含某元素
来源：http://hz.sysykeji.top/gtqmppfycg.html

Py:   x in arr
来源：http://hz.tian-w.cn/gtjgbiecpd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zycfv.cn/gtygjzlcjn.html

JS:   arr.includes(x)
来源：http://hz.hammf.cn/gtwjdapdfn.html

TS:   arr.includes(x)
来源：http://hz.sweek.top/gtloxlijbk.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gtawtsapag.html

Go:   slices.Contains(arr, x)
来源：http://hz.xylfe.cn/gtkitcchhc.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gtuyjomlxe.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtaevcmrhh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gzhubu.top/gtodeoampu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtiuaivpbw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.meibo888.top/gtnipmsnlh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yueranfly.top/gtehuwtxds.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtsbtyszfi.html

Java: new ArrayList<>(list);
来源：http://hz.jyoumei.cn/gtcbxiotjg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydzc1.top/gtkgmcqszy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cucudq.cn/gtgwuugiww.html

C#:   new List<int>(list);
来源：http://hz.ivvv.top/gtpsmahpzu.html

[D23] reduce 累积计算
来源：http://hz.jinqigufen.top/gtvoinfumr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.vqdsnc.cn/gtwzgrqayw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xingfuxueyuan.xyz/gtklwqucfx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtzvibgcqm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtestjgjpj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydzc1.top/gtwczwyjbe.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtgxbcmxgv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ywan-chungtsiang.top/gtwmyfbyjc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuanzx.com/gtmecsupzv.html

[D24] 字典 / Map 基本操作
来源：http://hz.cheryme.top/gtycembsnk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gtdwwgwuvk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxuanxn.top/gtvejhnmwu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fengsongda.top/gtyivuoqez.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuanzhike.top/gtjsjmgizb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jqgfzy.top/gtaasbnqni.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.smart0.xyz/gtcrysloja.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gogol.net.cn/gtyhxsehha.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gtbahdfvzp.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxuanxn.top/gtauoekxdc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.snrcjt.cn/gtqxtvoary.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jlsjyb.cn/gtsicpnium.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xingfuxueyuan.xyz/gtbnwtkgts.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigfzy.top/gtyfolkgaq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gtczrvkwcn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenlongwang.top/gtmtyvryzh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sufxvd.cn/gtqkrxlacg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnxiangtu.top/gtemtljoiq.html

[D26] 数组转字符串
来源：http://hz.cheryme.top/gtmmddedcx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj202588.top/gthzuakdky.html

PHP:  implode(", ", $arr);
来源：http://hz.guowangkeji.top/gtjrzliepa.html

JS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtrkezgoyh.html

TS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtwtwnkvrj.html

Java: String.join(", ", list)
来源：http://hz.gzhubu.top/gttqatuhrr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuanzx.com/gtcohzczzb.html

Ruby: arr.join(", ")
来源：http://hz.jqgfzy.top/gtfwmixytm.html

C#:   string.Join(", ", list)
来源：http://hz.tian-w.cn/gtkqnginmv.html

================================================================================
来源：http://hz.meibo888.top/gtsxifoyoi.html

E. 字符串处理
来源：http://hz.feifeiyinyue.top/gtmfbednby.html

================================================================================
来源：http://hz.tanke756.top/gtiepwayog.html

[E01] 拼接字符串
来源：http://hz.wangshuangyany.cn/gtenvhonqf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.wangdashe.top/gtwfselhss.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jianghu66.top/gtvbhiyucy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtqurxcxim.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtlzsdnwpu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jyoumei.cn/gtfdrvggcb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinyuanbaomall.cn/gtrmttizme.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtwwixbmou.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenjidiqi.icu/gtxoltdlhv.html

[E02] 重复字符串
来源：http://hz.zhaomingkeji.xyz/gtqwzwcrfk.html

Py:   "ab" * 3
来源：http://hz.nanxuanxn.top/gtlnpstnuz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.redwolf501.top/gtqgtagdlr.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtlzsmpdwz.html

TS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtskwznxop.html

Java: "ab".repeat(3)
来源：http://hz.guannengcc.top/gtvuyaziwk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yangfankeji.com/gtdarnadqe.html

Ruby: "ab" * 3
来源：http://hz.zhixingplan.top/gtgzhovfvq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.vqdsnc.cn/gtcwekrczq.html

[E03] 截取子串
来源：http://hz.yuxming.cn/gtnbmrkehl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gaohongyu789.top/gtfmpesumo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zycfv.cn/gtdylucodu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sweek.top/gtusvalecs.html

TS:   s.slice(1, 4)
来源：http://hz.zdqjudy.top/gtfwxzklhu.html

Java: s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtdgjxojva.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinqigfzy.top/gtlbwkfowx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.quarkkingdee.top/gtxssrqmhr.html

C#:   s.Substring(1, 3)
来源：http://hz.daxiang520.top/gthbeqxjnr.html

[E04] 查找子串位置
来源：http://hz.yanxiufei.cn/gtlagrfwxb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hnxiangtu.top/gtxjazmorf.html

PHP:  strpos($s, "x");
来源：http://hz.zhoulong.xyz/gtatxmxbza.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtdzmsnqhc.html

TS:   s.indexOf("x")
来源：http://hz.snrcjt.cn/gtfwxlxnzb.html

Java: s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtifjxgfxz.html

Go:   strings.Index(s, "x")
来源：http://hz.meibo888.top/gtyurjtnfo.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtqqxwispu.html

C#:   s.IndexOf("x")
来源：http://hz.aizwys.cn/gtgmtoxrtt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhixingplan.top/gtrjaprdxc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258.top/gtqcxohsiq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ppjwa.cn/gthwdgvvwm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtfjespjqm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.vqdsnc.cn/gtpvacnzat.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtqmswmbjl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtqnnezdls.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.52xcode.cn/gtloqslwso.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangshuangyany.cn/gtehrilalh.html

[E06] 替换子串
来源：http://hz.gogol.net.cn/gtabkfdqhd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.snrcjt.cn/gttfzydpvf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yvedp.cn/gtfqqvpond.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtbymlqqvm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtfqmqtihe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtkpxiensu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fzhhl.top/gtumseqplm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtaotpkpoh.html

C#:   s.Replace("a", "b")
来源：http://hz.zhengqikj.top/gtvseptpwv.html

[E07] 按分隔符拆分
来源：http://hz.hammf.cn/gtuggmllsr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuetiantiany.cn/gtduimifgi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yongpay.top/gtlxwimeep.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cqqwz.cn/gtquofkfpo.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtmdmnxtbh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shuidangran.top/gttgsdjcwn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.9152youxi.cn/gtcfdxhnst.html

Ruby: s.split(",");  s.split
来源：http://hz.birdmap.top/gtlftbxyyh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daxiang520.top/gtordyajen.html

[E08] 数组按分隔符合并
来源：http://hz.c1oappe.top/gtnzjezinu.html

Py:   ",".join(items)
来源：http://hz.zycfv.cn/gtzdvgdtkw.html

PHP:  implode(",", $items);
来源：http://hz.zdqjudy.top/gtnkxqkygd.html

JS:   items.join(",")
来源：http://hz.aibaodan.cn/gtuhrggrnv.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtxjvgrcyy.html

Java: String.join(",", items)
来源：http://hz.aizwys.cn/gtmwagoyal.html

Go:   strings.Join(items, ",")
来源：http://hz.cqqwz.cn/gtxsvwknej.html

Ruby: items.join(",")
来源：http://hz.zdqjudy.top/gtpdzvyypf.html

C#:   string.Join(",", items)
来源：http://hz.jiagoushi.top/gtzfrkhnll.html

[E09] 去除所有空白字符
来源：http://hz.aibaodan.cn/gttmfdfymb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jlsjyb.cn/gtdazebcpv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtkwgxjygq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtdsmjxbkw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtreyxmkos.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.snrcjt.cn/gtuowzouua.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cheryme.top/gtkviispux.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtrxydvtka.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gaohongyu789.top/gtjestvhlv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nanxuanxn.top/gtsxeuwnnn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cdnleiting.top/gtmqectmrp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhiwuduotai.top/gtgfjotlmv.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtjamgupkd.html

TS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtffnjusxb.html

Java: String.format("%03d", 7)
来源：http://hz.aizwys.cn/gtnvtxgcxa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhijiandao.cn/gtqsdbrwjn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gtqeldpcdv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zdqjudy.top/gtueykxodo.html

[E11] 反转字符串
来源：http://hz.jinqigfzy.top/gtoglhidcj.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gtbpelubsa.html

PHP:  strrev($s);
来源：http://hz.wangdashe.top/gtuukmdxvd.html

JS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtjmrdeopr.html

TS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtffllhamz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hysaishi.cn/gtmrjqcptf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhengqikj.top/gtpysmxyub.html

Ruby: s.reverse
来源：http://hz.tian-w.cn/gtgjdeqmvk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtqeoiyuws.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtfhqkyyvl.html

Py:   s.count("a")
来源：http://hz.gzhubu.top/gttcrtqnvh.html

PHP:  substr_count($s, "a");
来源：http://hz.guowangkeji.top/gtxiekgnxp.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtdoujcqsl.html

TS:   s.split("a").length - 1
来源：http://hz.zhixingplan.top/gtgpjaebkf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sxryk.cn/gtsxbtlkik.html

Go:   strings.Count(s, "a")
来源：http://hz.jlsjyb.cn/gtgalubgkx.html

Ruby: s.count("a")
来源：http://hz.tanke756.top/gtkdeudcfk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj202588.top/gtsixomgac.html

[E13] 逐字符遍历
来源：http://hz.tianlin.xyz/gtwxgkthsq.html

Py:   for ch in s: print(ch)
来源：http://hz.chenlongwang.top/gtiirrqjza.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dashuyun.cn/gtbbljmmey.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtoabjnhos.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtvyefkpii.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cucudq.cn/gtdprthbbo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yongpay.top/gtsxpibmqv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuanzhike.top/gtaxmkzivi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuanzx.com/gttyatlvqr.html

[E14] URL 编码与 Base64
来源：http://hz.zhijiandao.cn/gtvlvuilqw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhijiandao.cn/gtwwpchgan.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhiwuduotai.top/gtprtafcgz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aibaodan.cn/gthdgjvvoh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gtaicfzppj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgufenzy.top/gtcpouhrmf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aibaodan.cn/gtejwjmpoj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtcyelkvft.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinqigfzy.top/gtvyqmpeog.html

[E15] HTML 转义 / 反转义
来源：http://hz.bjfxy.top/gtmktuzhpi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtfstjsutn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tianlin.xyz/gtzjiilhsx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.redwolf501.top/gtltawqygd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtzuclplbx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydjk.org.cn/gtunltxrpq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuxming.cn/gtytyxbwmy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shuidangran.top/gtxaijbbkf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dianchejie.cn/gtwyqkormn.html

[E16] 数字千分位
来源：http://hz.snrcjt.cn/gtwaerjmer.html

Py:   f"{1234567:,}"
来源：http://hz.yonumen.top/gtpyqbrcxd.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtnqseyzmn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gtjrzfbvrs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtzmlqvmyy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yanxiufei.cn/gtojnaavfy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ybcxt.top/gtubzrjsms.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenjidiqi.icu/gtdcvjubhm.html

C#:   1234567.ToString("N0")
来源：http://hz.hnxiangtu.top/gtczfocldk.html

[E17] 首字母大写
来源：http://hz.chenlongwang.top/gtvoufvfmq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgfzy.top/gtgrfjuiik.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yonumen.top/gtjotinzyv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtbvlonnri.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtcowwchyq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jianghu66.top/gtlbsysbsq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenzaomai.com/gthlyhbfmi.html

Ruby: s.capitalize
来源：http://hz.zycfv.cn/gtatyotslc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xingfuxueyuan.xyz/gthxrnrufj.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gtymqfahgb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.feifeiyinyue.top/gtmdwxqflm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.andypj.xyz/gtahhvazwn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtzorhmvaw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gtjiivirid.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tianlin.xyz/gtttuxpkwd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtfezwyrsa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sysykeji.top/gtnveforwb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.redwolf501.top/gthtkxfair.html

[E19] 多行文本按行拆分
来源：http://hz.ppjwa.cn/gtnduhhwic.html

Py:   s.splitlines()
来源：http://hz.havefunace.top/gtxvoslief.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shzxlz.cn/gtqjkidnpf.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtjwnbtynl.html

TS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtnhakkfux.html

Java: s.lines().toList()
来源：http://hz.wangdashe.top/gtldlvjppi.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gtznrbrxoz.html

Ruby: s.lines
来源：http://hz.aizwys.cn/gtsiwrwkmh.html

C#:   s.Split('\n')
来源：http://hz.hywenlv.cn/gtktpawvhq.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtdxyagdoq.html

Py:   if not s:
来源：http://hz.cucudq.cn/gtgcjtlcck.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.mhx1999.top/gtnqwlgqer.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.iojbl.cn/gtdbdijipr.html

TS:   if (s === "") {}
来源：http://hz.jinyuanbaomall.cn/gtgosfdewt.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtgltrjefl.html

Go:   if s == "" {}
来源：http://hz.shangyingyoupin.top/gtmxhqlhzx.html

Ruby: if s.empty?
来源：http://hz.wangshuangyany.cn/gtwyotccnq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ybcxt.top/gtmwebdwea.html

[E21] 超长截断加省略号
来源：http://hz.cqqwz.cn/gtqfevwlqi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtaosttwyr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtxkkelahj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtfcdqcgfc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtnbqcicpb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtmkprntha.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gtbeltihox.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.havefunace.top/gtcvwpblsf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhijiandao.cn/gtovsggvxb.html

[E22] 字节长度与字符长度
来源：http://hz.svipenyu.cn/gtcexbzipc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtcjciqhlz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtydyjklda.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gteaogwslo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtkfceqlxb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtnhdopisa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ydzc1.top/gtuzajdvma.html

Ruby: s.bytesize;  s.length
来源：http://hz.bjfxy.top/gtsamxyhan.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtumxizyqh.html

================================================================================
来源：http://hz.yj20258888.top/gtnzategvx.html

F. 文件与目录
来源：http://hz.shangyingyoupin.top/gtccjrzvml.html

================================================================================
来源：http://hz.cdnleiting.top/gtzcfojyyi.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtdljscjon.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtcmdhhwha.html

PHP:  file_get_contents("a.txt");
来源：http://hz.snrcjt.cn/gtfwqbvjku.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yongpay.top/gtxoxkumvx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.iojbl.cn/gttapjakwn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtuxoxvqle.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gaohongyu789.top/gtkbzcvpdu.html

Ruby: File.read("a.txt")
来源：http://hz.yvedp.cn/gtsezcmklk.html


<!-- 参考信息 -->