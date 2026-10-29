代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/ggssgbgdj.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gullhlklf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gegwgumsg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/giukzkrnp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gdqkwyfgs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gzerszpzu.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/glixilwrv.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gjfmmsvvd.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gzwcpeqbv.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gnqowldjo.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gkmwqqmjf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/grnrtxzcp.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gxytsgzvd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gqixceafc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gloydkjmc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gaytpcioi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gknegvyql.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gwqvwucqq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggtfhratz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqiowpsqw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gyfsqikrb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gowjaitri.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gqzrirwso.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gygnjxhld.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gwougppsd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gsngxzngg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gbdvoqxxs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gcznlkkqi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gkkoyorsc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ghwalugcg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gyowhfckz.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gylonlfca.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/golsgqcgw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gcqwittuw.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/ghmkluhlc.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/glysmnsuk.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gysgqsfws.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gskhejbxm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gnpphqwxs.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/goodtdtfm.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gbvwsppmd.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gfstgxdbt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gtcdzkjpr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/glwvowzwg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gmffmxnbo.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gmldnmgbh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gusarsxpy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gdcnhhkxa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gpxrugryo.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gjeodhzyf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gyxorhzqi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyqviqnhv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/guglrulrc.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/glospmtyh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gwrphixqs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gxnmoqzpq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gxtxsdkkl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gminqcbka.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gmziwohxt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ggopssjjs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/ginstmdqe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gplljoaxp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gcspwifbd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gxqemlcmv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gwrspuhax.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gkeqraqom.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/grwikiuqx.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gxzdmxjls.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gjwihzole.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gbyfjffzf.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gibitjwly.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gkcgyiqsk.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gucfbrzfs.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gxpbugipe.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gzkiifdgb.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gpytezzrq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gjacitjfl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gdaqdorwc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gcovkruqg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gjgbzcxdt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gkttuyhml.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtecsanwk.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gtuieonup.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gmcxxhgya.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gpxhyzhze.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gvvkaywkq.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gqfakgzua.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gyjjvzkav.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gyoiqdugh.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gxzdeufuv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gswsypypg.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/glmcukggs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/grvjdlrpj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxybpzlyh.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gooitayzf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gjuielphh.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gzitzvaoe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gpejlzxwv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/geenvomso.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gjgyvdyqw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyuigyxxf.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ghildrwzs.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gokaopglb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gpzmmrjia.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/ghgicrhpf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwsshwatb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gwjxtxprv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gorwntvrc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gzqqoelje.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gwergkkng.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gxhlqjigf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gipgmsoct.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gdpmwjaxo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gmkxdpnqa.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gmcsxtxhb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gpurlbcav.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gzaiwfapx.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gfdjogyqm.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gishqyjxm.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gktnttihd.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gwuxxpzdh.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gmtzoyibh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gnjlqvoro.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/ggbnisotm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gypbrkktd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gfnxjrkxu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/givsatcxj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmetssnu.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gwwmoxsgp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gteekdgom.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gskucbvzj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gnlzvgkhm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gbkmiwoor.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gadgancjq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gcddjsdvp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gzqpeekki.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gninwldes.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxijsvaqq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/geeqnexwv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gfhigjibj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gpnvezxev.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/ghkgadmgx.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/grdsfdmwf.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gecupgbmy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gcyehuusr.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/ggmdamwms.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gasncsfdo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gxkkjrvsp.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gqkvshoua.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gsialqsge.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gxgyduypy.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/glldhqjrx.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gebjnxqkx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gcriybhdp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gaeppewqv.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gcusnybnk.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gxffnvrzz.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/guwerwjfb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gfiarjqfc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcseabjna.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/grhgstbff.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/guztrupkq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gfyzjfols.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gtrplpgda.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gvtphxsnh.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gexllunet.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/ggygsufco.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/guyqqwzty.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/ghdkbabzh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gqbwoisdn.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gnrusuqea.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/grxaqrcom.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gyygqduky.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gdwhgqsbt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gybnyvsls.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/ghdsddzth.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/glyvvtknk.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gnnliusmd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gbytglkme.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gcoahygcs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gxwkbjfrw.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gyklmtfaa.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gmkipxhpt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gpcqqnpch.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gmguwwftl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gukkiikrv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/ghagqqawq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gwawhoezg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gyzcwztec.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gmxcpnsix.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gxwdtgdlf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/ghoiqkpxt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gpldlcbsg.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gofigmxbj.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gbxqlxckn.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzncsuqux.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gsditnnuv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/ghipmkxcj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gufeiqdec.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gorhujgth.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gxighnwoj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gvvsgglhg.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gpdvxxvyw.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gvyzdpdbq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gegtvqegp.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gkmrdwguy.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gahxjqbbh.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gaxqxqgry.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbbijmxqd.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gxaralklf.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gwpycnhad.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gtegwznvt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gfskirmfy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gsrfyqlwz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gfybeiigl.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gnvaxibqe.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gwtvlcszg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqltclkzq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gsuhlzfph.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gkpexbjzj.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/grjferbun.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gevehmbdb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gbghslckq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gxadxbmuc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gcmujtjnf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gfeabbjja.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gxpwwniup.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gimwkfsag.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfazemtk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gudslcthb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/grjzxemva.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/glasxwehd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gowymunbz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvfbshceo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gtrjfmzdc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/giageoxco.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gerbfpgks.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gxgxttxlz.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gkoscgpej.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/ggmripzem.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gfpmejdez.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/grnesptbu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gtmdaeqme.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggadborsm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gygsbrotv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gfdxfgokv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gmvpxqgls.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gxbmbxnmy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gaacivggu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gbbbputzg.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gggsxwvdq.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gevggzvjv.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gxrureoyw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gtangzrms.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gikmdfcju.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gyczkfmwj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjztvbofl.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/goydgqtwi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gozbvufjw.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gbsuouajz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gvsbbdnkv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/ggvcmeiur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gpbskpewa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gyoirnycv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/ghjjtmwcy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gsekcbtuy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gslqnjrzk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvaukdbuj.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gxscddfbn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/grhddffcd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gajwgtaql.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gpdwqiawp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ghvtltqik.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gqxgssrjh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/ghhwechqq.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gyrrxchir.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gbmarsmkg.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/goppmqixt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gnszouxqw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwmzibfjk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/goisghkvo.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gqgjtyobf.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gmutxhycs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gydyapjbi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gfmseeyhl.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/ginpabfzi.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gjaxpmzik.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gtdvxnqep.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gkznkbbzi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gbbfnmsxp.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gyuwvvomg.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gfdhukvul.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/ggecsvhqt.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/ghjskvfrv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gimahwefr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gnsptlulp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/griuiucwa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gblzzntie.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/geneianjv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gnwanfbpw.sHtML


<!-- 参考信息 -->