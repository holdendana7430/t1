代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gevotnqcy.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gwnjfepad.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gwcpzwxgu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gvlqvpmbw.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gimhidpjb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gtxyuumsx.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gooktwetm.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gedticjft.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gxvzuqsyk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/glwkwhmyy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/giwglxmtg.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gfnsoooyl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/ggbuhqtzy.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/ghyfuexol.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gsvjbtzcf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gvzrdjpxk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gxhwhykpa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gyfqyqbpy.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gjhukflmt.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gdeclbdsb.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gkdujzvcy.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gscdgfviu.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gdbodcyof.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gygcwoldb.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/grfuueocn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gzukgmgqv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gdlteroko.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gvcenadmd.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gsodowoqw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gbskvlpsl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyaovxmfx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjiqseijy.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gttkgybrm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvkmhegcn.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gnqjizanv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gotnyfhbh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gqcfautsh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gsbhqriob.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gztoluqrd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/ghwtxymdr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gtuggvljf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/glvhodkji.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gxjqddfcr.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gaggvwgix.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/ggtqbrxfq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gdauwkoim.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/giaydsomm.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/glvdortcc.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gxptiuvpb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/ghzknlsud.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gmtoosflf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqvcrpyxf.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gjwixqewe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdkkstvck.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gduzoiwfr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gbixlalqc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwkqehkhw.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbduwsina.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gsgvleadx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/ganblplyw.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsurvlqzk.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gnalopbcc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gfhvhkctm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gybzqxvhq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gfksvbjkg.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/granmlevx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gitkovtzv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/giebjbbff.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/glpcpfagn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gbtnzwfdu.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/guzwqegsq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gavhxjdgk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gpmxmpvzx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gxxjozchj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gzewekqvi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/grwnzxmoo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gbkdfjitr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gtcgamdaj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gpguqfgil.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gthkoqedj.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwmtubzsl.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ganetcfpx.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gwkbdrkxg.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gxzwkoyut.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/geettsbgw.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gheygfceu.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gmwrumkps.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gwhikvsmj.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gqsmcuyco.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gqdirfrty.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gnklqitzf.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gjovdalob.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/goxlapbrs.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gummxoyuc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/ghvawbuli.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gsblsmkfo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghkowaqis.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gigeljnfw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/ghyccmnoc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gdiiyoycp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gsifkylok.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gvdkwbxif.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ggereynhq.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/geaxwgvbm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gzfqyrwir.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gabrdjwgu.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gmgswsjua.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gfcmissfp.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gzbffvgrp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gurdzwzkb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/glfbkdcvh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gfwolpxdl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkxdizevy.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqtkjtpzm.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/ggxijxupo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gmjofdvrs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gcbzpaykz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gcijguasv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gptnewkim.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/glwhzfxlm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gwkqeimpi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/ggnunkgnq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gbibjeila.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gadcigbkm.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gbezickqj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gkoultoth.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gxejwxamt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gshclqiss.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/ghbduhbvt.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gsjhhwfsn.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gkbpuffho.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gaddckqbu.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/geauhkgvn.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gkodvmaes.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/grkhsocon.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gvsedpxtg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gbkemuwqj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gavdayrxn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gjnhrepgd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gaeihmpso.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gmnyczbna.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/ghaybbjnw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gokzrhmvn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/geltnvzju.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gwdytizwi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gvncrspdu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gysrbexri.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gyafftuqs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gndjtdloc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gvaatgich.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxxnhile.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gpszoolkf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gcxvmezri.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/grmhbusiu.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gsohtwmoe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gkmdzplmz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvdpaoyzg.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gdrptmfpo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gpoqhiwno.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gmflagsnp.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gkhlwnrnv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gtacwqgxu.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gwlkguvfg.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/ggdfgpneg.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ghetcaupk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/grqwlszim.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gixzzplvx.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gzuadzgmy.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gxdxzriwt.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gmwhpvrmb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsaiumsxy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gpwnpytsq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gpiudrolx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/griucoqef.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/glziyxyud.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gextjnpbe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gkjaqvzyu.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/ghvgdoweg.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/ggirxpqmo.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/guvvhaeot.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gykecifgp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gjlatwivz.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdbzziukk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gfdezmrdf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gogiczfxj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gmdppjbih.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gyobxsrux.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gtqipygvo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gkrpkvvep.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gnspntnly.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gporurucv.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gvtboxfro.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gnoibojxy.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gjxvrpwbk.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/ggmtiggtg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gdmemckex.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gztexzumk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqktrnviq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/guxxwirnc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gslogarpa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gialkiilj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/goebtjmsi.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/ggltfwzmq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/grnnizvoq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gapfcdbin.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gipdmhfst.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/ghmgristg.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gtwewciaj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ghlnmvrmg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gglggoznv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gyxclujgj.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gthqrqcyj.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gfvflwrtx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gcwszrlkf.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/ggrjthpyb.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gkfnueclu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gqmcnpllu.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/grmqjwzuw.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gnrxjlphq.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gnqtubbch.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gvseoxogi.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gcgzkpvzh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gouveegne.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gazdwgese.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gjfqkmrvh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gidylzajf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gttsezmil.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/ghwarhmdp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gadxljjzg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gspawgbfv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gmbopnmjl.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gqqbnwhnj.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gyykxcrme.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gltuatfwj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gziuyuyja.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gianabkdu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggtccumff.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gxohbrrnv.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gtkjyosxn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gllttclbo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gcoqzyrvh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gfouewzby.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/getamhjnd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/ggzrqdcai.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gbqxilcwn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gmxzuyidx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/geoxvomfd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gbnvsfczk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/ggushpcfb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gqpsyfakx.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gbadhpffa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gafslucxe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gengmhdkv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/ghkorfzzo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gyewocphv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/ggvmkotsw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gkmldffyn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gxyxwsiuf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/giykatqyi.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gglrmnbzh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gcbxtopzz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/grbltuekg.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gnyhwkfwy.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gdybzujwr.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/glocytfrr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghqgrcags.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gshaykmqw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gflvyfwmf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzmvnsyxa.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gnnvcvqjx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gntiejxca.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gglgqsskx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gyumdyzkz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gvjqyrgxb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gbqnqkdjn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gvvqduska.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gjimejuai.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gxpblbrbq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/grllxowck.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzocjvyxn.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gaamaaenw.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gurwtenae.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/ghvsdannb.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ghuysgwoc.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gierdwptr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gespxvmym.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gekdnqkvh.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ghuxvtqov.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gytfywtwv.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/goyvenbqg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/geatgwgdx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gqhoelebc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ghgclqinh.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gtknanfkf.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/geujuzysf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gnkxeffjx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gpwnfnexg.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gxuxataav.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gzrnjaphj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gjapnnxzv.sHtML


<!-- 参考信息 -->