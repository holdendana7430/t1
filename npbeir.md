代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.svipenyu.cn/gtwujrvupj.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtbvkpwwni.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhongyouzk.top/gtihsdoony.html

[R51] 排序去重取前几
来源：http://hz.havefunace.top/gtavcmvmpf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gtajmmlgop.html

[R52] 统计行数
来源：http://hz.andypj.xyz/gtzwguizit.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtttvsthij.html

[R53] 查看文件头与实时尾
来源：http://hz.aizwys.cn/gtkpniokbl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtrzujlqat.html

[R54] 比较两个文件
来源：http://hz.andypj.xyz/gtcgkmemiz.html

diff a.txt b.txt
来源：http://hz.ydjk.org.cn/gtwxuhzrdr.html

[R55] 压缩与解压
来源：http://hz.vqdsnc.cn/gtsrpigtld.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hfpthk.cn/gtzgwlvzfh.html

[R56] 远程拷贝
来源：http://hz.guannengcc.top/gtwrxgwkji.html

scp file user@host:/path/
来源：http://hz.sysykeji.top/gtljhcbrue.html

[R57] 远程执行命令
来源：http://hz.zhongyouzk.top/gtxzaidcwe.html

ssh user@host 'uptime'
来源：http://hz.pengpengdd.cyou/gtyhlrzdwo.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtkwungjne.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxuanxn.top/gtepeqbtsv.html

[R59] 发 POST JSON
来源：http://hz.zycfv.cn/gtwpentngh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hysaishi.cn/gtdynciflg.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258888.top/gtqgeedzrp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtknuwnbct.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtcusoytgz.html

df -h;  du -sh *
来源：http://hz.guowangkeji.top/gtlcepeaea.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gtvvqwtcoa.html

du -ah . | sort -rh | head -10
来源：http://hz.yangfankeji.com/gtptjkbxqz.html

[R63] 内存与进程
来源：http://hz.jyoumei.cn/gtpgizuwwx.html

free -h;  ps aux | grep nginx
来源：http://hz.xuanzx.com/gtyyuevsyw.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtkhztlmih.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtvmunuqbm.html

[R65] 查看端口占用
来源：http://hz.guannengcc.top/gtjekrikxr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtymgouzjr.html

[R66] 定时任务
来源：http://hz.yongpay.top/gtctnyrdna.html

crontab -e;  crontab -l
来源：http://hz.ivvv.top/gtsskfwqdp.html

[R67] 生成随机十六进制串
来源：http://hz.shangyingyoupin.top/gtehxmtaxr.html

openssl rand -hex 16
来源：http://hz.gaohongyu789.top/gtplnnniop.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtikqppciu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.andypj.xyz/gtwbfichch.html

[R69] 生成随机密码
来源：http://hz.cashguo.top/gtzgjphvos.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhiwuduotai.top/gtamgvtpqk.html

[R70] 时间戳与互转
来源：http://hz.tanke756.top/gtwdvfcqbj.html

date +%s;  date -d @1700000000
来源：http://hz.shuidangran.top/gtbxkhvnhc.html

[R71] 日期格式化
来源：http://hz.xinyue.icu/gtxwjwgynb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangtech.top/gtenbudzmg.html

[R72] 等待端口就绪
来源：http://hz.zdqjudy.top/gtlhipsnjs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ppjwa.cn/gtuvvtpubi.html

[R73] 分割大日志
来源：http://hz.zhongyouzk.top/gtuoufgckr.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtynrlgoor.html

[R74] 批量重命名
来源：http://hz.pycfn.com/gtevxmrjla.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sxryk.cn/gtiizjuaxx.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtptuvmjau.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gtstkbkkmw.html

[R76] 使用临时文件
来源：http://hz.yanxiufei.cn/gtwuhhagzg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtpblqldfq.html

[R77] 读取用户输入
来源：http://hz.jinyuanbaomall.cn/gtfotecvka.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gttckeckim.html

[R78] 交互式菜单
来源：http://hz.yj20258.top/gthjosmszu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinyuanbaomall.cn/gtfhoghhyz.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtuvupyyey.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtwwoapulq.html

[R80] 查看脚本执行耗时
来源：http://hz.mhx1999.top/gtnkotviii.html

time ./run.sh
来源：http://hz.9152youxi.cn/gtvgazoayz.html

================================================================================
来源：http://hz.hammf.cn/gtlsprbmrk.html

S. C / C++ 专题
来源：http://hz.daria6918.cn/gtdsjgcbfo.html

================================================================================
来源：http://hz.yonumen.top/gtehbeaccz.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gtplvnjpfl.html

#include <stdio.h>
来源：http://hz.yj202588.top/gttfcwmnve.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xuetiantiany.cn/gttuwwxwmt.html

[S02] C：变量与格式化输出
来源：http://hz.bjfxy.top/gtrqtuzoln.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtuigsarqi.html

[S03] C：读入整数
来源：http://hz.yj20258888.top/gtuujfozxz.html

int x; scanf("%d", &x);
来源：http://hz.xziqi.cn/gtsxjcehuk.html

[S04] C：字符串复制
来源：http://hz.zhoulong.xyz/gtkocslzjy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtmbwfrkyn.html

[S05] C：字符串长度
来源：http://hz.chenzaomai.com/gteutlbtnn.html

strlen(s)
来源：http://hz.ivvv.top/gtugbolmgc.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gtxkglyklu.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gtdelshxtk.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gtesnuqjwy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtmgyzmhal.html

[S08] C：动态内存分配与释放
来源：http://hz.guannengcc.top/gtfoibfljw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangkeji.top/gtxesnfymc.html

[S09] C：结构体定义与初始化
来源：http://hz.meibo888.top/gtgnhhrvof.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yanxiufei.cn/gtqincbhwa.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtbxxvrrip.html

int *p = &a;  *p = 5;
来源：http://hz.zhijiandao.cn/gtihbvagzq.html

[S11] C：逐行读文件
来源：http://hz.0kj1m.cn/gtvlpbzarx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.birdmap.top/gtfovphgsl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gtpoyyjsqc.html

fclose(f);
来源：http://hz.c1oappe.top/gtkrleagqv.html

[S12] C：写文件
来源：http://hz.hongshengwenyu.top/gtbzjdbkmv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gttaegwadn.html

[S13] C：宏定义
来源：http://hz.xuanzx.com/gttjvejbot.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gtnxpbjhps.html

[S14] C：枚举
来源：http://hz.shangyingyoupin.top/gteynryjof.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtxphzxphw.html

[S15] C：类型转换
来源：http://hz.smart0.xyz/gtasfwgrqu.html

(double) a / b
来源：http://hz.zhoulong.xyz/gthwpcoone.html

[S16] C：位操作置位
来源：http://hz.hywenlv.cn/gtwatogfce.html

x |= (1 << 3);
来源：http://hz.hywenlv.cn/gtqahgoatv.html

[S17] C：安全拼接字符串
来源：http://hz.hnqzz.top/gtmuloirnw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gttriwxxqz.html

[S18] C：命令行参数
来源：http://hz.ydjk.org.cn/gtkwzghkvm.html

int main(int argc, char **argv)
来源：http://hz.ehwqpu.com/gtxmrjcrsd.html

[S19] C：快速排序
来源：http://hz.smart0.xyz/gtphlbdjra.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtzkukgxcg.html

[S20] C：二分查找
来源：http://hz.tanke756.top/gthnbwrvdl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtjgneotlj.html

[S21] C：字符类别判断
来源：http://hz.aibaodan.cn/gtsjmlwpgp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.svipenyu.cn/gtemsuqmzy.html

[S22] C：字符串转数字
来源：http://hz.zycfv.cn/gtxbrlfzyd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtizceanjg.html

[S23] C：随机数
来源：http://hz.aibaodan.cn/gtoqxmbpuk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinghuilouyu.cn/gtxwyeakvh.html

[S24] C：获取本地时间
来源：http://hz.cheryme.top/gtpurpavhn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daria6918.cn/gtsmkvktxl.html

[S25] C：内存拷贝
来源：http://hz.jinyuanbaomall.cn/gtelighduj.html

memcpy(dst, src, n);
来源：http://hz.yvedp.cn/gtuagivxii.html

[S26] C：内存清零
来源：http://hz.aibaodan.cn/gtvuxuiryg.html

memset(a, 0, sizeof a);
来源：http://hz.andypj.xyz/gtomsdpyoe.html

[S27] C：定义常量
来源：http://hz.sxryk.cn/gtjkmorckk.html

const double PI = 3.14159;
来源：http://hz.xinyue.icu/gtaegyxnhj.html

[S28] C：静态变量
来源：http://hz.guowangkeji.top/gtardxjukh.html

static int counter = 0;
来源：http://hz.guannengcc.top/gtiaxnadzw.html

[S29] C：变参函数
来源：http://hz.xingfuxueyuan.xyz/gtnopyuqlc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daxiang520.top/gtpqzhqmdv.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtkuttfrnr.html

#ifndef X_H
来源：http://hz.quarkkingdee.top/gtqfcongtm.html

#define X_H
来源：http://hz.redwolf501.top/gtwlrouojp.html

#endif
来源：http://hz.smart0.xyz/gtkqdgwyvu.html

[S31] C++：Hello World
来源：http://hz.tanke756.top/gtntwvufsm.html

#include <iostream>
来源：http://hz.316326.xyz/gtfacejsfw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtmnzsrllj.html

[S32] C++：字符串
来源：http://hz.yj20258888.top/gtglgmunnk.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtvzwmqyiq.html

[S33] C++：vector 增删
来源：http://hz.hnxiangtu.top/gteukvwyrm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gaohongyu789.top/gtslxnurye.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtvytdzgdf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ivvv.top/gtxfhzwogt.html

[S35] C++：map
来源：http://hz.daria6918.cn/gtttmhztvz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtswowpwou.html

[S36] C++：unordered_map
来源：http://hz.yueranfly.top/gtcawmsxis.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtuxusaced.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtcgbsewzn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gotoacloud.top/gtgrqtvhxo.html

[S38] C++：排序
来源：http://hz.ybcxt.top/gtszblrrpj.html

std::sort(v.begin(), v.end());
来源：http://hz.ydzc1.top/gtyuezisgk.html

[S39] C++：自定义比较器排序
来源：http://hz.zycfv.cn/gtrpmfryhd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtgcqgjwhv.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gtszsalyhg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtqpphzjsc.html

[S41] C++：类与构造函数
来源：http://hz.nwbrower.top/gtrwoglelp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ybcxt.top/gtukihpalq.html

[S42] C++：继承与虚函数
来源：http://hz.cucudq.cn/gthjpydxyk.html

class B : public Base { public: void f() override {} };
来源：http://hz.yvedp.cn/gtyggpxxzv.html

[S43] C++：智能指针
来源：http://hz.svipenyu.cn/gtykfkkpbi.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258888.top/gtbkmflymv.html

[S44] C++：引用传参
来源：http://hz.ydzc1.top/gtfqscjjzr.html

void inc(int &x) { ++x; }
来源：http://hz.hysaishi.cn/gtmodcqmid.html

[S45] C++：lambda
来源：http://hz.kuanghao11.cn/gtrhhmquct.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtfhenzqpp.html

[S46] C++：函数模板
来源：http://hz.yj202588.top/gtedbofuut.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ybcxt.top/gtwlsffoty.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhaomingkeji.xyz/gtkdiiodbo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.havefunace.top/gtjcllnezm.html

[S48] C++：逐行读文件
来源：http://hz.daria6918.cn/gtpoiufrcv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuetiantiany.cn/gtnmufsdad.html

while (std::getline(in, line)) { }
来源：http://hz.chenlongwang.top/gtveuyprro.html

[S49] C++：写文件
来源：http://hz.nanxinkj.top/gtcyizimle.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gtvqqtzhsz.html

[S50] C++：格式化数字
来源：http://hz.yuanzhike.top/gtnaheknuj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenzaomai.com/gtrltdoxxg.html

[S51] C++：显式类型转换
来源：http://hz.dianchejie.cn/gthbjgddiw.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtxveguius.html

[S52] C++：const 与 noexcept
来源：http://hz.gaohongyu789.top/gtkepjsfdr.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtlzwcomzl.html

[S53] C++：移动语义
来源：http://hz.yvedp.cn/gtheirclee.html

std::vector<int> w = std::move(v);
来源：http://hz.cheryme.top/gtslsengzt.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gtfciorxdz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jianghu66.top/gthetveolz.html

[S55] C++：结构化绑定
来源：http://hz.xinyue.icu/gtdaidneum.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nwbrower.top/gtipmrcdoi.html

[S56] C++：optional
来源：http://hz.yuxming.cn/gtghdzqizg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ehwqpu.com/gtwyceyzwg.html

[S57] C++：编译期常量
来源：http://hz.hysaishi.cn/gtiyncymjd.html

constexpr int N = 10;
来源：http://hz.quarkkingdee.top/gtloqhynkn.html

[S58] C++：命名空间
来源：http://hz.aizwys.cn/gtbtnbdgru.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gtucphmmbr.html

[S59] C++：静态断言
来源：http://hz.daria6918.cn/gtrokhdfey.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhaomingkeji.xyz/gtsdinjgmw.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxuanxn.top/gtugmqlxgq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtwbubweti.html

================================================================================
来源：http://hz.ppjwa.cn/gtndianxln.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtkhtkvvkz.html

================================================================================
来源：http://hz.vqdsnc.cn/gttasjiyua.html

[T01] Kotlin：Hello World
来源：http://hz.smart0.xyz/gtiyepjwuq.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtoxoykrbv.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtgvrrlqgi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jlsjyb.cn/gtuvsndqgl.html

[T03] Kotlin：字符串模板
来源：http://hz.c1oappe.top/gtauhmfuas.html

"值: $b"
来源：http://hz.redwolf501.top/gtndqdnswi.html

[T04] Kotlin：空安全
来源：http://hz.gzhubu.top/gtltywlnze.html

val n: String? = null;  n?.length
来源：http://hz.cqqwz.cn/gtmnyvziyx.html

[T05] Kotlin：when 表达式
来源：http://hz.wangshuangyany.cn/gtpduuzaam.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.vqdsnc.cn/gtelsnisjo.html

[T06] Kotlin：集合映射
来源：http://hz.haohaochexian.top/gtmubfaxiv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ywan-chungtsiang.top/gtrugigzrv.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtkuednlek.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cucudq.cn/gtzfkxdgyt.html

[T08] Kotlin：数据类
来源：http://hz.cashguo.top/gtekwekvrx.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtzehukiai.html

[T09] Kotlin：扩展函数
来源：http://hz.jiagoushi.top/gthuuvdcdp.html

fun String.exclaim() = this + "!"
来源：http://hz.yuanzhike.top/gthpyhuhkr.html

[T10] Kotlin：默认参数
来源：http://hz.pengpengdd.cyou/gtenusyiyb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nanxinkj.top/gtihxvldaq.html

[T11] Kotlin：协程
来源：http://hz.yanxiufei.cn/gtttosaowa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenlongwang.top/gtwcfujvon.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gteudmjkun.html

val (a, b) = Pair(1, 2)
来源：http://hz.sweek.top/gtwtoszqaa.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtsvmlykfq.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gttxhqgnyl.html

[T14] Kotlin：循环
来源：http://hz.daxiang520.top/gtladfocqk.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtuzpbjrzk.html

[T15] Kotlin：接口
来源：http://hz.iojbl.cn/gtmsfeyfct.html

interface Shape { fun area(): Double }
来源：http://hz.jqgfzy.top/gtqgukccfe.html

[T16] Swift：Hello World
来源：http://hz.52xcode.cn/gtjwwhodmw.html

print("Hello")
来源：http://hz.ivvv.top/gtvpncgwrw.html

[T17] Swift：变量与常量
来源：http://hz.yj20258888.top/gtzladbrsw.html

var a = 1;  let b = 2
来源：http://hz.kuanghao11.cn/gtbelrxvfd.html

[T18] Swift：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtenntqnpl.html

"值: \(b)"
来源：http://hz.guannengcc.top/gtzfqjrwun.html

[T19] Swift：可选绑定
来源：http://hz.c1oappe.top/gtykiidavi.html

if let n = opt { print(n) }
来源：http://hz.aizwys.cn/gtgzcndyjr.html

[T20] Swift：数组操作
来源：http://hz.daria6918.cn/gtcqexwiid.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhijiandao.cn/gtthbuqifz.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtgdeyqhlz.html

for x in a { print(x) }
来源：http://hz.aizwys.cn/gtmbzrfpsz.html

[T22] Swift：字典
来源：http://hz.meibo888.top/gtpbzshpbs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.haohaochexian.top/gtfuhgarwa.html

[T23] Swift：函数
来源：http://hz.dashuyun.cn/gtdxdvatje.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.52xcode.cn/gtmyldgcvr.html

[T24] Swift：闭包
来源：http://hz.yuxming.cn/gtfpkpukgd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhongyouzk.top/gtbmrkahff.html

[T25] Swift：结构体
来源：http://hz.fengsongda.top/gtmolosaup.html

struct P { var x: Int }
来源：http://hz.zhoulong.xyz/gtbvfqivmb.html

[T26] Swift：类与重写
来源：http://hz.sxryk.cn/gtbyhurxxp.html

class A: Base { override func f() {} }
来源：http://hz.zhaomingkeji.xyz/gtonmimtcp.html

[T27] Swift：错误处理
来源：http://hz.cashguo.top/gtzwnowujh.html

do { try f() } catch { print(error) }
来源：http://hz.gaohongyu789.top/gtajdrrqje.html

[T28] Swift：枚举
来源：http://hz.haohaochexian.top/gtwuhrejzg.html

enum Color { case red, green }
来源：http://hz.zhiwuduotai.top/gtotjoxuur.html

[T29] Swift：guard 提前返回
来源：http://hz.nanxinkj.top/gtwiriqqlv.html

guard let x = opt else { return }
来源：http://hz.ehwqpu.com/gtkgkkujki.html

[T30] Swift：协议
来源：http://hz.sweek.top/gtfvwniilo.html

protocol Shape { func area() -> Double }
来源：http://hz.c1oappe.top/gtxwkapzwk.html

[T31] Lua：Hello World
来源：http://hz.ehwqpu.com/gtdnxhqqpl.html

print("Hello")
来源：http://hz.pycfn.com/gtxjrcwkqm.html

[T32] Lua：局部变量
来源：http://hz.yj20258888.top/gttwdptwhk.html

local a = 1
来源：http://hz.chenzaomai.com/gtabqcrwgr.html

[T33] Lua：表（数组）
来源：http://hz.zdqjudy.top/gteaqkgutc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xylfe.cn/gtfqicdmcd.html

[T34] Lua：遍历表
来源：http://hz.jqgufenzy.top/gtyttdjxeu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.feifeiyinyue.top/gttmdfurfi.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gtslhxczpz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenzaomai.com/gthnmuavub.html

[T36] Lua：函数
来源：http://hz.birdmap.top/gtvwngcqft.html

function add(a, b) return a + b end
来源：http://hz.xylfe.cn/gtccstptmi.html

[T37] Lua：字符串拼接
来源：http://hz.tian-w.cn/gtiaonltzr.html

"a" .. "b"
来源：http://hz.cqqwz.cn/gtwbxlacer.html

[T38] Lua：条件
来源：http://hz.hywenlv.cn/gtmwvgnhsw.html

if x > 0 then print("正") end
来源：http://hz.sweek.top/gtzklfdusq.html

[T39] Lua：模式匹配
来源：http://hz.tanke756.top/gtefxpbaty.html

string.find(s, "%d+")
来源：http://hz.kuanghao11.cn/gtufxhbwkd.html

[T40] Lua：元表
来源：http://hz.yanxiufei.cn/gtghqcjfkk.html

setmetatable({}, { __index = base })
来源：http://hz.jinghuilouyu.cn/gtixsbynri.html

[T41] Perl：Hello World
来源：http://hz.shuidangran.top/gtnacqtdpq.html

print "Hello\n";
来源：http://hz.52xcode.cn/gtogqqkkqx.html

[T42] Perl：变量类型
来源：http://hz.yueranfly.top/gtkehfjtik.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.9152youxi.cn/gtfdpfhkpv.html

[T43] Perl：字符串插值
来源：http://hz.jqgufenzy.top/gtbxikbvbh.html

"值: $a"
来源：http://hz.hfpthk.cn/gtsslivzyp.html

[T44] Perl：条件
来源：http://hz.xinyue.icu/gtvdpbwmds.html

if ($a > 0) { print "正"; }
来源：http://hz.hywenlv.cn/gtwwhadqvh.html

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gtdcvnqcka.html

for my $x (@arr) { print $x; }
来源：http://hz.fengsongda.top/gttcxsxxmu.html

[T46] Perl：哈希操作
来源：http://hz.shuidangran.top/gtmjfsgstt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ybcxt.top/gtouxphevr.html

[T47] Perl：正则捕获
来源：http://hz.yj202588.top/gtjyvxydli.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daria6918.cn/gtftklzmqs.html

[T48] Perl：正则替换
来源：http://hz.shuidangran.top/gtconifpyw.html

$s =~ s/old/new/g;
来源：http://hz.tanke756.top/gtfneoljif.html

[T49] Perl：函数
来源：http://hz.tian-w.cn/gtnmfoyatn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxinkj.top/gtyafqtfeq.html

[T50] Perl：逐行读文件
来源：http://hz.hywenlv.cn/gtzfhafmdl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.pengpengdd.cyou/gtpuksiwit.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jiagoushi.top/gtxghjojlf.html

[T51] Scala：Hello World
来源：http://hz.shzxlz.cn/gtagtmvqva.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtfugopvqz.html

[T52] Scala：变量
来源：http://hz.yj20258888.top/gtfpfszmso.html


<!-- 参考信息 -->