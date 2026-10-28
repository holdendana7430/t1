代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.dianchejie.cn/gtiqcfqezf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yangfankeji.com/gtmuyxwdwj.html

TS:   Math.max(...arr);
来源：http://hz.316326.xyz/gttbwpipeo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gtzuqkzkoi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtbhwppaer.html

Ruby: arr.max;  arr.min
来源：http://hz.sysykeji.top/gtkmbvallm.html

C#:   list.Max();  list.Min()
来源：http://hz.chenlongwang.top/gtrtxqiick.html

[D18] 扁平化嵌套数组
来源：http://hz.meibo888.top/gtjxtlvlfd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtvdoaymqj.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258.top/gtpbufhnbw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.daria6918.cn/gtxonpkhun.html

TS:   nested.flat();
来源：http://hz.hongshengwenyu.top/gtqmptmqtg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenjidiqi.icu/gturzkozde.html

Go:   // 手写双层循环
来源：http://hz.jinyuanbaomall.cn/gtxvygjubb.html

Ruby: nested.flatten
来源：http://hz.0kj1m.cn/gtbesyqnww.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinyuanbaomall.cn/gtdprgwtnu.html

[D19] 按字段分组
来源：http://hz.kuanghao11.cn/gtnqrbkhxh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aibaodan.cn/gtunvoiopj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhixingplan.top/gtpplsmktp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gtjkgfyiqy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtpstbczgu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gthpldbgqo.html

Go:   // 手写 map[string][]T
来源：http://hz.316326.xyz/gtqkkgpihn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.havefunace.top/gtjtnoujbd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtbsyyesgm.html

[D20] 统计每个元素出现次数
来源：http://hz.tian-w.cn/gtescstwgt.html

Py:   Counter(arr)
来源：http://hz.cqqwz.cn/gtlgwedipr.html

PHP:  array_count_values($arr);
来源：http://hz.feifeiyinyue.top/gtdyagndqj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtbcenvbxw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtgudejoxe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.0kj1m.cn/gtbfsrxmgl.html

Go:   // 手写 map[T]int
来源：http://hz.zhengqikj.top/gtmhftoubl.html

Ruby: arr.tally
来源：http://hz.jiagoushi.top/gttmfoycov.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtbebsmfdg.html

[D21] 判断是否包含某元素
来源：http://hz.gogol.net.cn/gtrqpyuxuj.html

Py:   x in arr
来源：http://hz.daria6918.cn/gtawllipnd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhixingplan.top/gtbywibkaq.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtseqxlrpq.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtwqnnmxej.html

Java: list.contains(x)
来源：http://hz.snrcjt.cn/gtqeckumuv.html

Go:   slices.Contains(arr, x)
来源：http://hz.shangyingyoupin.top/gtlzniefuj.html

Ruby: arr.include?(x)
来源：http://hz.yongpay.top/gtaafgtsdy.html

C#:   list.Contains(x)
来源：http://hz.daria6918.cn/gtyhdcxufo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenjidiqi.icu/gtbmshqnvj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtpbzmfytt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xylfe.cn/gtexqqoopr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtttkvemza.html

TS:   [...arr];
来源：http://hz.pengpengdd.cyou/gtmjfddxrq.html

Java: new ArrayList<>(list);
来源：http://hz.cucudq.cn/gtsivaywku.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.fzhhl.top/gtskuajvhw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xziqi.cn/gtgpbyylla.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangtech.top/gtwkdkulzp.html

[D23] reduce 累积计算
来源：http://hz.jianghu66.top/gtzmoqnfee.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aibaodan.cn/gtvdbkbecs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tianlin.xyz/gtfcmdfrrx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nwbrower.top/gtldymqepw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtvzzuvwbl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.316326.xyz/gtwuaslamj.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtzperwccv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhoulong.xyz/gtrjhibirk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhiwuduotai.top/gtaqwsgsvi.html

[D24] 字典 / Map 基本操作
来源：http://hz.yanxiufei.cn/gtnctlietc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zycfv.cn/gtfaguvqvf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.mhx1999.top/gtdtlbdqmy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhaomingkeji.xyz/gtpgcrfrgj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gzhubu.top/gttkqqefca.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenjidiqi.icu/gtgswgbffo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuxming.cn/gtaaluxdvb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jianghu66.top/gtkckhwxbm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hammf.cn/gtmhxihvup.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtgsnmlwfo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.9152youxi.cn/gtnowgicck.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gthygwznow.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gotoacloud.top/gtpaazjjyw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gthrbspczz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigfzy.top/gtrwfmjmot.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtiitxpuaf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yonumen.top/gtxhhsqbdq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cucudq.cn/gtcbsyxkyd.html

[D26] 数组转字符串
来源：http://hz.ydjk.org.cn/gtnqumfetv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gttqzjypbf.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtfudcltwi.html

JS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gthhmngtjv.html

TS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtlixokopf.html

Java: String.join(", ", list)
来源：http://hz.jlsjyb.cn/gtqagenopd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.316326.xyz/gtkziajisq.html

Ruby: arr.join(", ")
来源：http://hz.jqgufenzy.top/gtzmggfasr.html

C#:   string.Join(", ", list)
来源：http://hz.hammf.cn/gtizrosrgs.html

================================================================================
来源：http://hz.snrcjt.cn/gtcewkiepr.html

E. 字符串处理
来源：http://hz.fengsongda.top/gtjllpqwfg.html

================================================================================
来源：http://hz.yuxming.cn/gtfqjgltft.html

[E01] 拼接字符串
来源：http://hz.kuanghao11.cn/gtuusbirrx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cdnleiting.top/gtujflpkmm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.316326.xyz/gtfzorqrfc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtpasidnrv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zdqjudy.top/gtlpzgtqty.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hysaishi.cn/gtijlhvzik.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gzhubu.top/gtsptauazw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ybcxt.top/gtvfrvcbwp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.bjfxy.top/gtzlsxpslp.html

[E02] 重复字符串
来源：http://hz.shuidangran.top/gtiprtnyam.html

Py:   "ab" * 3
来源：http://hz.shuidangran.top/gtsebccnay.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jlsjyb.cn/gtdtjlwars.html

JS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtxprucacf.html

TS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtfpeqgosp.html

Java: "ab".repeat(3)
来源：http://hz.yj20258.top/gtieqfxvgp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gzhubu.top/gtrjtxhsqj.html

Ruby: "ab" * 3
来源：http://hz.gotoacloud.top/gtmnmdbrdy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yonumen.top/gthclnxjex.html

[E03] 截取子串
来源：http://hz.meibo888.top/gtneqsxddn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuetiantiany.cn/gtovjncljp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gaohongyu789.top/gtefljmddj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtuztwzqch.html

TS:   s.slice(1, 4)
来源：http://hz.quarkkingdee.top/gtnzjwjdui.html

Java: s.substring(1, 4)
来源：http://hz.daxiang520.top/gtvtavxshy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhiwuduotai.top/gtzddbrvde.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.dianchejie.cn/gttihjkixa.html

C#:   s.Substring(1, 3)
来源：http://hz.jiagoushi.top/gtmhegoszt.html

[E04] 查找子串位置
来源：http://hz.xingfuxueyuan.xyz/gtiwosodib.html

Py:   s.find("x");  s.index("x")
来源：http://hz.316326.xyz/gtnvytdqnq.html

PHP:  strpos($s, "x");
来源：http://hz.iojbl.cn/gtiocvgwen.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.svipenyu.cn/gtrshqqsht.html

TS:   s.indexOf("x")
来源：http://hz.quarkkingdee.top/gtpdfqmtgs.html

Java: s.indexOf("x")
来源：http://hz.ivvv.top/gtzghldpom.html

Go:   strings.Index(s, "x")
来源：http://hz.chenlongwang.top/gtregitivu.html

Ruby: s.index("x")
来源：http://hz.iojbl.cn/gtcpumpccc.html

C#:   s.IndexOf("x")
来源：http://hz.tian-w.cn/gtduejkniw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pengpengdd.cyou/gtutvbjygh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxinkj.top/gtxwprpkzx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hnqzz.top/gtrnvcyvfq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtvdyoxafr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gtaxkwfyzw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtgpdjbdpk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinghuilouyu.cn/gtgdcjnspq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.vqdsnc.cn/gtmmbkyijw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.redwolf501.top/gtukjmelof.html

[E06] 替换子串
来源：http://hz.kuanghao11.cn/gtenawsvhl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guannengcc.top/gtzewfiaij.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuanzhike.top/gtcosdxrgq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtikfmbnhu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtblvsixdo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtpuplkirf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nwbrower.top/gtgxrrxkoz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.havefunace.top/gtfemqznow.html

C#:   s.Replace("a", "b")
来源：http://hz.shzxlz.cn/gtpnvjddet.html

[E07] 按分隔符拆分
来源：http://hz.jyoumei.cn/gtxsscjjid.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.haohaochexian.top/gtewhpojti.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuanzx.com/gtjyrqactu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtxmewibta.html

TS:   s.split(",")
来源：http://hz.gaohongyu789.top/gtwdqljcph.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.feifeiyinyue.top/gtmwnnzaxo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.bjfxy.top/gtocayikux.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258888.top/gtmsogvfod.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.meibo888.top/gtrnopycbq.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258888.top/gttmnxkapb.html

Py:   ",".join(items)
来源：http://hz.pengpengdd.cyou/gtluctrdhu.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtnqcclbfq.html

JS:   items.join(",")
来源：http://hz.hammf.cn/gtdoymfula.html

TS:   items.join(",")
来源：http://hz.ehwqpu.com/gtjnybtpgj.html

Java: String.join(",", items)
来源：http://hz.yj20258888.top/gtdkzdpovt.html

Go:   strings.Join(items, ",")
来源：http://hz.guannengcc.top/gtgxtubsoy.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtgeemzery.html

C#:   string.Join(",", items)
来源：http://hz.zdqjudy.top/gtnazfcgos.html

[E09] 去除所有空白字符
来源：http://hz.jianghu66.top/gtqjjrpali.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tanke756.top/gtwjqhhaif.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhoulong.xyz/gtkqdhdbuu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sweek.top/gtunjvgpxl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtoiuixrjn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ehwqpu.com/gtsbzxwqkz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aibaodan.cn/gttbkfyfjt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxinkj.top/gthkhvlhef.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hongshengwenyu.top/gtazzrmhtq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhongyouzk.top/gtlxgcpjud.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtlmnmywyf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jiagoushi.top/gtqavfbgei.html

JS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtvuuaxffv.html

TS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtryqqhqvb.html

Java: String.format("%03d", 7)
来源：http://hz.zdqjudy.top/gtxvompcbw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shzxlz.cn/gtbwpivvkg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gthcamfzks.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dashuyun.cn/gtnsrqhazw.html

[E11] 反转字符串
来源：http://hz.shanyushiyangtech.top/gtrxspoakr.html

Py:   s[::-1]
来源：http://hz.zhijiandao.cn/gtadpwkhbd.html

PHP:  strrev($s);
来源：http://hz.hnxiangtu.top/gtgdktsjfh.html

JS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtexltyezo.html

TS:   [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtuhymxqxe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.bjfxy.top/gtffbzvhep.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pengpengdd.cyou/gtfsizyagt.html

Ruby: s.reverse
来源：http://hz.pycfn.com/gtmekdrtew.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtpiepgnxx.html

[E12] 统计某字符出现次数
来源：http://hz.jianghu66.top/gtfjlsfvaj.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gtuaftjopw.html

PHP:  substr_count($s, "a");
来源：http://hz.zhixingplan.top/gtpvldmtsd.html

JS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtebtzmwqr.html

TS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtpfjqtsxx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258.top/gtsrzynlro.html

Go:   strings.Count(s, "a")
来源：http://hz.bjfxy.top/gttllsndrm.html

Ruby: s.count("a")
来源：http://hz.sxryk.cn/gtkkojilpj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.snrcjt.cn/gtdrfxmrec.html

[E13] 逐字符遍历
来源：http://hz.xingfuxueyuan.xyz/gtydrubirk.html

Py:   for ch in s: print(ch)
来源：http://hz.jlsjyb.cn/gtydlsofdc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.bjfxy.top/gtcarlfchc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtyfizuvsx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtpenvuvmy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cashguo.top/gtqenbcand.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj20258.top/gtkcfwwvhr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhixingplan.top/gtolldfkum.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtvcdlgrok.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtkleocaej.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dashuyun.cn/gtwgcrmmmt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xziqi.cn/gtaldrktow.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangshuangyany.cn/gtntygakgh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gthijipxuv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.feifeiyinyue.top/gtifoclios.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ehwqpu.com/gtamxktqmt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hongshengwenyu.top/gtgkwdqphj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhijiandao.cn/gtyzjhhnni.html

[E15] HTML 转义 / 反转义
来源：http://hz.jqgfzy.top/gticmbpavc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aibaodan.cn/gtuikgqvxn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jiagoushi.top/gtenpbukkp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hywenlv.cn/gtjxkfjtte.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dianchejie.cn/gtxleekncd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtxdzracrd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigfzy.top/gtpwikkygt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gogol.net.cn/gtgnawivau.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xziqi.cn/gtevldkmym.html

[E16] 数字千分位
来源：http://hz.xylfe.cn/gtyiozwitr.html

Py:   f"{1234567:,}"
来源：http://hz.zhijiandao.cn/gtojfhwwnf.html

PHP:  number_format(1234567);
来源：http://hz.zhoulong.xyz/gtcsqbpmou.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtmrjatple.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.316326.xyz/gtfghjcaka.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guowangkeji.top/gtmzzfflzn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtpobrqtkh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinqigufen.top/gtfubhirvb.html

C#:   1234567.ToString("N0")
来源：http://hz.gzhubu.top/gtiehabilq.html

[E17] 首字母大写
来源：http://hz.gotoacloud.top/gtbitzmtco.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cashguo.top/gtbzfmewpo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cashguo.top/gtjlwqnwsl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtejakffvo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtoeoegvxi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhengqikj.top/gtbgemihek.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gtounnpviq.html

Ruby: s.capitalize
来源：http://hz.kuanghao11.cn/gtjahddtiu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gtfvdcncon.html

[E18] 模板占位符替换
来源：http://hz.dianchejie.cn/gtfhoqgoac.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.smart0.xyz/gtewuzjtly.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zdqjudy.top/gtaugyjlqb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtsjqywuee.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gtyzohawbo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.snrcjt.cn/gtumdwxdal.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hammf.cn/gtfnlykgqh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jyoumei.cn/gtldncdcsy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aibaodan.cn/gtxgocitpn.html

[E19] 多行文本按行拆分
来源：http://hz.yangfankeji.com/gtrcknlzhg.html

Py:   s.splitlines()
来源：http://hz.ivvv.top/gtyhhfnsgb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtvktvhkgt.html

JS:   s.split(/\r?\n/)
来源：http://hz.sufxvd.cn/gthcwrwkwj.html

TS:   s.split(/\r?\n/)
来源：http://hz.sxryk.cn/gtoeovhmfe.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gteyfmlmnl.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnqzz.top/gtqdakevvk.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtgfchjqts.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtrgosfwol.html

[E20] 判断字符串是否为空
来源：http://hz.yongpay.top/gtdtppniqr.html

Py:   if not s:
来源：http://hz.shanyushiyangkeji.top/gtsmwdnbzh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yueranfly.top/gtpjafirjo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guannengcc.top/gtptfiwoau.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gthehttoqu.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangdashe.top/gtjubcesdn.html

Go:   if s == "" {}
来源：http://hz.chenlongwang.top/gtksuzxzwk.html

Ruby: if s.empty?
来源：http://hz.chenzaomai.com/gtmozjdgkj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangkeji.top/gtbdqmwcaa.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtllpjdhoa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhixingplan.top/gtndydfwtp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnxiangtu.top/gtdxctouao.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtbbrijzkv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtuxvcoalq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtpnzkuhjg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtvnevygsb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hysaishi.cn/gtelijsgqr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dashuyun.cn/gtuzxfxpdy.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtjdnqcaqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinghuilouyu.cn/gturixspzn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gtydrgvnxw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtonvxdljf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtzngeerrr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgufenzy.top/gtsoqgeizb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtautuqfgj.html

Ruby: s.bytesize;  s.length
来源：http://hz.yangfankeji.com/gtlhnzzlzl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.haohaochexian.top/gtsnmauqcz.html

================================================================================
来源：http://hz.zhixingplan.top/gtyqdngwmk.html

F. 文件与目录
来源：http://hz.nanxinkj.top/gtpqdykhtv.html

================================================================================
来源：http://hz.zhijiandao.cn/gtojdmzozz.html

[F01] 读取整个文件
来源：http://hz.fengsongda.top/gtocmzaonm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258888.top/gtdvltpick.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtvxujjmzz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.daria6918.cn/gtliiuxgbz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtsjztyhhm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtthbpijmy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hammf.cn/gtqwtlfbea.html

Ruby: File.read("a.txt")
来源：http://hz.hnxiangtu.top/gtzuqfkjqo.html


<!-- 参考信息 -->