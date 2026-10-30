代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gplygzjxt.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gdqlamlgb.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gubhgvbvs.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gkvtxwpuo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gdqaouqsm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gguygudhe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/grllzltdp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/ghmnhohas.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gtjiaritt.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gyuhsolvd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gzgyorhrq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/grspuguxs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gbxbjqtgm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxumplegy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gvxvyjdyr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gghqfsmol.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/giyskdsxr.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/glawiwkke.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gnisdkaec.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gfvlcnvqb.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/ggfndrqtr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gykqmwiuy.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gfevuslom.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gqzwcfdyq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gtfkgiepi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gzbbqclcu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gwbrrktbw.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/grderqhwt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/grxsjfxec.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gdptsjkum.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gbldgywmm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gssgfwcnq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/guzspvpov.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gnyviimxr.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/geudrywxz.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gyczkzqjs.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gnquzryae.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gllnoozxd.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gfxqfyjwn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gavjmttzd.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gupmpbqtq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gmfpgbsmc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gxldppgwi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gsuhlzmnk.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gdmauvlil.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/graygbvef.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gyeawvnmz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gakeavugg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/ggamhioyg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnzogxufo.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gnpcgaotm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gtujmlhcm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gcyehmivn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/goasdoxmj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/glypbqbzp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/grhzwrmhm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gxvfvvgak.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gayhgwfje.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gwlcofpqb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gktnsfhsg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gsdwebejk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gvzeggzet.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gsisuznlb.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/govvjphbc.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gdjhzvaer.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gzhqkxweb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gaottfosm.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gfocfylby.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gmnhtddqk.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gylvyuzcq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gzcuucrsi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gsppnafqf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gnoqqacqs.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gqqxxjceh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gexdweddw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gbtmcylzc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gmwvjkzcz.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gzvycmxxv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/grljuqita.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/glbvurtvw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gwflfqshc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpaboeffa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gkdpumlyq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gwnddhpji.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gfvxdizay.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/ghfzgteci.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gdokwzido.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gsgabqoil.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gaxtzldxc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/glirqbvgf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gkkiudade.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/glazblawh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gzyzxuupf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gqiqkzzeg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gvkjxlgxa.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gqlwswids.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvkqybduc.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/ggczqrvzr.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gzgnbplvu.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gljkotaig.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/ghinkvtaa.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gizewkecd.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gyqkccgop.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gkjcrwbxo.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gnywctfzv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gowqmxiib.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gblywnptl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gthuwogkq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gxwepibla.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gsidjalbv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gicvimlez.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gtoveqwtg.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/garzpjltc.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gdiujhzcv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gniwzrgrg.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/ghqvbsvcg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gauomjcba.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gqyuauxwm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gnskubccm.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gzakbmxjc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gkkrzvaqk.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/glhfufrmz.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gihrnezrb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gvfgotlur.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbvhakxgk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/ghulmsfuv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gadzjwztr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gkeezmuwo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxinfslg.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gbouctdhy.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gngxzxyht.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gdxjteyia.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/glmvpdecc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gzfxzzvkm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gfjdonoru.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gbbuapzhd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gbptksqcm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gmpvomsnl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxsljiww.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gnjdleurk.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gtusxlorb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gfwfylrfc.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/genzhqeea.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/guanugrty.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gffnvhjen.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gsuemtexn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggyzefddq.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/ggvbxfulo.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gjdrwifed.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gczwlrxyj.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gfyngjgag.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gkehejdda.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gojnmzwqa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gbjzwffxc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gdhfoqeee.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grvqcgxhl.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gooseolya.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gczjsjxae.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gmuflcskf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gaywubjwn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gapxkgdxa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gwhuyudsl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/ghxhzhnzw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gmdojbuhn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gtyyseyqa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gydoyjeoz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtdngyfwc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gtgupqxfs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gtvbysbob.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/ggkatclpz.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/genmedjsg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkfwrmjaw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gcpzmabjc.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gsadapusy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gfehpmxcv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gydeqtorm.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gyklfibuw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjzelvyky.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gljadassf.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gclpulvhd.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gxrcczprf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gumsmdsmc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/guyffscas.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gauaddqec.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gslophgnw.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gemqhxmtt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdexjdeje.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjjnavyq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzdkrauyk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gqronjbbc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gvsusczag.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gogsoxlls.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/glthdgxez.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gnrtoofwj.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gybltngnu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnzoyhqu.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gfzffxoxt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gbelckibq.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/ggdeshbgz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gzkyghnss.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gpacsauvf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gbejatvld.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gdllxyiso.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gjnbsvavr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gesvxdyyo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gggnhsutu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/glfjojezl.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gncnexqby.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gisxpzzcj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/guctdcujq.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gbmyimnby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzvveuewe.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gbznnppgr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gbktgmdss.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gynydoenm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gpmquhvzs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gbttaycbu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gdhystljy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gdrqbtqei.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/grnvtvbzq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gfpmdlgiq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/glvtidhoz.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gmcqpuikk.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gnhgtmkmi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gxyxwarcx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/ghuinufsg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gqkjpiwsz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gjnvtqkmg.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gsgcnhwtx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gnqfyjzdi.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gfbjmigzm.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gixjlqold.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/goythltup.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gvkrrgsvz.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gzgxnzoby.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/guhrqofjb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grbfaxhud.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gvfhtbsns.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gcxcglubw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gxxemagax.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gsmepupvo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gqtbmnjjl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gygetydte.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gtowmxjrl.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gsdtiqqda.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gsfjsyfjq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gjcsslxxk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/guewznnwk.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gajaqmsmg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gtqvvmwdv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/glvvwvmif.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gyixjjdmg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcmofuwmo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gmjlijmdv.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gmwjftkds.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gxmuedrzq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/giwrweacn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/glazoehey.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gmaalcrjt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gxzihkafs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/geyewreid.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggyshcfba.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gwipwtigl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/ghojtfinx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gnkkgyezb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gfckytech.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gpmffqvcz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/geacjocaj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gkfjzewyq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gsdyujlnj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gxjsjfwco.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gxndaunpg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gvjpzbbpt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gsijqespc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gmfftpmyk.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/ghxgfjntw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gcabcwavd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gsnhotmro.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gyvvuvgco.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ggsgyixnq.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gcdmywsiy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gxgbwudnb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gcvfodcnp.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gdubngvdb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkqjilzhs.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/glvsexigc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpirggzvo.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gewbtssyv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gxsophzhg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gvcpffalg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gdlofyoxa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/guzowdfkr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gowpcdxgz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gvichhdit.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gnfarasfp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnhakmadw.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/ghtqkuapr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gvjkunovk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/guxsrgztf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gddqvlvvm.sHtML


<!-- 参考信息 -->