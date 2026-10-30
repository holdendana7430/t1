代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/ggkfttswc.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gzknixdsk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gbvvepsfl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gnzmkmfqm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gmgbpknbg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gawbrusxo.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gamfshfss.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/ggffkhfqg.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/guhpkelyy.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gemenzxrs.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gkmyqqeyx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gjvxvnxoy.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/glcofsnse.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gitcibwjk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gkxppttpo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gviwmuxpq.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gwqrgupui.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gqrbhllqc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gmiikienk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gejnneqvk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/ggjioyedn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnsrjyvuj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gbmszpmyi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gtxxorhne.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gunsjhgbh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gmdzqznhr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/ggxkqweuf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/goglhdpds.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gjxzanhqw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gduuxqkei.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/giblfevqu.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gtrxodvud.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/geelsihct.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gozdzjgim.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gkaywnrut.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gwsgeekyz.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghjliiicc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gkefacxdi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gsyxmnzdd.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gobnxudgj.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gmyhwugxg.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gkzbxaztv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gmtjmvglo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gllybtlqn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdzguylnh.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gvzfzktki.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gwgzixtiq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gbbzlecvf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggkougrve.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gwwldiejg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gbgwptmyb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gksqexdro.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gcmfnkuqp.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gaijlozhd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfiliycnj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/geyumxugu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwbywzong.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gltutfihu.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gmefexoid.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gvhwyebab.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gbjteehle.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gobzpmdce.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gcggwbxyd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gtnjglkyx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gyuobhdtj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gxhrryngw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gcgpijbml.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gsvlfmrdi.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grzqvpnel.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gqizrzkwt.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/ghmxawyhy.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gbiswvxrd.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gwgbqqbmg.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gzzrtbtyy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gsppmjkgl.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/ghtwzylpr.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gczhelktz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gggsbwejk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gbwyqwtnh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gsykkhwah.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdnszxzyu.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/glqscpxqp.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gnhbrehyx.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gblgtgshi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqtwzmec.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gaqhwtzmd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gxshrhpyb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gtoeyynpd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gpaplxxti.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gfqjpunsy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gfubuapck.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/glvykoafe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gfxojddcd.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gdigxeaeb.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gsjpmjxql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gdlxzdell.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/govdeunfr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gmeatrgbi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gxtinbvki.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwbojmxh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ghlanfwbx.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gjyqhhhrg.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gqndlsrwa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gtklpqzxy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gvapkrpso.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxpdutjkb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gytxobgqq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gptdepnvy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gfybvouwu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gxylzaerj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gmnpooilg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gtkgvmekt.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gebbqzbwz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/geknfyejj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvbhguoas.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gvtvrolgm.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gubeimlvy.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gmghweckd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gwyoaylmo.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gyopjjspi.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/ghgaorqkv.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/ggjpsigjo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gxkqxhcfo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gixslryby.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gtejvjdzk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gdjpntzpt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/grmcwdqwb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkltnqeyn.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/grgvzhrha.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gvhknfqvu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gfwhkxugk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/ghwlaptmd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gkkwfzyxt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gpihhryin.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxdcyodmg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gkvqqbuov.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gandhazod.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gqssppisu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gkyfbzwse.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gvmdqavzz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gegjjyngz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gbwgudgol.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gjqvglsjf.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gxeueisju.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gjftylwat.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gzfansiuv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gostksqdv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gexpoivph.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gweenuhof.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gtljlzqsm.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggasbxhgt.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gckyxeypb.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gzufligbq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gwpqxvvag.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gmpjajzcb.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gnimtjaqo.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwkpitpoz.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gkhgvkhwg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnhgclzk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gkcwiamqf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/golwgcren.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gsvhqwhcc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/ggfovnvbu.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gdmomwboa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gtgdrsnjr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/glaycwmee.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gnrdhfqwn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gmkrghrts.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtvxlkotn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gjirupfis.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gfwscrbch.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gcnjxkwlb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gdeyqdpaf.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gzcejxmat.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gvhrkqyaa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/grexgjhlf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gjysigknx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gbankdfcb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gbekgzufd.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gwzsxiaxl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gfdxerkfj.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gdbmskdtr.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/giklxasxx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gcdlglzpu.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gcfxayxxo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gdpefdult.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gghwogwvf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gfxyvwutg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/glpjiyvuk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gchhgvzsr.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gcfhjmmdt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gtwdqwrxn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/grbgeiutu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gopajdghf.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gdtqxjaxj.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gedsojvoy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gkmxyhxuv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gjjogyhlw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gwlpytrng.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gjiuexylx.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gzvtiivdw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gokdcvitw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gqpvlevps.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gmmzmxcuc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gpzbpihii.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwpjlvnbg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/glwlnkwjg.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gqjqdgpfs.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/ggmiahsui.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gvtgbfxia.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/glxtyfshm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/ghvyxjegn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/givfonypa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gwsjywgwq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gkxaavnxl.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gonvfzdoa.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gqjszioqq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gvoashrzh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gcopctbhb.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gehstkjeq.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gapxxdxvj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjxlfpqbp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/ghawrxrwa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gkljeeaaz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtbqbtllb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gfdtulonm.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gcpwxtaoo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gbjgdimue.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/giskxysiz.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gxikkolnx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gzjtadrcj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/guwotxbrp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gchcyadeg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/glhwmwpyw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gwqeugjra.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gipeqcqdh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gweksmlvb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gnhotwhhw.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gcpgesahk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gevessvix.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gvhlshsny.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gtiukwtwj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gcbvqanmv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gitkramzq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/ggljqhksw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gakunhqyy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqmnrjuxx.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gstokzfja.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gelogdtmf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grqjubtuy.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gkfarpbwv.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gyruladjw.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ggtbaufom.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gnkwlegcx.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/goegjhkpv.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gqancasbj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbmfegwit.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gnfqktohp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glwfukefk.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gojejlzku.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gfbdgexxd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gpfxftnzy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gabnyibck.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gixviehsc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gvphvdhzd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gxlmiqcpe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gnwnxmass.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdjzgisfc.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gxlmpjzou.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/giscvndls.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gejmjzctv.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gcvziodoa.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gcrrhritb.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfrzimnkz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gcifzammx.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gxgfyzeqw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gomwgtvxf.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gzhxefkbl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gpoyltanm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gtlsazwbl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gpdaloaha.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtqygxjuv.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gaeavrusr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gjnyuvjaf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gehzcwgod.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzgxcsbqh.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gwvixumfk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gzghxgaad.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gdykexzip.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gkcgjxqoo.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gqfoymojn.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/grgucpjkr.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gktimdkqz.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gnrbkuwyp.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gpbqbvfdb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gfsilitrm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gugvbtszs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gsqaafqzr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxtlzoatv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/grvhnjxmq.sHtML


<!-- 参考信息 -->