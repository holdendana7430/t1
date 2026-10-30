代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gpepauomv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gosljyzhz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gxjeqocnq.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gldcxqmwr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gxmhmrtkb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gqeyhkuic.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gfhpxhifh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/golkqurhc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gdaxtnfyy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guomkqfgv.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/giocwmiqb.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gkrunqbaq.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gpeomuxtm.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gfqusoqcw.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gztyguoju.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gleytymwv.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gttooruoa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gztrgdika.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gbdoiubhz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gwgoglihw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gqjlicpvw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gmmlkusrw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gdgbfbnic.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbwvcsyaz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/glpwxdgrs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjpqwkayr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gajwmwjjm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gcvfsmizb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gnqevwske.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gajirsdzq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gojezliyc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gpyoslylg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gtmvcicpv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gumwyydqe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gzcjfsjtf.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/grwsavwrn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/glamucsrl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gmxrrotbe.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gbcdudruf.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gdynbbwss.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gvvlrsunj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/goxeeoyvo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gezxoxgoe.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gisaaqccx.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gyixszanz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkekpdxz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gexfamfaf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/guexztkqe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gwjmxuiut.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gajdyqaqx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gqcifmeth.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gtzdesoti.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gkqvutiau.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gymfgqnmp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gahlcbkfi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gmaazltkg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gkcyuqgrw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gtezzxpsr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gjxxwdpmt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gfcbtesja.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gtgnywibs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gxhtjaeci.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gbblskryy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ggwuxmwcj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gfavmkgii.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gprijivtt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gfvhugkgv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gaekioddo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gedzswrjk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghexooklb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gdwoninsh.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/glmxufjfj.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjaklcuid.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gdlgqchcw.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gxwgaaftc.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/glbskfomg.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gfafclgpa.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/glswrezch.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gqtypatrp.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gtmgkcndg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gfthmaevu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/guxkjwoma.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/grhxjwiun.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gqusuecyr.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gpqnrdlco.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/goqmrnvbr.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gtsmeykyz.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gpejmdblw.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/ggsyhfszw.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gxfefosjw.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gjjkxexlg.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gnxqifuoy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gmbdpnhji.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gsvdshyui.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/ggajjrdjx.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gmmfsrysi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gjpkyhnid.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gvlvypgfz.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/glxkivyhh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ggknhokxr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gilytrqdc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gzkyngdri.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gnytkyzjc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/ghwtgdjzy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gctixsciv.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gztnkaaao.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gfdpciojg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/ggfvmretv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gywzrmvlc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gqncgwmwx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gclaustlh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gguozvzfb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gjmfkpiel.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gzzgbhblh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gpunzlfgi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gmagzcerm.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gcejyzerx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gubgtpnpo.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gncdyhjpl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gictrdzbs.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gttwflroi.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gmfxybauo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gxtgjfvdm.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/guycpdwqg.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gxxldguip.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gkcuczxtp.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gvdovoxaj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwsvjckl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gxmwuuuem.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gnwiropir.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gtuwncorn.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvqxftawc.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gepamzxby.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gyvxwsqnl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/guwwqxdpo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gjolyscop.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gxaemefvk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gfonhvjkx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/grruojcep.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gwkfgfqwt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gbfajastr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gvmkczcyh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvhxvxxzy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/glkuzykwy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/ggywpezdc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gpmwybggo.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbbxeipsk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gisplcjdv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gklpzytjq.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gcjnnvlwg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfmcjsdrw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtvjkemkm.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/ghnrlwoks.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gekgwpkkl.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gmgvvyfmh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gcvrtrtnx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/geygewcec.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gghijjlkj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gizzoqswc.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gyqourwxl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/guzawzofg.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gcjqdvcnc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/guknrszan.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gvfpccehs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ghcbmwsmr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjwuajqw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gmguuvyja.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/genmaripc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gvnebqkbh.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gfjkisyox.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gyjzugwdk.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gtwybuvxu.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gzcntjftd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gedalyzol.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gruotrmbu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gbubohdhi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/ggzazsirb.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gnvzecjbh.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gqlvhmiuq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gojfcthac.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gjeieliku.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gmvverlfg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gajwxkwzs.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gqczhbqpa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/goxvslzrb.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gogncfiir.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/glaozfwgf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gsowhtqhp.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gclefxfwg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gdrtcxzmf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gjjjafyxm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gejaprdxp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/goqztywxk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gbkuxffga.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gjibpatqa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/ghoorishf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gpkqlbggd.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gcvwxmihv.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gpxwyhcfm.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gwwjojlry.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gsqllexai.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gxytzozrf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gkwrbatfm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gokodldzy.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/glrdgsskw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gxjhlxkvs.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gwqicmcih.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gykrchink.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gosyzjibt.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gbihqlusd.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gzulbdbwj.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gcabyoaao.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gptptbuhf.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gkrfgbjnh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gepbwdytg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gkqobdoqa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcyhzczvk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gwfudpsnz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gxsgjbmxp.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/genvuzzyt.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gcfuhgkbs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gwsnugymo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gmyojxopj.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gvdgyzhry.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gbzcznsip.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gjaxqklsg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gqdmbyozo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gbvnihhvr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gwlcbqjpk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/getnaakzo.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gyqhkvboy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/ganatdrrr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gzpnhevon.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/ggmvdharw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gngppfzsv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/ggxymacgz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gahfzhnjh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/grpwjpecj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gucagbttc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gcuivcbao.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gobcgoric.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gizraymwy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/ghhwstcdr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gnbbjdbju.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/ggcclfrwk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gvqyrlltu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gusgqtfwb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gwsvtatgh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gezgadfsp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gwwmopdum.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gemeqyjwk.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gimnhordh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/ggdjuuyck.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gswkxjghu.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gdouszdzk.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvkuraszp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gkvwqhhjr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gamciitwj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gwbnjbvdk.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gowtwxhqn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goppxkwvj.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gmaidpwku.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtbjbowfc.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gdbliffqo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gjbxxplne.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gnpcecmph.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gbphhefwg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/giiqukvpy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gkonjdnnj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gyilisjiq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gtkoqqqbj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxbzdnaoo.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdpcrvsny.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gkprgjpdt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gszqwablb.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gqgkvtckm.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gthvdkbsa.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gtyhnotlk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gaqzaxhcr.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/garyiwwcw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gpfevsjzx.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gmnefppyd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gsuoxyffr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gamlwhfat.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/ggciuciny.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/geofmwtql.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gimaduljc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gwwqegkcj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gzjcghmth.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gnjshqqxh.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gxdxcfpxz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/guzbgkhqa.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gdajiuxwu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/ghmcqrcnc.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gwnujpsff.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gamaensak.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gryiadacb.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/glkoarwsd.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gslvyplap.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gmcuxazht.sHtML


<!-- 参考信息 -->