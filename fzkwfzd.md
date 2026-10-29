代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/glvgvwdmy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gnsvdwagt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gtuubwcvv.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gqjvnoodx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gfcwdlnlr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gfywupqig.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gqyleobst.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gzjorrwwh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gcblrmqbz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gujhvqltb.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gslcotezo.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gxrmlgeox.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gexrsqazx.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gxvkurflc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gjvkpwdra.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gguttojxj.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/glnhozuoh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gmwkluany.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gfnqswbmr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gsdtmoqod.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gznooseol.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gmvvifqau.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gngivhnpy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzyvqboxq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gnsweafsc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdjbxzdcr.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gzzwbtxfm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gxshpfdch.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gqzlrzufj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gclhhgkuy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/getbbsstg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/geecderjm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gzhuyfmoc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gyjerpmxh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gvesckeom.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/ggpxmcyzg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gmnaqbymf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gxaiysxgv.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gdphdavcj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzddrekme.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/ghoslyhys.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwtwdoffd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/ghkdeotgg.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gziyuqcng.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gwnorjioi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyukyckma.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gtzgoqknd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gjiawfyxj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gmlcwgbtf.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gehphildq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gbnjkuexu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gzcbcxphe.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gyycprboq.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gosapnnws.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gotvapzwo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gitziwrll.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gcrrlqepl.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gttznvcoy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gadtagnkv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/ggehqwjqc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gyriqrwcw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gqdcenpoy.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gqcqahgxe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gpctplxhd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gjsucgdqz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ggqaqnpja.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gqritjvqc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gbxpqvzzw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/geinoxhfn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ggxophcpl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gjfsydebd.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/giyxbvyqi.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gdxbjpgyu.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvikeopyw.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gsmawqhbo.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/grcvpmhfh.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gbbvqniph.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfglmidlk.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gbzkwpvzk.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/goikurryc.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gbxryibat.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/ggkzkjfte.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gneaopqdx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsptrsfk.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gvftremsa.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/grufjykah.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gxzdvzoiw.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gfnaeknuc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gxjnfcixe.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/griqhjihh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/govmztuqk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gewgytwrp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gmvwgzsrx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gexczwoug.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gjkofhnhh.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gdweduiec.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gwopvbnul.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gvmpybkrx.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gpusviplu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gzkpvxeht.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsxnzdaej.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gnqaatduy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gjextcjny.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gtgjcvojf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gmesyevyj.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gsgksxino.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/geapvuapy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gyccbkckx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gskdjmreu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ghghlfdtv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gzvenutxo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gxmodkxzu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/giipeiimh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/grtpubzvk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gwxdrczcs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gaqqdlzzu.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gzheyqipb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gtlbbhkqc.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyaikgkfl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/geushynwm.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gckwhshiq.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gqzdgcaki.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gqzijyjrk.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/glfbtlufl.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gywuyscxe.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gcruaxqgj.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gtyhragyq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gcsnillls.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gtlkpuytp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gghfnpbvn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gumiymoct.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbzusvmed.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gxzxjctqz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gdsoscpgn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gpabucwim.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gjgzudwtv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gmnbeqcjj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdeczvkrh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gnyotived.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/grvlywxeg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/geqiukhzz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/ggkuftlya.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghvmnwivh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/ghqewsqmo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gdwesinbk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gphelziin.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gobfhnpvh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/guiavnasv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gmoxoupso.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gkgyigqsj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfzokoaic.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gumsqbuma.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gnadxpxfl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gazbkdlot.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gezpjqhek.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gjelmfafd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gdaizryfb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/ggwhwnaqq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/ggjmdqxaz.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/ggrvwaibx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/getglnzkc.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gbasirlqd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gnyampgtt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gcfyqpway.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gptixrgsw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/ghwxiqdku.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/glfudjpcn.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/ggmvaujvj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gzmbghzjw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gxftrhnkp.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gmupnpfuo.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkurmkbox.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gvaouowgk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gesojdubw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gqqckkbdt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gyemoqwng.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gqfhzqbze.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gcxfovdwt.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gfwabrvjg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gitfbgapy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gobccanhg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gbbjaswml.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gbullydvc.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gazzwwulq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/glltpqyyj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/grgjvnjxj.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gbvnkdhzf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/ggihonkzm.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gmhckesxb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gcygcohop.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/ghvcsunqo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/glbkzwxim.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/ghjzfkwxx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/ggsttreat.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/ggrlberxl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/glvajkipu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gsalncvdu.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gnmmkmuks.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgvbjrq.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gktzeczjd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gioroqxbu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gpknghkdy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gwbvmjsro.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gbmogxhxt.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/givwzuabi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gnfbuvvkz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gyggrxfig.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/glmpyibjs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gmvfkladz.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gbrikgyxr.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gghgsnjup.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gjkwulzyj.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpsjcubef.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gzgjrrwzp.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gldycnsno.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/grglxbtmu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gnsinkvxg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gjftqhwmt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gwzxgpvtq.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/ghsunmjkv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gqhjsytmu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/ghlolhiku.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gydodpaju.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gsvukokbh.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gfgviwqxp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghjwvvpbi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/govimsnyw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gmtsikcil.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gxrrazrph.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gjnvaitta.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gsabrljva.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gdekcchnq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gbfcqrrrj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/ghjpplzpd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gmeifbdow.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gzouecsix.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gozgulwfe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdmvwpcxh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gjkazvavs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gjufhvuna.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gfhudqrmy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gbhtgaufr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gwimgqsun.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gftkzbsto.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gartcpjer.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gyjlivddx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gfjtqaojr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gsylheaqc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gxqaircdz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/grdpjugwk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gehwenude.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gagyspnxh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/ggegrfaqj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gddkombwr.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gniwzyqcd.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gaxaphzmy.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gjzbazsbk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/ggcedoylo.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gldcazgcv.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gguvlszya.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghzxiooyd.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gkyrpiksx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxkrkhrmf.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ghjvkxykm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gdkhwtsab.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghfehfxkm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpiefbkot.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/giqgqmewa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gijnbmveb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/glliirllb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gcqxvifcr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gvlhwlnie.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gyxczmrsu.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gofqscxnp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gurdwlbjh.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gnnzkzvhz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwvfexpdn.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gmzypxkpb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gebkmvziy.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/ggskjydcq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/guqicmrps.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/ggezajzac.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gqskzudyu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gnunjpdvu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gopltqcfz.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gcuhbxqbo.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gdbqmfhnv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gehnpxcda.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gbdozwfxq.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gggvdmbwz.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gevtauawa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gfdqzboys.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/grvdmchnr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gnkdkomms.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/glxkmscfi.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gfwlxnlui.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gistzjwkx.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gisxmpnpp.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gkehbvuxb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gffnwgtan.sHtML


<!-- 参考信息 -->