代发 wailian999

Ruby: arr.index(x)
来源：http://hz.jyoumei.cn/gtjjyeodjn.html

C#:   list.IndexOf(x);
来源：http://hz.hammf.cn/gtrqxqrpns.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gaohongyu789.top/gtqdswznvq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sysykeji.top/gtzzfojrbs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hywenlv.cn/gthqojaoyj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtitnianqk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtatecywac.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yuanzhike.top/gtnzpnjxjx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hysaishi.cn/gtcesfljha.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ybcxt.top/gtyhvqmyyd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xziqi.cn/gtukoxpgie.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gtttiwgdyo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yangfankeji.com/gtxkxrghvd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ppjwa.cn/gtibywmjft.html

JS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gthixruofs.html

TS:   arr.map(x => x * 2)
来源：http://hz.svipenyu.cn/gtgaytpdmo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zdqjudy.top/gtjepuvycs.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gtyduzizoq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.daria6918.cn/gtmmqnhare.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.bjfxy.top/gtranqfhdr.html

[D15] 去重
来源：http://hz.cheryme.top/gtmipwcjvu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtmgsjugkl.html

PHP:  array_unique($arr);
来源：http://hz.ppjwa.cn/gtclawdyfc.html

JS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtmbdwnyps.html

TS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtuusbrslr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtncydhpnq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jlsjyb.cn/gtxfgurkwz.html

Ruby: arr.uniq
来源：http://hz.hammf.cn/gtbbyfghyh.html

C#:   list.Distinct().ToList()
来源：http://hz.pycfn.com/gtpptaxejb.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtdrbuwxyy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.quarkkingdee.top/gtjralfpjq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shangyingyoupin.top/gtmbbwqnfm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtxarlihds.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtnhcrujaj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenlongwang.top/gtzbmvhode.html

Go:   // 手写循环累加
来源：http://hz.xuanzx.com/gtmnpqzvbk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yonumen.top/gtaemzhlol.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangdashe.top/gtdrpqnoyi.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtcaztilzz.html

Py:   max(arr);  min(arr)
来源：http://hz.smart0.xyz/gtgdgsyots.html

PHP:  max($arr);  min($arr);
来源：http://hz.haohaochexian.top/gtdtqaycgn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.svipenyu.cn/gtsebanjpw.html

TS:   Math.max(...arr);
来源：http://hz.jinyuanbaomall.cn/gtzizhfjmf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sufxvd.cn/gtsrqrsybx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ppjwa.cn/gtnpfgdurd.html

Ruby: arr.max;  arr.min
来源：http://hz.mhx1999.top/gtueqxcmil.html

C#:   list.Max();  list.Min()
来源：http://hz.birdmap.top/gtkpbybgad.html

[D18] 扁平化嵌套数组
来源：http://hz.hfpthk.cn/gtlssckwto.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yvedp.cn/gtvwpyansu.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtejvhgwad.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gtvmyviqje.html

TS:   nested.flat();
来源：http://hz.ppjwa.cn/gtdswidigl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtzsyhwuzt.html

Go:   // 手写双层循环
来源：http://hz.chenlongwang.top/gttsguhpri.html

Ruby: nested.flatten
来源：http://hz.jinyuanbaomall.cn/gtcqwebipk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.vqdsnc.cn/gtraroitmi.html

[D19] 按字段分组
来源：http://hz.zhiwuduotai.top/gtkynabpch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigufen.top/gtvmeabizo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zdqjudy.top/gtmqmwwmgr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xinyue.icu/gtcfypueyk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenlongwang.top/gtibwviefa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtidzdjtct.html

Go:   // 手写 map[string][]T
来源：http://hz.pycfn.com/gtjlwnhimg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sxryk.cn/gtfhzeegoo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhoulong.xyz/gtucgfpkes.html

[D20] 统计每个元素出现次数
来源：http://hz.shanyushiyangkeji.top/gtudgmsyvn.html

Py:   Counter(arr)
来源：http://hz.vqdsnc.cn/gtqtagzmst.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258888.top/gtsweizwoo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtwdtdmgym.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtoxmmkrvy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtvlygxtrw.html

Go:   // 手写 map[T]int
来源：http://hz.yueranfly.top/gtchjvlgst.html

Ruby: arr.tally
来源：http://hz.hnqzz.top/gtzhqowhzf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxuanxn.top/gtmnjrdabw.html

[D21] 判断是否包含某元素
来源：http://hz.cashguo.top/gtiqlnfacq.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtltcrpozy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gtwzwrwxrs.html

JS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtapnrisbn.html

TS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtasavhcdy.html

Java: list.contains(x)
来源：http://hz.shuidangran.top/gtigcggskg.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxuanxn.top/gtmipqmyms.html

Ruby: arr.include?(x)
来源：http://hz.tian-w.cn/gtjvwwlfgb.html

C#:   list.Contains(x)
来源：http://hz.yj20258888.top/gtalocinhd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ppjwa.cn/gtqolwasiz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhixingplan.top/gtkojtglha.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.guannengcc.top/gtkiaezhus.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tian-w.cn/gtmtmhzxhp.html

TS:   [...arr];
来源：http://hz.hysaishi.cn/gthopcrzuq.html

Java: new ArrayList<>(list);
来源：http://hz.316326.xyz/gtcanggcdi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhijiandao.cn/gtkomaqhcf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dianchejie.cn/gtjbgfbzya.html

C#:   new List<int>(list);
来源：http://hz.yj20258.top/gtoljbdixt.html

[D23] reduce 累积计算
来源：http://hz.jinghuilouyu.cn/gtaavlrmct.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtyiifoxhj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fzhhl.top/gtppuypjcb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtxulgsgvh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gthvbnguev.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sysykeji.top/gtyrwoynhx.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtupofvzye.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.vqdsnc.cn/gtfqhfsaad.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fzhhl.top/gtgdalgogt.html

[D24] 字典 / Map 基本操作
来源：http://hz.hnxiangtu.top/gtxpwdczqs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.c1oappe.top/gtrxuplhhy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gzhubu.top/gtsgqkxnzj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gtbzrmwixr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shzxlz.cn/gtrjamkaur.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenjidiqi.icu/gtfxavtpgj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydzc1.top/gtvjzaqbtm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydzc1.top/gtvvumesyu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dashuyun.cn/gtjttmfnqa.html

[D25] Set 集合去重与交并差
来源：http://hz.jianghu66.top/gtvnrgmiej.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guowangkeji.top/gteacegnef.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fzhhl.top/gtukisgtza.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.iojbl.cn/gtsqblodqp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtuoamdhkb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.0kj1m.cn/gtlyfxxjzk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtwdxnhtwq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zdqjudy.top/gtwwtcfitk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhiwuduotai.top/gtmdbuehef.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtglsymsiz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xylfe.cn/gtzroxscxk.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258888.top/gtnqesmakk.html

JS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtewqmpkih.html

TS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtrxmvzylu.html

Java: String.join(", ", list)
来源：http://hz.jianghu66.top/gtvsbuinoj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinyuanbaomall.cn/gtadluhgxg.html

Ruby: arr.join(", ")
来源：http://hz.sysykeji.top/gtokxbkwli.html

C#:   string.Join(", ", list)
来源：http://hz.dianchejie.cn/gttxbihvdf.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnjlggzpr.html

E. 字符串处理
来源：http://hz.dashuyun.cn/gtxumdekpj.html

================================================================================
来源：http://hz.316326.xyz/gtisgpxdhw.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtjuufamci.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.c1oappe.top/gtombwgyga.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.guowangkeji.top/gtbeiophrr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtornmasyx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtsttcgwra.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xinyue.icu/gtwdyppyxt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sysykeji.top/gthkbshppv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gaohongyu789.top/gtmpqdjzjg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gthqkoxvyh.html

[E02] 重复字符串
来源：http://hz.dianchejie.cn/gtnufelzbn.html

Py:   "ab" * 3
来源：http://hz.guowangkeji.top/gtysewsfta.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydjk.org.cn/gtxabxgtlv.html

JS:   "ab".repeat(3)
来源：http://hz.tanke756.top/gtzflymdrf.html

TS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtmetsitdv.html

Java: "ab".repeat(3)
来源：http://hz.xinyue.icu/gtvzzqmxss.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yangfankeji.com/gtfjcqxqab.html

Ruby: "ab" * 3
来源：http://hz.feifeiyinyue.top/gtahwetvec.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.daxiang520.top/gtkqidmlau.html

[E03] 截取子串
来源：http://hz.wangshuangyany.cn/gtxveuwgpj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtouzsavhd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtnatyfpqp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gzhubu.top/gtjlshrsvn.html

TS:   s.slice(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtzjhpovuc.html

Java: s.substring(1, 4)
来源：http://hz.guannengcc.top/gttmnpvmdp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenlongwang.top/gtmblqozpj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xingfuxueyuan.xyz/gtberxxtcx.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangkeji.top/gturdptxcb.html

[E04] 查找子串位置
来源：http://hz.ywan-chungtsiang.top/gtjeufinpp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tianlin.xyz/gtyqttlzhg.html

PHP:  strpos($s, "x");
来源：http://hz.xziqi.cn/gtyscvkvwr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xylfe.cn/gtfrgpshcq.html

TS:   s.indexOf("x")
来源：http://hz.yuxming.cn/gtazpukido.html

Java: s.indexOf("x")
来源：http://hz.iojbl.cn/gtgvwufqsx.html

Go:   strings.Index(s, "x")
来源：http://hz.c1oappe.top/gtmrlvmlzw.html

Ruby: s.index("x")
来源：http://hz.52xcode.cn/gtcssdlchz.html

C#:   s.IndexOf("x")
来源：http://hz.aizwys.cn/gtojqgbysi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hfpthk.cn/gtrkzicfvg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ppjwa.cn/gtilvxkytq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenjidiqi.icu/gtjsoabwyf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtczbohmoa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydzc1.top/gtyfieqlda.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtyxzhxbrq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yongpay.top/gtvpspjtcg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sufxvd.cn/gtomguakhj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ivvv.top/gtmnzmqdld.html

[E06] 替换子串
来源：http://hz.kuanghao11.cn/gtbejrqsgf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.iojbl.cn/gtreenvftl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xylfe.cn/gtzqhentqn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtaurawpxx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtlihazmcd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtiovysaow.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hywenlv.cn/gtjtahaaxo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shangyingyoupin.top/gtdoafpjsb.html

C#:   s.Replace("a", "b")
来源：http://hz.xuanzx.com/gtssmuxjxb.html

[E07] 按分隔符拆分
来源：http://hz.xziqi.cn/gtsavrimwh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydzc1.top/gtoxfmrkac.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yanxiufei.cn/gtscktqfvw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hysaishi.cn/gtlvvirzlv.html

TS:   s.split(",")
来源：http://hz.kuanghao11.cn/gtqphcrfvb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.0kj1m.cn/gtiwzxsgox.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtgvkqucbm.html

Ruby: s.split(",");  s.split
来源：http://hz.c1oappe.top/gtvorvqubt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jyoumei.cn/gtihgqpkzx.html

[E08] 数组按分隔符合并
来源：http://hz.nwbrower.top/gtawmlafqd.html

Py:   ",".join(items)
来源：http://hz.sysykeji.top/gteosipalo.html

PHP:  implode(",", $items);
来源：http://hz.hfpthk.cn/gtwnsbqbki.html

JS:   items.join(",")
来源：http://hz.guowangkeji.top/gtlwgnxksx.html

TS:   items.join(",")
来源：http://hz.yj202588.top/gtpcgtxugf.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gtjktznjjh.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gtbdydkaei.html

Ruby: items.join(",")
来源：http://hz.daria6918.cn/gtdjuulohs.html

C#:   string.Join(",", items)
来源：http://hz.yongpay.top/gtnyaormie.html

[E09] 去除所有空白字符
来源：http://hz.nanxinkj.top/gtfprruhuu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sufxvd.cn/gtltuguwac.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yvedp.cn/gtbdldjxgq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtrcdryshw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtxguqnkxh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jianghu66.top/gtzpitcbgj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtizsjhmzh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gttuvarflr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinyuanbaomall.cn/gtyqkkgtfl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cqqwz.cn/gtsbaqbdjy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sufxvd.cn/gtooohvkvk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gttinfmhkb.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtlyiuctep.html

TS:   "7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtvtvietsa.html

Java: String.format("%03d", 7)
来源：http://hz.yueranfly.top/gtxtimxsyw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sweek.top/gtwzhmkecr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gtabbkgekq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yj20258.top/gtutgjbfty.html

[E11] 反转字符串
来源：http://hz.sufxvd.cn/gtvjwiytjx.html

Py:   s[::-1]
来源：http://hz.yuanzhike.top/gtreiieevm.html

PHP:  strrev($s);
来源：http://hz.jyoumei.cn/gtpaxgtetf.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtvempdiuh.html

TS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gttvecuhig.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yvedp.cn/gtebxjxuxx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.daxiang520.top/gtuuanoxeb.html

Ruby: s.reverse
来源：http://hz.316326.xyz/gtdfxeonio.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtylqfatgs.html

[E12] 统计某字符出现次数
来源：http://hz.shzxlz.cn/gthkljuptx.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gtvzmvudru.html

PHP:  substr_count($s, "a");
来源：http://hz.yj20258.top/gttpmiyiix.html

JS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtoztrjdrd.html

TS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtntubhjxg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sweek.top/gtdtkrnyat.html

Go:   strings.Count(s, "a")
来源：http://hz.bjfxy.top/gtelcxoefh.html

Ruby: s.count("a")
来源：http://hz.ehwqpu.com/gtqcogrtku.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cdnleiting.top/gtdhichnfk.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtifxhoacw.html

Py:   for ch in s: print(ch)
来源：http://hz.ybcxt.top/gtzitjfafu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xinyue.icu/gtlhcprftp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtlufwjhoz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtxkloafyv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.dashuyun.cn/gtsfrxzazn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gaohongyu789.top/gtgulqjwxx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.316326.xyz/gtlhlvqydj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtsshyjkmv.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtlhshhbbb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj202588.top/gtnzxwbtlf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shzxlz.cn/gtufhivzdh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hysaishi.cn/gttexezwgs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xinyue.icu/gtushmloma.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dianchejie.cn/gtkdjrwlwy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigufen.top/gteyzxxxxo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtqezziixy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fzhhl.top/gtbzlmeycr.html

[E15] HTML 转义 / 反转义
来源：http://hz.haohaochexian.top/gtocelsgoh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgufenzy.top/gttsqmxeyp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxuanxn.top/gtvnqmqeee.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aibaodan.cn/gtizyjwiwc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gzhubu.top/gtypevkkaf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xingfuxueyuan.xyz/gtnxmmxwym.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yanxiufei.cn/gtyfqwubgx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtkgxpyrnv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xylfe.cn/gtszyianyh.html

[E16] 数字千分位
来源：http://hz.zhaomingkeji.xyz/gtfacurlbz.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gtezlvryix.html

PHP:  number_format(1234567);
来源：http://hz.hnqzz.top/gtuflbgejx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtdumvbsoi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtsnqcqgcu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gteyteggqs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yongpay.top/gtjjbrapml.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtwmefhcok.html

C#:   1234567.ToString("N0")
来源：http://hz.fengsongda.top/gtqrbcvmst.html

[E17] 首字母大写
来源：http://hz.c1oappe.top/gtsvbikuxb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hysaishi.cn/gttfoxgvaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtwrouyfho.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtpdffehkc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtxwnfxarn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhixingplan.top/gtjmddofin.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aizwys.cn/gtvepqwouw.html

Ruby: s.capitalize
来源：http://hz.chenlongwang.top/gthziljdxt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zdqjudy.top/gtttwfdvjr.html

[E18] 模板占位符替换
来源：http://hz.zhijiandao.cn/gtakzziqfg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yueranfly.top/gtsfoebmic.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.redwolf501.top/gtlnadbkhv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtjhlxrnqf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtpuvmswvj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtijgbrmjh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jiagoushi.top/gtxbtdaaaz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yongpay.top/gtmfznzdkk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yongpay.top/gtcxlfmxbs.html

[E19] 多行文本按行拆分
来源：http://hz.svipenyu.cn/gtzpjcysil.html

Py:   s.splitlines()
来源：http://hz.guannengcc.top/gtuycmjkye.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guannengcc.top/gtwpgbxbsu.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gttvlazxhy.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtqgszuash.html

Java: s.lines().toList()
来源：http://hz.bjfxy.top/gtcvhvkusw.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangshuangyany.cn/gthtwrtogb.html


<!-- 参考信息 -->