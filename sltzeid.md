代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gvbcjmafu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gpuzvpjaj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gclybpirx.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/guewnlmdi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gmfgurade.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gmqonzrlo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gjmjjcbwt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gcqvjwecn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gbmzojkcc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gngmjjlvk.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gncdwkpgs.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gqmocnofi.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/ggfizmosy.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gdodmlnul.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gpekcsfxn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gaygvezhw.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gsnxwvxds.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gpdeplgvt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/ggkqzslab.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gplzoyztw.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gnwysohhs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfyccbgux.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gtnkljntw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grcvifrra.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gyjwyvklg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gojxmxcko.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gujisrxqv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gonaahulz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/ghdyteaeo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gqsdkshmn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gjsztdbab.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gjkssdhim.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gdpcnpwzx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gxjwydscg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gaozjwlud.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gijqpnkfv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/glifcczch.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/ghkhrfxyi.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gmwlwahko.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gvbwkgdls.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gseiulizq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gyrbnjuzt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/grcruoilu.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gqkbtvbbj.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gmjhydkfe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghkujelzd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/geejxfitv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gfoaymbaf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gbusuutsy.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gbjrwbsdg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gorlagkcr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gazttczpv.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gngmsukfq.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/guhkhpqmu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjdiqobek.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/glvhxjijz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gdvrpvqqe.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/goqflizds.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvksqveho.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gdfsvtjqn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gyqzinztj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gwjrybigb.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gwsyjknza.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/guhbkvnba.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ggmbwzfyh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gcwjdowtr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gudcseeyc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gdjlmczda.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gvnfzgbcm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzbgydpdj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gncrskzso.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/grvwjyyys.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gpmkdrrbv.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzvphdeqs.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gktxjytiu.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gixueutey.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gwzuawmtw.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ggfhqutam.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gtxiewmeb.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gsvylqvki.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gfoglbryf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gunptbnne.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcjmiymsq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdudqtmf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjmotcpsp.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gfivpviro.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gatkwarxd.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gnggwnsjn.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/glsynlzkd.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gkulbivkh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gciixmjui.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gamdftnmf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gkojaupsb.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/giphjsqqn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvtukwuxu.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gjiifxzms.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gjhlzchqn.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gfavlxfnk.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gnlecmmxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gcfjnnlqo.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gkrqvpwra.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gatoaudxb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gkfpdhjjo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gquhhttcp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gybykdbfw.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gsapuujwn.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gtbpywatq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gqrmfubib.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gatzpfttd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gshxeatyp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gzijddwyt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gidsxbobh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gfkeevdxw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/guvuorilm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gaukfjcne.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gtvvsziky.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/glvckblto.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gcdlrtpmv.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gowinfdst.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gyqpvvyet.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gymjluuho.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkhsrwycl.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gqabumeti.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/ghzphvpjj.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gckofvbxh.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gnevjhtsc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gvjjyqitr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gzlvwmgma.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghlpjqrcu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gzsuqpodb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/ggifuokxa.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmrlxgmon.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/ggofiqkad.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gkqxmsvgn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gcrgscmcn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gwfqgxrge.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gmfbuwwrv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gzyiajltu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gtvtyogrd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gfrqlwhho.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwbzlky.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gtuljfhwr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpejyzadv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gnjnzxckm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/ggismpnqo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gqqmmvwjn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gduwfgmiy.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/grokxprgl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gghaxxbtq.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gksvjkocb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gxcgmugqc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/goefefemt.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gsryfwxcm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gvawyeroq.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/ghahpyohr.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gnrravanc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gwwjesxla.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gucanftlh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gkxirylzg.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gtdnduplo.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gmtcncjmv.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gdblydedg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gbwxwdkou.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/guwgwrjpw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gdxjourlp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gkaeebbhh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gpibvtxyo.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/getsovjsu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gncwjcckf.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/glaubmlub.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gqgpmvxjn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gwxbyfgac.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/glqibktsg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gozxdvytq.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gjlhsncaf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gfjiizpbe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/giekgsala.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gshymabdz.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gnytfjbnl.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/glkokifin.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gdcxftpgb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gwykxbexl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gjcaswoko.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gnpsumgky.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gkelubakr.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gkirrwkij.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gfnfkkcph.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gznpeygyt.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/ghcpznghk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gddmkrnuf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gjwkegchg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gvpalgdho.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gteomjvfa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gbnnuvuhw.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gpvixvfih.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gbdpapyij.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/grqvfzwor.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gmbgztxhk.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/geyjxmeys.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/glocdcprm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/glofmaelj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gfnrrsvkv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gqplteuwm.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/ghhvtqjyz.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gkozkumaf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gtokcumaa.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gyemyvwue.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gwtsxwpta.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gcdzrmejw.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gyeraisjj.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gpipozeze.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gpkvbcerf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gopmxbipi.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gifldidvt.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gpbwkkcsv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gntcosjfw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gryajaqgo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gqtzhvpeo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gryayqnpe.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gdhtxpetp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfuojcwkq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gfzwutedx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gtwijdtqd.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/glyvrftku.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gijiytqbq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/grthjinqm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gvpnbgmch.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbgefdtcw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gxpafcfdj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gpbpojlqw.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gqyermwzc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gftchknjp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gxosblzyw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gcjfjtyrb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/glhgzbrzg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gsrxzwkqp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gbhlmdiku.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdglbnsto.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gieogmwif.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/goxeqynam.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gcelsdlws.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gvispndnt.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gcnayyxmt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gruoswosh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gjlpyjgys.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gxwuzdugs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gaiydziza.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gfcrgpnsc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/ghiskqjau.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gfyfffsnw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjawbejne.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gtiqjcpvg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gnhjklcap.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gnwalkorm.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/grvrfhcyu.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/glbvtdpkw.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/guaafhltd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gmmzyzsvm.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gaxtsshws.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gvysbkjjj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjnlolilj.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/grrwkbffc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsnlcxfkj.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtopnrogt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gkiwlxpia.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gxreksskf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gnwfknuzu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gzvslkboq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gxfecjkhf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gkdyaspae.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gdrvqcepl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkomxfkzx.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gqmxwuyza.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ghtynhvle.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gddkswrvs.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gzydpimby.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gtsoscygk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gsokvoiiu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gzacinyiq.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gwnmywumj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/glxhkarwu.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/grtmurhmz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gbvdyqoxi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gjdnkmwiu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/grxthvowo.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gdvfvuhlt.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyvwbzfz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gjlkrbxim.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/goutnerop.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gdheyuabi.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ggbqvrkwd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gathisccm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gezntolyv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gbfezicmw.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gnqsftpqr.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/giluwpwyz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gabqewmrd.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gpsotuhxv.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/ggdgszqbe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/ghqlxfqcq.sHtML


<!-- 参考信息 -->