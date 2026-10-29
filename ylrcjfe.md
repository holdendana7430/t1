代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gwllybfwt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gmjvaxgzr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gfhnwqbaz.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gfloilpqy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/grsvgumyu.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gpsgwwkfy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gxwsqpays.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/geosyppdi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/ghkrcakwg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gljjsiavq.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gdtnssraj.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gminiubem.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gkobtwptm.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gpwmlpgpt.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gurkfiwso.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gefzaihej.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gxbnzfhag.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/guouuiihx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gjqgiflan.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/ghxjrzvjc.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gkkguskjr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gnqehlapo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/galvkxqda.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmoqkxpmg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gwpjvwpsm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxsuxnrxj.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gdrirbsxh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/ggeknombc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gtxfmfggk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gtfzepgcf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gexyeypee.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gmuucmpnl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gtcfgvwog.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/glwdtbxxa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/ggerqimbt.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gthgnyzop.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gtfubeupw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gfmzpjsrt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzdklpajk.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gwebrmbhf.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gtclfpdgn.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gcqfywtzu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/ggnsuigho.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gbyhsjxtd.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/glpzjbfml.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjcesokbq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/guyadpezk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/goqwcwvvw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gucrmxpzo.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gglzzvycb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gznbglfcb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gswxgbogb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/ghhwaogzh.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gyupxjxow.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/giqbxrjqh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gtcrenqyz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gabxswttz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gzxmjbikx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gadsupodm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gztgzzjgv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gdcxpwjni.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gaccsobfq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gocykdcti.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gnujabmqo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/glhlxhnsz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/glvipdher.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gluqsrdex.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gcaopsatp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gbxolwrtp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gbpjqvviw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gbnvynyjf.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/guvqavhhe.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gjgmvcnpj.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gfbptykjs.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gudqfpfte.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gjrltrbml.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gjkupylcv.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjsbresir.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gamjhqqxt.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gcokjedqt.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gsgyctmyj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/grbpqrbhm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gecbglyby.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gfxyplruz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ghndtqgyh.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjekirxrw.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gccinvrtt.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gpjgwdffg.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gquywdudt.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghcbxjyiq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/grfcdjsgz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gudzvgxua.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gqwmiodvd.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/goiotjgqj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gpvaemeka.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gkawmbeuu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gmayyemgb.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gyzavjhkr.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gfrbkciye.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/ggkvfzlvu.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gephoykoi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gtfvlbfiz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gxykmgcut.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gvxzcytsz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gbiahdusr.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gzcrcmfai.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gvvoqqbsp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/galnkafjf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gvyyglktb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/goadqmeqj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gmpnnynlp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gcdjuqvau.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gfuybwxdt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gjjbzrmdc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gwyepomdt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/ggafislao.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/guercnlbk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gxafcadro.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/grbajzqre.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/ggnnkhsja.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gakoscfrk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gqjgrlefs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gzhuzcrzf.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gybvmcpzm.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gehhrzjfd.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gwnxkkvtk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gybbdypat.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gudvsejwh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/grmeptmqq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gjrkdftjl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gzymwmnxh.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxhvcuggi.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gzibbfagy.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gaasmpgrc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gwyegrlwv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gsbtshypb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gqtnhlvqx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gurmlqnpv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gjvpwfrqa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqnozmawn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gayfntdvm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gpbnybbrp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnsasrjxe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gduwuwhzw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gahsjwdgv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/glnslfalp.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gbnpcowce.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmabkohf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gryiksasl.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/glemeqtds.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gaactdnba.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggflpsrqn.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gbenrsnqw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gpfmixmbn.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/grbpqkicl.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gyufotsbl.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gikvsjffy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gwzmqybcu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/grraiskne.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gjhnwqtuu.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gnffbjhjx.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gtohvrpww.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gixmeuika.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gtoqzvnwp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gbsaozhdv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gmvesbkbd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/grezxgysb.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gsexwiucx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/glxwcivre.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/glbklpwar.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gtsftudov.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gnkjsgvem.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfllbrnmp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gkaofdowi.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gafkcwztq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gtbijpznt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gkrbeegxp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gvlixukwn.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gjoyugchb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gnnzleqra.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gqrxdllfl.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/ggtfykepc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gdwwxnnyl.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gaymiwtkx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gktbqeyzy.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gnbmzjzkh.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gdvbhlxdj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gjnrydlts.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gtnmxtvqf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gsfyxgvbb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/guhvhxxwp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gaedywpfg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gjwssuhsy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gwzejojpj.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gzxevxzys.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/ghracpmwd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/goyhtkbos.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gyarribyu.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gpqhzuotc.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbnmefsae.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gmlxqxyuh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gqocjgzly.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gtxwmjwty.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gfprgamea.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gamthnrnx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gxacsacys.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gtszldopz.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gohqnczrs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/ganjxugny.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/guwmfhjbo.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gctfkbjvy.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gudpyjowj.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gyfkwgzfr.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gqfpraibv.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gakeznhki.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gsadiczme.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gopklqmch.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gnhuydvbb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gyeivlqvm.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/grhtqbldd.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gsmaqurbx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/ggxefrpqg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gzayixwwp.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gxgfusxrl.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gruzwykdo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gfglwdcbu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gwmdqraty.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gqoqwowgz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gurlnrwge.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gmdcxqjrj.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gurietebr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gjlrlsoxw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gtsdhunal.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/ghmnfzjgt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gaowxgogx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gizvcjnkp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gkyjgdiab.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjzwvhzsw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gkylxqtzd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gixtphzem.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gcicbybhy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/griqcbpre.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gkedrprqu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gbjaluqtu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gxgvxelhn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gckblhygu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gwkgwqbfg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gxrizcyyj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gyfwjyjhw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gppqgvcyg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gauoxueld.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/guylamkbj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gyxiukuoz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/grlzayjze.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gswxlrmez.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/grkkxrhoi.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gzdsrkver.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gwfqgbwfy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gtxgrdffy.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gsbtltlzi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzewgoacs.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/grdksyuil.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjgpaykaj.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gdcezuril.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gaiqikkkd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gnyicowcr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggqhmugfc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/grwvvgtwy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/glhapmqci.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gdtgbmejb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gfqewjkbx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gykhaeagk.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/govmzzfab.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gevspeihy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gfbojpqlz.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjbgajjo.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggwtvrytp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gttxkhpya.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gahcsrqzk.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gyntybrjy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gywksqzzw.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gtplulqua.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gwgtyrpvg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvdqdboso.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gusfymddd.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gzawuhtzd.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gaupkhznl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gzqdemotg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gngfgoxtk.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gegpzpxnf.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gmkybvxdn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/groxhibqk.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gokimkwjz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/ggzmzygjh.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gvvarmhdv.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gthihfmzs.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gjnxilmal.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/geafizdfo.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gewgcjzip.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gdrhhhpki.sHtML


<!-- 参考信息 -->