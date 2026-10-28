代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.wangshuangyany.cn/gtevwtvevo.html

[D16] 求和与平均值
来源：http://hz.yanxiufei.cn/gtbqjblaoe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hongshengwenyu.top/gtfjmnobul.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.feifeiyinyue.top/gtlgrkoyqg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtadmeyywb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhongyouzk.top/gtxllxueog.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jyoumei.cn/gtoqjcvhdb.html

Go:   // 手写循环累加
来源：http://hz.yangfankeji.com/gtykpzsknb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhijiandao.cn/gtmwsnsiec.html

C#:   list.Sum();  list.Average()
来源：http://hz.sufxvd.cn/gtgowihfkj.html

[D17] 最大值与最小值
来源：http://hz.yj20258.top/gtnfywfzlj.html

Py:   max(arr);  min(arr)
来源：http://hz.zhengqikj.top/gtmbdrhryz.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gtuvifbypm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhengqikj.top/gtcaublsqv.html

TS:   Math.max(...arr);
来源：http://hz.jinghuilouyu.cn/gtzbyimkwk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.316326.xyz/gtuqgsunqe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.quarkkingdee.top/gtsfegnuzv.html

Ruby: arr.max;  arr.min
来源：http://hz.haohaochexian.top/gtfulhwfwd.html

C#:   list.Max();  list.Min()
来源：http://hz.daria6918.cn/gteiioffft.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gtyehekgxt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.9152youxi.cn/gtmginwswk.html

PHP:  array_merge(...$nested);
来源：http://hz.iojbl.cn/gtlevxjsja.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xziqi.cn/gtodiatmue.html

TS:   nested.flat();
来源：http://hz.hywenlv.cn/gtsifzdvea.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhixingplan.top/gthsrhlise.html

Go:   // 手写双层循环
来源：http://hz.wangshuangyany.cn/gtdnaytcvd.html

Ruby: nested.flatten
来源：http://hz.ybcxt.top/gtsbvnbfju.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtfxzgsuoj.html

[D19] 按字段分组
来源：http://hz.xuetiantiany.cn/gtwqkldczm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtnrozkgjl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sweek.top/gtrxvbgnan.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.316326.xyz/gtnetmoryg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gtbsbhwvny.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangdashe.top/gtudwnumop.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigufen.top/gtchltgpol.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.smart0.xyz/gtcxhbsion.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuetiantiany.cn/gtxtxndtlg.html

[D20] 统计每个元素出现次数
来源：http://hz.gotoacloud.top/gthtdkkooe.html

Py:   Counter(arr)
来源：http://hz.wangshuangyany.cn/gttaucfeuz.html

PHP:  array_count_values($arr);
来源：http://hz.nanxinkj.top/gtyqcjrjuf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtkwtbtefq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtovcpujen.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hnxiangtu.top/gtzablyqbv.html

Go:   // 手写 map[T]int
来源：http://hz.jiagoushi.top/gtpsfnyont.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtodkzquqz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258888.top/gtycqdgrcw.html

[D21] 判断是否包含某元素
来源：http://hz.gogol.net.cn/gtuccibnac.html

Py:   x in arr
来源：http://hz.gogol.net.cn/gtjyzipfyh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gaohongyu789.top/gtaumtztha.html

JS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtmxugsqnc.html

TS:   arr.includes(x)
来源：http://hz.sxryk.cn/gttwothxwi.html

Java: list.contains(x)
来源：http://hz.jqgufenzy.top/gtypzvchpj.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gtyvteiuhq.html

Ruby: arr.include?(x)
来源：http://hz.aizwys.cn/gtkwijywax.html

C#:   list.Contains(x)
来源：http://hz.yonumen.top/gtrgwuxref.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tanke756.top/gturkleoeo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xinyue.icu/gtdgeatgby.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sysykeji.top/gtyzpfaddf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinyuanbaomall.cn/gtzczvtndg.html

TS:   [...arr];
来源：http://hz.zhoulong.xyz/gtsrpjcsqc.html

Java: new ArrayList<>(list);
来源：http://hz.xinyue.icu/gtmvstrtnm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ivvv.top/gtbdkuefza.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ydjk.org.cn/gtokuzzktk.html

C#:   new List<int>(list);
来源：http://hz.tian-w.cn/gtuicpbaml.html

[D23] reduce 累积计算
来源：http://hz.gotoacloud.top/gthvfyptns.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ybcxt.top/gtxdqirbgi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ivvv.top/gtzjfdekiq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtrvusqlfj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gttefopvef.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hywenlv.cn/gtdybmjtqy.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gtmmxzedsm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yvedp.cn/gtyellgqie.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtsnaupaoh.html

[D24] 字典 / Map 基本操作
来源：http://hz.dashuyun.cn/gtnusnfqxv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258.top/gtalxqxwdh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxinkj.top/gtqrfjuptc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenjidiqi.icu/gtbaremibx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zdqjudy.top/gtspxnzdya.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shzxlz.cn/gtkebzeubj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtlnnqbogz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gtrlybahxs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinghuilouyu.cn/gtxnascdtq.html

[D25] Set 集合去重与交并差
来源：http://hz.zhoulong.xyz/gtfeaprriv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtlfpaarpo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.svipenyu.cn/gtgiabvdkr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangkeji.top/gtladobnee.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gttciderki.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dashuyun.cn/gtwxnwdiel.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhiwuduotai.top/gtngtrchew.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj202588.top/gtjuzusues.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sxryk.cn/gtelbqkqsr.html

[D26] 数组转字符串
来源：http://hz.iojbl.cn/gtqsnazgox.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gogol.net.cn/gtkcqexxqw.html

PHP:  implode(", ", $arr);
来源：http://hz.guowangkeji.top/gtunmmcwov.html

JS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtfjuoopbj.html

TS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtxitshbek.html

Java: String.join(", ", list)
来源：http://hz.zdqjudy.top/gtnzbwgdvu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtcsjfnktk.html

Ruby: arr.join(", ")
来源：http://hz.aizwys.cn/gtymgovtuc.html

C#:   string.Join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtbymaxwwn.html

================================================================================
来源：http://hz.gotoacloud.top/gteuzxdqqf.html

E. 字符串处理
来源：http://hz.yvedp.cn/gtzrhmcmxu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtrzfbtpxf.html

[E01] 拼接字符串
来源：http://hz.sufxvd.cn/gtcguwyisw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.andypj.xyz/gtkctgckfj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cucudq.cn/gtfyuqfbhp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtzauejanr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtdqigjvsf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.meibo888.top/gtszejqfgt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinghuilouyu.cn/gtacbzuehs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxuanxn.top/gthxyuiqaw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gtapwnfawh.html

[E02] 重复字符串
来源：http://hz.ppjwa.cn/gtdomcjaun.html

Py:   "ab" * 3
来源：http://hz.fzhhl.top/gtwkouyjpb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hfpthk.cn/gtzphotqzv.html

JS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtciihhhsl.html

TS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtaklhhnoq.html

Java: "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtjmslgvem.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ppjwa.cn/gtqgoigrzn.html

Ruby: "ab" * 3
来源：http://hz.cqqwz.cn/gtrbuutnff.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnqzz.top/gtlgbndbvb.html

[E03] 截取子串
来源：http://hz.hysaishi.cn/gtoylgeeby.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xingfuxueyuan.xyz/gttxrnbgjy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fzhhl.top/gtqphkpwvu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yueranfly.top/gtpjmclmof.html

TS:   s.slice(1, 4)
来源：http://hz.gotoacloud.top/gtfolgajqy.html

Java: s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtljfvwkxm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jqgfzy.top/gtpilmiwzf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yueranfly.top/gtpegcrcoc.html

C#:   s.Substring(1, 3)
来源：http://hz.havefunace.top/gtyvdmdxbe.html

[E04] 查找子串位置
来源：http://hz.andypj.xyz/gtutvyrudr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fengsongda.top/gtseptsbbv.html

PHP:  strpos($s, "x");
来源：http://hz.fengsongda.top/gteehfaqvs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gaohongyu789.top/gtehwrioeu.html

TS:   s.indexOf("x")
来源：http://hz.sxryk.cn/gtwqgzajhb.html

Java: s.indexOf("x")
来源：http://hz.birdmap.top/gtxefnrpaz.html

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gtqfzkjtmi.html

Ruby: s.index("x")
来源：http://hz.zdqjudy.top/gtnclnydye.html

C#:   s.IndexOf("x")
来源：http://hz.zycfv.cn/gtrnpzyziq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guowangkeji.top/gtejszvmbd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuetiantiany.cn/gtawlvmwjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhengqikj.top/gtumiosmhv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydzc1.top/gtleccvrqd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinqigufen.top/gthmabwnly.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtxdesccyy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.0kj1m.cn/gtgsyrqpoh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangdashe.top/gtbvxjxzvy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnqzz.top/gthorloglj.html

[E06] 替换子串
来源：http://hz.cucudq.cn/gtrljqqawe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.iojbl.cn/gtpftmkrab.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.daria6918.cn/gtraxlejzl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtgqofeprl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtyxgypoak.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtsafylhlq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgufenzy.top/gtjhlvkond.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jiagoushi.top/gtqetrlsbd.html

C#:   s.Replace("a", "b")
来源：http://hz.yonumen.top/gtkmdazrgg.html

[E07] 按分隔符拆分
来源：http://hz.0kj1m.cn/gtnbsilnar.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nanxuanxn.top/gtqgzwpjum.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtnyreewod.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cheryme.top/gtrckwsneg.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtishshcfd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gtcwahcjkn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.feifeiyinyue.top/gtxukfhlgx.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtjnpewkkd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gaohongyu789.top/gtylnsgbbs.html

[E08] 数组按分隔符合并
来源：http://hz.yangfankeji.com/gtxevcmvul.html

Py:   ",".join(items)
来源：http://hz.shzxlz.cn/gtuwetftlj.html

PHP:  implode(",", $items);
来源：http://hz.mhx1999.top/gtcanbndeg.html

JS:   items.join(",")
来源：http://hz.zhixingplan.top/gtcibxeewl.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtlumotwxo.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gtlqouigxa.html

Go:   strings.Join(items, ",")
来源：http://hz.cucudq.cn/gtavepdldo.html

Ruby: items.join(",")
来源：http://hz.wangdashe.top/gtglwsomjk.html

C#:   string.Join(",", items)
来源：http://hz.jianghu66.top/gtdibiurgc.html

[E09] 去除所有空白字符
来源：http://hz.cucudq.cn/gtmikfzopa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nanxinkj.top/gtgffuaets.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnxiangtu.top/gtsopupfuf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtghghcumw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtudcnazme.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hongshengwenyu.top/gtqwrxndvb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hongshengwenyu.top/gtpespjltt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guannengcc.top/gtzpyvtozf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nwbrower.top/gtfeugfeyp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hnxiangtu.top/gtxbrkghop.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ehwqpu.com/gtmvdefisn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gotoacloud.top/gtakxmilws.html

JS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtarxxhzla.html

TS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtzrehotke.html

Java: String.format("%03d", 7)
来源：http://hz.dashuyun.cn/gtbzinghqx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fzhhl.top/gtmjipgzqi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hammf.cn/gtovxacesg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.havefunace.top/gtyyjkqwsb.html

[E11] 反转字符串
来源：http://hz.guowangkeji.top/gtvqeotgup.html

Py:   s[::-1]
来源：http://hz.yonumen.top/gttpfovgcr.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtiwximyix.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtsftgqitl.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtnfkbxgjd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.havefunace.top/gtbvwqeiuq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yvedp.cn/gtnfwcvzgc.html

Ruby: s.reverse
来源：http://hz.yuxming.cn/gtppgbvrft.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtjagbketl.html

[E12] 统计某字符出现次数
来源：http://hz.feifeiyinyue.top/gtlmusuepx.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtjvdwisev.html

PHP:  substr_count($s, "a");
来源：http://hz.iojbl.cn/gthjbsndub.html

JS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtfnyjugfm.html

TS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtbflxpoqg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ivvv.top/gtwwoeinlv.html

Go:   strings.Count(s, "a")
来源：http://hz.zhongyouzk.top/gtuscqpubc.html

Ruby: s.count("a")
来源：http://hz.smart0.xyz/gtrlzhkbpb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dashuyun.cn/gtgpdkeogq.html

[E13] 逐字符遍历
来源：http://hz.chenjidiqi.icu/gtrrrhgdzs.html

Py:   for ch in s: print(ch)
来源：http://hz.hongshengwenyu.top/gtmbusfnqy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gtsqjwfcds.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtbpjsmcsc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtjckwkldp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hammf.cn/gtpcleykec.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ppjwa.cn/gtcesycacd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cqqwz.cn/gtgasgzrrw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.havefunace.top/gtzjaflysi.html

[E14] URL 编码与 Base64
来源：http://hz.wangshuangyany.cn/gtnzstbgnc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtuievolbj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xinyue.icu/gtvdvuawjy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pycfn.com/gtxdthngap.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxinkj.top/gtfovvogfe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.9152youxi.cn/gtmysxdfau.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gtlmvvhmil.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.smart0.xyz/gttiwiosdi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jyoumei.cn/gtvsvwjgqv.html

[E15] HTML 转义 / 反转义
来源：http://hz.0kj1m.cn/gtrqlmkizi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hammf.cn/gteondiaay.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydzc1.top/gtsxtshnjs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sweek.top/gtvcprzhji.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.birdmap.top/gtzdvygcsm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gttfodhztu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.aizwys.cn/gtfnmkzwfh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gtdegicfqe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yuxming.cn/gttkmaasix.html

[E16] 数字千分位
来源：http://hz.cheryme.top/gtdnwkvzho.html

Py:   f"{1234567:,}"
来源：http://hz.ppjwa.cn/gtqsjblbwt.html

PHP:  number_format(1234567);
来源：http://hz.haohaochexian.top/gtzxdmkcgl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtjauzeuzn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.316326.xyz/gtpsygxxgr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtbfwcgvdl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cdnleiting.top/gtbsnhpwyy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tanke756.top/gtywokjogy.html

C#:   1234567.ToString("N0")
来源：http://hz.52xcode.cn/gtpabnwzew.html

[E17] 首字母大写
来源：http://hz.daxiang520.top/gtclxbpswl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgufenzy.top/gtvlzslibh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtvmnpdvju.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pengpengdd.cyou/gtdsqiuiai.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtqzrbwywn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.52xcode.cn/gtjvruyddh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.svipenyu.cn/gtdbvuvcsk.html

Ruby: s.capitalize
来源：http://hz.sufxvd.cn/gtmflldkab.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxinkj.top/gtlemwjixo.html

[E18] 模板占位符替换
来源：http://hz.dashuyun.cn/gtemewksnr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtmitfnetz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhongyouzk.top/gtmtgqlbdh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xinyue.icu/gtpyupgknn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtvwhnhwzp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.iojbl.cn/gtyahcwjqq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.meibo888.top/gtydzuoxqt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhixingplan.top/gtbcuvuenk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tian-w.cn/gtvnzybbcs.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gttfzkkyqr.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtxolqtwzx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.mhx1999.top/gtchmzlzei.html

JS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtasayikyp.html

TS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtzcvipfjv.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtrqzzzbmq.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gtuplmdujc.html

Ruby: s.lines
来源：http://hz.cdnleiting.top/gtbcmdkxee.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtlosusscj.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtsqlnvgcw.html

Py:   if not s:
来源：http://hz.cashguo.top/gtrjhvouga.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jlsjyb.cn/gtnhkouidy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yanxiufei.cn/gtivnzcnzf.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gtezmugvwg.html

Java: if (s.isEmpty()) {}
来源：http://hz.fzhhl.top/gtirosvvat.html

Go:   if s == "" {}
来源：http://hz.shuidangran.top/gtiqougtub.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gteyvprwqb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtjvsshyen.html

[E21] 超长截断加省略号
来源：http://hz.yvedp.cn/gttnmigzwc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtvihatppj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxinkj.top/gtpwdeateo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtqpegiguz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtukacdfuy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtailmxkpo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xingfuxueyuan.xyz/gtlqrexlqo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gtinftdpsh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.c1oappe.top/gtigvvzkkd.html

[E22] 字节长度与字符长度
来源：http://hz.xuanzx.com/gtsysdglvn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zdqjudy.top/gtptcuqpqs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gthqdysxcs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtpwgkgicc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gtvfgglvbs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yonumen.top/gthhcftvuj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.redwolf501.top/gtvduopdsc.html

Ruby: s.bytesize;  s.length
来源：http://hz.ybcxt.top/gtizubsmad.html


<!-- 参考信息 -->