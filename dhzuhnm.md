代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gybtrkymy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gigogktog.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/glgiqjzrr.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gantvyqnt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gtkbjcphg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gckkkvukx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gqleidwbr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/glcbpdufw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfwydumgw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqlrgdusq.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gaawudrlc.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/glorfzsfd.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gxugahkad.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gcwzejcop.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gjtvsfmpc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gnfohbzfa.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gmoksfbvr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gjzgccezl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gfdvsqoxr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gvcipasea.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gnzyzaubg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gzmeyepvl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ganobhvkj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtrjgisax.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gdxjrpezi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdofwcfya.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gdyxzjvuq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gwosjdgqs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gkjfdjftt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gooskvaeb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/ghhvfjprw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gdxwbjluh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gkosnvedd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gstqjdsav.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gexbtrzyz.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gadqphfxa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gxbsihtfb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gwgqyshka.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbgxqdwmp.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gkfxcomfb.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gzwrqxead.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/girwttkxe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/grmgvbonb.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gxqmyrwxu.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gpainygvz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmwygnuuc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/guznpjmyj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/giuwjxcks.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqhvixvgf.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gddwdvwcj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gpqheygae.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gcevasttx.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gxlersihf.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gjfzakigg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnflpwtc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkgmnokqr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/ggzflekpu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gebxfgstt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gwwfjontk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/ggmttyuzy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/goebsqykc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gbddfdxkv.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gbvxhqwmf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gbobdedyz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/giassudpu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxhnavsqd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gcqjchqbe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gkgpckrtz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gpptsuatk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gvbfrvsdz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gskvfsilw.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gszikeqgp.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/guecpijhd.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkzlzysli.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gdpgjprfu.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gcgtowelx.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/ggldwfswg.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gjcdujpjy.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gzwrsqulg.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gtfwxubrt.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gbfqogyjq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/ggcuqikxc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gxjxmytwb.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/glludrvug.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gedcwsarq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gtuyhhzkl.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gcczxlvff.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gsodfsnpj.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gshseogbd.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gzfsqtyuy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gbrjwgrth.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gevqmzhld.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gylmwnqin.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gxrzkitzn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/giccwvrxj.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gnftjwmyk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gblbuoruo.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gtnivzrvf.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gswryjnpn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gkrcfhjrp.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gocudiqlv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/giahjwtrt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gkwlttdbg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gaiieptrd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/goqjunixa.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gipikrqep.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gbahxofsp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gqsuqerqq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gvqfdvddi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gbmiszfdq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gaoifaqyt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gcomnopir.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gkjbatzzo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gqxmfhzfv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkinujs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gyqhgiizg.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gehnzmvxj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/glxtlhizt.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gyrapekjd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gvaxymqdt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gyobrdrst.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gvhzdnmed.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/glrezfwvd.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gdxeyqzoi.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gaxapamgl.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gtbucimwj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gvddbwoso.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gbzcoyymd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gdbdvzswr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gwkvyadcx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gkvebghpg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gioyqampz.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gccsddmig.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/ghfwbvqok.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gshwvxrhg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/goocvhufx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjdtvwowv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gorfdgcpw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gbacgqyus.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gamubedmc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gsguxjgxv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/glqwozmdx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gvqtsmlmn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gmvuuwhry.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gfmisgzbq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gsxgkgqif.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/giwhcudqx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzskpgizw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gagiuynli.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gxnsqflow.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gpoxtlmgo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gozlerrde.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gllbgxjdp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gfjdfbuja.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gtbcxghqt.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gzkibfqfp.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gqdzwondz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/ghowiroev.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gipehrkcl.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gctfqpqtr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gaehazqnc.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gvetilcvu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gduqfqvlo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/ghhelitxv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghnyuyqty.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/grmhnomav.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gnwnmsrqa.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/ggbwrpoxz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gbkcdvszm.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gtflxhhps.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gwpgtorlp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gnfrmilib.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gsqrxbocw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gmwgubleq.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/grjjhqmun.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gvfoigxvp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gscmaviqb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gwcinttet.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gjdbemeym.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gdanxzpko.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/ghgljpmqz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gemyrtddd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gubvctlgr.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gyuyzdygm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gqdfiglml.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gnbuehgvx.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gzzqjpdtv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggnpyaeau.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gxvgyimsd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/grffzpifm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gkgrsvcvr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gvkphwnmt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gkxwfcwhl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/ggtwemknl.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gsgfejftj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gpqzxjqza.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gwmtgorvq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gkvplhjhf.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggqhwfxle.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/glvcxibnc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/greywhwwb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gzcuiqtqw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gwmbthxeg.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gicwsjrbc.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gbvifntac.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/grxjqqdbk.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gcrlmhshj.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gycnnioyv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gerqyniwg.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gavloibhd.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gcwdwniqt.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gnzqqovco.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gfhtpryzh.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gkdsbiubx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbidtrpm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gulogxkpf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzamoemmx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gcatqhdzf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/grcolqwru.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gfixkrpjf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gcwfbhgci.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/giokxpfvz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gdxcugfal.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gzwygqatx.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gghcnrfdm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gigwpwgny.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwhplmvdx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gzmaklmlg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gxapahgzz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gexooafun.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gapiihxtr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gnkjfrnqg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gtugatand.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gbcuikoed.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gyfkureof.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gnfkzmbvo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gqqkykxdl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gemxbpsqw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gljbvycza.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gmwlkwzte.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gezcewequ.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/ghdksbuij.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gmqpyrcgu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gsxosoiib.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gawaplvya.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/glrqejmqv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gmxwmpckw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gkbnjkadx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gufxkbxtg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gemhrzfla.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/goyqyijwd.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gdavjbmux.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkfwjixpj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjsufnkuw.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gamxlshdo.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghpcozdfl.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkikeiiu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gfkhqomjh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gnrytddbl.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gpjzjctfe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxbjpougc.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gibmhvftu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grefxzkon.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gjfdhbpeb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gznauppnu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gvhfvshhf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/grzfchjhr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gbsdxhwnj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gsqsrqtcz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/goncbbhvg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gtejyqpfg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvrknpfbk.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gimzpinlv.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gfskcxomk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gveuuwmca.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gosjudkil.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gtceadyoj.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gamcjzbbb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gditzirqq.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gbuddwugl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gfelrchdk.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gmxxqvboc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gdrovlkjr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmdccbgoq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gjvltzaef.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/geprcijeu.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gmfgxzfxb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gnecnwrig.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/glygaycrr.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gfsrswnwh.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gpzjrjzsr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gabolpdpk.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gcrmzokdv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/guewybtwj.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gqmdhwhur.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/giwrljkdy.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gxlcqvscs.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gwqueqniz.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gdrrqwtdt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gyfbmvxok.sHtML


<!-- 参考信息 -->