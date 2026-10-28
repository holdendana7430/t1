代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydzc1.top/gtmdpqovdx.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtmtxaqjxl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yanxiufei.cn/gttxkpayaw.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gturaatxxo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtglfkfvup.html

[R52] 统计行数
来源：http://hz.yj20258.top/gtntqfyymg.html

wc -l a.txt
来源：http://hz.yuanzhike.top/gtjucavugj.html

[R53] 查看文件头与实时尾
来源：http://hz.wangshuangyany.cn/gtjsbmpzoy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhoulong.xyz/gtieykgtvs.html

[R54] 比较两个文件
来源：http://hz.jinghuilouyu.cn/gthivcmapx.html

diff a.txt b.txt
来源：http://hz.hfpthk.cn/gtxcybxwcy.html

[R55] 压缩与解压
来源：http://hz.shzxlz.cn/gthmybynuc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cqqwz.cn/gtdhvalpnu.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gteiaehpjr.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtumjjllib.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtpgcjrrrx.html

ssh user@host 'uptime'
来源：http://hz.xinyue.icu/gtscvwgsuq.html

[R58] 下载文件
来源：http://hz.mhx1999.top/gthffisylc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hfpthk.cn/gtipfutvqp.html

[R59] 发 POST JSON
来源：http://hz.hammf.cn/gtwxouoife.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ivvv.top/gtvwpufvff.html

[R60] 只看 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtjbuzhhtd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtwhmzbvuq.html

[R61] 磁盘占用
来源：http://hz.dashuyun.cn/gtxbzughjr.html

df -h;  du -sh *
来源：http://hz.hfpthk.cn/gteawbwtqc.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gtakmspptm.html

du -ah . | sort -rh | head -10
来源：http://hz.ydzc1.top/gtqsjlnnmk.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtqvmxnzeb.html

free -h;  ps aux | grep nginx
来源：http://hz.xinyue.icu/gtcawybjyq.html

[R64] 结束进程
来源：http://hz.ydzc1.top/gtwsosyrkz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtvimpklvf.html

[R65] 查看端口占用
来源：http://hz.zhaomingkeji.xyz/gtamuddfeo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jyoumei.cn/gtpbhujvvq.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gtajqhhrql.html

crontab -e;  crontab -l
来源：http://hz.yuanzhike.top/gtwyvejqkc.html

[R67] 生成随机十六进制串
来源：http://hz.andypj.xyz/gtairvccly.html

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtbdeqzrkh.html

[R68] 计算文件校验值
来源：http://hz.zhixingplan.top/gtbjwswtvm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtxumwqvlx.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtsdhxkfqo.html

head -c 16 /dev/urandom | base64
来源：http://hz.ivvv.top/gtprlqbncl.html

[R70] 时间戳与互转
来源：http://hz.shzxlz.cn/gtxhjwrask.html

date +%s;  date -d @1700000000
来源：http://hz.shuidangran.top/gteekywfcz.html

[R71] 日期格式化
来源：http://hz.sxryk.cn/gtwztjkacq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ywan-chungtsiang.top/gtfbuxhulw.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtxzribdus.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtfsrrjvmx.html

[R73] 分割大日志
来源：http://hz.sxryk.cn/gtlfxvzjmf.html

split -l 1000 big.log part_
来源：http://hz.quarkkingdee.top/gtvxiuwecz.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtjhmdsfxk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hysaishi.cn/gtvyylfejs.html

[R75] 导出环境变量
来源：http://hz.kuanghao11.cn/gtwurnnuoh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gtgqztkzka.html

[R76] 使用临时文件
来源：http://hz.hnxiangtu.top/gtxwmwjrtq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtgbywdata.html

[R77] 读取用户输入
来源：http://hz.zhengqikj.top/gtmfwdodie.html

read -rp "请输入: " ans
来源：http://hz.cdnleiting.top/gtwjffwqbs.html

[R78] 交互式菜单
来源：http://hz.nanxinkj.top/gtngyifsha.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sysykeji.top/gtbexfmceu.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtesnuxhhs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtzrlzsltt.html

[R80] 查看脚本执行耗时
来源：http://hz.sysykeji.top/gtqznqxdrj.html

time ./run.sh
来源：http://hz.yvedp.cn/gtctqnqcrc.html

================================================================================
来源：http://hz.pycfn.com/gtpihvkzwl.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtsicbtvvx.html

================================================================================
来源：http://hz.tanke756.top/gtrdxnpcho.html

[S01] C：Hello World
来源：http://hz.sxryk.cn/gtxvyaypbo.html

#include <stdio.h>
来源：http://hz.shanyushiyangtech.top/gtnwvzebhj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtvhkchxnf.html

[S02] C：变量与格式化输出
来源：http://hz.c1oappe.top/gtteignpvj.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhiwuduotai.top/gtvjkajgcu.html

[S03] C：读入整数
来源：http://hz.hongshengwenyu.top/gtxgtzudej.html

int x; scanf("%d", &x);
来源：http://hz.redwolf501.top/gtnjygqaog.html

[S04] C：字符串复制
来源：http://hz.zdqjudy.top/gtvpwzcsph.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gthjlfxivq.html

[S05] C：字符串长度
来源：http://hz.jianghu66.top/gtcrkfgzqg.html

strlen(s)
来源：http://hz.gogol.net.cn/gtomqduedm.html

[S06] C：字符串比较
来源：http://hz.redwolf501.top/gtbzkvwfux.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gtqsyzyoen.html

[S07] C：数组遍历求和
来源：http://hz.jlsjyb.cn/gtddgbsgez.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fzhhl.top/gtovgxrvsc.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258.top/gtpwyzrycn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gthfxoqjuw.html

[S09] C：结构体定义与初始化
来源：http://hz.jiagoushi.top/gttglvvdwd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhiwuduotai.top/gtebdamzhg.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtdjhqktlw.html

int *p = &a;  *p = 5;
来源：http://hz.yvedp.cn/gtjrxcqnuk.html

[S11] C：逐行读文件
来源：http://hz.yonumen.top/gtnyiasief.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.feifeiyinyue.top/gtuydsddfk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.c1oappe.top/gtypllslyk.html

fclose(f);
来源：http://hz.xinyue.icu/gtqqzpsyky.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtiturtjje.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xinyue.icu/gtboakzoyk.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gttpocsxov.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenjidiqi.icu/gtxpwkbjnt.html

[S14] C：枚举
来源：http://hz.smart0.xyz/gtoslptenm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jiagoushi.top/gtxagqivyv.html

[S15] C：类型转换
来源：http://hz.fzhhl.top/gtwippabit.html

(double) a / b
来源：http://hz.ehwqpu.com/gtdthhtpzs.html

[S16] C：位操作置位
来源：http://hz.tian-w.cn/gtakbkdivp.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtzvjlwlgs.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gtsljjawod.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dashuyun.cn/gtjnairbli.html

[S18] C：命令行参数
来源：http://hz.havefunace.top/gtxlhnnttw.html

int main(int argc, char **argv)
来源：http://hz.jyoumei.cn/gtfywgpvsd.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gtpuqbvrne.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtfhpmhowc.html

[S20] C：二分查找
来源：http://hz.cucudq.cn/gtvvzgjlqt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtdawupson.html

[S21] C：字符类别判断
来源：http://hz.zhiwuduotai.top/gtspbvzeuv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangshuangyany.cn/gtvogdlsdg.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtgnuxlmci.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtbgxubbah.html

[S23] C：随机数
来源：http://hz.kuanghao11.cn/gtycqwqjru.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtoolzwhgw.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtmwdgriav.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.snrcjt.cn/gttseltxng.html

[S25] C：内存拷贝
来源：http://hz.52xcode.cn/gtrimrvrsm.html

memcpy(dst, src, n);
来源：http://hz.kuanghao11.cn/gthxmswekp.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gtybdtwcls.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtquevjyyc.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtszauvdjq.html

const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtrdrafayw.html

[S28] C：静态变量
来源：http://hz.xuanzx.com/gtpdumubwr.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtokxhxszf.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtszzgavpu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.c1oappe.top/gtmdrcpypw.html

[S30] C：头文件保护
来源：http://hz.yvedp.cn/gtjcopzxva.html

#ifndef X_H
来源：http://hz.cashguo.top/gtdwqlweju.html

#define X_H
来源：http://hz.yuxming.cn/gtwmhxnilu.html

#endif
来源：http://hz.xinyue.icu/gtovohidyi.html

[S31] C++：Hello World
来源：http://hz.yongpay.top/gtduhclcyd.html

#include <iostream>
来源：http://hz.feifeiyinyue.top/gtspfrcljc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuxming.cn/gtzlopghkq.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gtvuuscviy.html

std::string s = "hi";  s += "!";
来源：http://hz.yangfankeji.com/gtoskqgerx.html

[S33] C++：vector 增删
来源：http://hz.shangyingyoupin.top/gtxqblcfym.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shangyingyoupin.top/gtvqvleehy.html

[S34] C++：遍历 vector
来源：http://hz.cqqwz.cn/gtuwzbbipn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dashuyun.cn/gtagxdfgzf.html

[S35] C++：map
来源：http://hz.fengsongda.top/gtfhzhgicr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtxythhkiv.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtxuhnghid.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtkjgdqpos.html

[S37] C++：set
来源：http://hz.ivvv.top/gtzpodvvyt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtbheqsgft.html

[S38] C++：排序
来源：http://hz.xziqi.cn/gtvkoprxaw.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtkneduuau.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gtmjuqegcb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jyoumei.cn/gtlpbfkcpq.html

[S40] C++：查找元素
来源：http://hz.dashuyun.cn/gtnvbttplk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenlongwang.top/gterspeuqm.html

[S41] C++：类与构造函数
来源：http://hz.gogol.net.cn/gturucwbqq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pycfn.com/gthlegscfz.html

[S42] C++：继承与虚函数
来源：http://hz.ybcxt.top/gtvjrseutk.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gtbkhneqvy.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtdnsnswvu.html

auto p = std::make_unique<int>(5);
来源：http://hz.jiagoushi.top/gtknbmmhvd.html

[S44] C++：引用传参
来源：http://hz.cheryme.top/gtswzxmwcc.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtldinrhan.html

[S45] C++：lambda
来源：http://hz.yuanzhike.top/gtvoisyobb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sweek.top/gtlnbbuqcx.html

[S46] C++：函数模板
来源：http://hz.hnxiangtu.top/gtxecixjsx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuanzhike.top/gtuqdwpryc.html

[S47] C++：结构化绑定遍历
来源：http://hz.guannengcc.top/gttxqyutjj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtidzueegp.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtehwhpipx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.52xcode.cn/gthrfldsxc.html

while (std::getline(in, line)) { }
来源：http://hz.9152youxi.cn/gtsgjrlfsf.html

[S49] C++：写文件
来源：http://hz.andypj.xyz/gtnzfsfxwc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gtckwxnicm.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtrdinxbxy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtdqyvcnab.html

[S51] C++：显式类型转换
来源：http://hz.jlsjyb.cn/gtourlhnrq.html

static_cast<double>(a) / b
来源：http://hz.guowangkeji.top/gtwfjlljgh.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtjrvidsmp.html

int size() const noexcept { return n_; }
来源：http://hz.yangfankeji.com/gtbaacnvgl.html

[S53] C++：移动语义
来源：http://hz.gaohongyu789.top/gteiqhdxsz.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gtixcjxljq.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtjsvorwmj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinghuilouyu.cn/gtiaoflldr.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtfrxfpxni.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shangyingyoupin.top/gtwkcptsue.html

[S56] C++：optional
来源：http://hz.xuetiantiany.cn/gtpvbwazji.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fengsongda.top/gtvwqmjzro.html

[S57] C++：编译期常量
来源：http://hz.jinqigufen.top/gtvehecjfd.html

constexpr int N = 10;
来源：http://hz.nanxinkj.top/gtkmxawzwf.html

[S58] C++：命名空间
来源：http://hz.nwbrower.top/gtpmbndmsw.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinghuilouyu.cn/gtnwjdfnqx.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gtilqglqpb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuetiantiany.cn/gtjoihclqw.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtacxmaznz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhengqikj.top/gtyswyvoiv.html

================================================================================
来源：http://hz.nwbrower.top/gtykmlqgva.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtmmqbbmpq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzhzpuiiq.html

[T01] Kotlin：Hello World
来源：http://hz.dashuyun.cn/gtcctswvsi.html

println("Hello")
来源：http://hz.chenlongwang.top/gtupvsjnhg.html

[T02] Kotlin：变量
来源：http://hz.sweek.top/gtbomftcbc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtzqdqktle.html

[T03] Kotlin：字符串模板
来源：http://hz.c1oappe.top/gtzocnorxe.html

"值: $b"
来源：http://hz.redwolf501.top/gtrzqbugek.html

[T04] Kotlin：空安全
来源：http://hz.jiagoushi.top/gtorokxpvy.html

val n: String? = null;  n?.length
来源：http://hz.quarkkingdee.top/gtupzodjei.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gtfazmwegc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xuetiantiany.cn/gtrxlexgud.html

[T06] Kotlin：集合映射
来源：http://hz.fzhhl.top/gtomdgkhoo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhaomingkeji.xyz/gtcbbzkisg.html

[T07] Kotlin：集合过滤
来源：http://hz.jlsjyb.cn/gtmawfhdwn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yanxiufei.cn/gtdxezjkyc.html

[T08] Kotlin：数据类
来源：http://hz.jinghuilouyu.cn/gtopwzkvqy.html

data class User(val name: String, val age: Int)
来源：http://hz.sufxvd.cn/gtmvpirodq.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtkohbohfj.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gtfgshekfw.html

[T10] Kotlin：默认参数
来源：http://hz.zhixingplan.top/gtxhjtrwku.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nanxuanxn.top/gtexcvtipa.html

[T11] Kotlin：协程
来源：http://hz.dashuyun.cn/gtrwrffjhe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xinyue.icu/gteengmpcu.html

[T12] Kotlin：解构声明
来源：http://hz.dashuyun.cn/gtrgabymvg.html

val (a, b) = Pair(1, 2)
来源：http://hz.pycfn.com/gtdtnuulvt.html

[T13] Kotlin：只读 Map
来源：http://hz.yj202588.top/gtqcpfyaxj.html

val m = mapOf("a" to 1)
来源：http://hz.cqqwz.cn/gtvrmvgbpg.html

[T14] Kotlin：循环
来源：http://hz.wangshuangyany.cn/gtmdusozky.html

for (i in 1..10) println(i)
来源：http://hz.jqgufenzy.top/gtlczscsfn.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtmurpdrhy.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gtjxthwlqg.html

[T16] Swift：Hello World
来源：http://hz.9152youxi.cn/gttarrucxl.html

print("Hello")
来源：http://hz.zycfv.cn/gtiygggmvb.html

[T17] Swift：变量与常量
来源：http://hz.cashguo.top/gtdvihenaf.html

var a = 1;  let b = 2
来源：http://hz.yuanzhike.top/gtaxfdwxwz.html

[T18] Swift：字符串插值
来源：http://hz.gogol.net.cn/gtwmkswmuc.html

"值: \(b)"
来源：http://hz.daxiang520.top/gtvsdrvnlm.html

[T19] Swift：可选绑定
来源：http://hz.yj20258.top/gtmqbwhdnu.html

if let n = opt { print(n) }
来源：http://hz.cheryme.top/gtodsjsvjz.html

[T20] Swift：数组操作
来源：http://hz.wangdashe.top/gtfpjsscfm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sxryk.cn/gthlcscwvs.html

[T21] Swift：遍历
来源：http://hz.jinqigfzy.top/gtotivfedh.html

for x in a { print(x) }
来源：http://hz.vqdsnc.cn/gtvulyndid.html

[T22] Swift：字典
来源：http://hz.daria6918.cn/gtcngczzrj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gtxuyykcqh.html

[T23] Swift：函数
来源：http://hz.xingfuxueyuan.xyz/gtdtommnxr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtjacqqwaw.html

[T24] Swift：闭包
来源：http://hz.svipenyu.cn/gtkrdilvoh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ehwqpu.com/gtkulbirmt.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtthihomoj.html

struct P { var x: Int }
来源：http://hz.yj202588.top/gtxsahyiat.html

[T26] Swift：类与重写
来源：http://hz.sysykeji.top/gtppziamvn.html

class A: Base { override func f() {} }
来源：http://hz.cucudq.cn/gtcurhvyuf.html

[T27] Swift：错误处理
来源：http://hz.mhx1999.top/gtyubequma.html

do { try f() } catch { print(error) }
来源：http://hz.redwolf501.top/gtmnrlzkzl.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtbhmdpccf.html

enum Color { case red, green }
来源：http://hz.aizwys.cn/gtmlekexva.html

[T29] Swift：guard 提前返回
来源：http://hz.xziqi.cn/gtgiiqcawu.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gtizfojjex.html

[T30] Swift：协议
来源：http://hz.iojbl.cn/gtdhvvivyr.html

protocol Shape { func area() -> Double }
来源：http://hz.sysykeji.top/gtkdntvpxh.html

[T31] Lua：Hello World
来源：http://hz.sweek.top/gtlnwuyhbt.html

print("Hello")
来源：http://hz.cucudq.cn/gtbdlijrdb.html

[T32] Lua：局部变量
来源：http://hz.andypj.xyz/gtuewwxlpp.html

local a = 1
来源：http://hz.hysaishi.cn/gtdptmhobq.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtpjmqllgq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hongshengwenyu.top/gtmuqlidbw.html

[T34] Lua：遍历表
来源：http://hz.chenjidiqi.icu/gtjvddjzmv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nwbrower.top/gtqqtuckbg.html

[T35] Lua：字典表
来源：http://hz.chenlongwang.top/gtezdiyuaa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhongyouzk.top/gtpjwnnzml.html

[T36] Lua：函数
来源：http://hz.xuetiantiany.cn/gtrmteilsv.html

function add(a, b) return a + b end
来源：http://hz.iojbl.cn/gtiqgchgdj.html

[T37] Lua：字符串拼接
来源：http://hz.jqgufenzy.top/gtmuyfokaz.html

"a" .. "b"
来源：http://hz.zdqjudy.top/gtjxwvamce.html

[T38] Lua：条件
来源：http://hz.guowangkeji.top/gtmvriixii.html

if x > 0 then print("正") end
来源：http://hz.dianchejie.cn/gtuzfkwgqp.html

[T39] Lua：模式匹配
来源：http://hz.shangyingyoupin.top/gtagtmvbek.html

string.find(s, "%d+")
来源：http://hz.iojbl.cn/gtapuacpqk.html

[T40] Lua：元表
来源：http://hz.shanyushiyangkeji.top/gtvhbtxsaw.html

setmetatable({}, { __index = base })
来源：http://hz.quarkkingdee.top/gtjhbydjzq.html

[T41] Perl：Hello World
来源：http://hz.yuanzhike.top/gtbroetawi.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtfsybqwlc.html

[T42] Perl：变量类型
来源：http://hz.gaohongyu789.top/gtwezjkqyx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ivvv.top/gtrloiawyx.html

[T43] Perl：字符串插值
来源：http://hz.chenlongwang.top/gtllitepih.html

"值: $a"
来源：http://hz.yj20258888.top/gttpyssmjd.html

[T44] Perl：条件
来源：http://hz.shanyushiyangkeji.top/gtvxetzjxv.html

if ($a > 0) { print "正"; }
来源：http://hz.yj20258888.top/gtfomknhdd.html

[T45] Perl：数组遍历
来源：http://hz.fzhhl.top/gtlgimexys.html

for my $x (@arr) { print $x; }
来源：http://hz.quarkkingdee.top/gtlloprvds.html

[T46] Perl：哈希操作
来源：http://hz.fengsongda.top/gtvdyrhisg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.nwbrower.top/gtiwzpqhso.html

[T47] Perl：正则捕获
来源：http://hz.jianghu66.top/gtflymxcbl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wangshuangyany.cn/gtwvewmrfl.html

[T48] Perl：正则替换
来源：http://hz.ywan-chungtsiang.top/gtjddfakye.html

$s =~ s/old/new/g;
来源：http://hz.xuetiantiany.cn/gtdurchqvv.html

[T49] Perl：函数
来源：http://hz.yueranfly.top/gtupaosjhk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yangfankeji.com/gthzaxkvqj.html

[T50] Perl：逐行读文件
来源：http://hz.sysykeji.top/gtwhmbtnqq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.birdmap.top/gtxnafjiri.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yueranfly.top/gtlzothuwt.html

[T51] Scala：Hello World
来源：http://hz.sweek.top/gtpagvsuab.html

println("Hello")
来源：http://hz.xinyue.icu/gtntaebkkk.html

[T52] Scala：变量
来源：http://hz.yuanzhike.top/gtsqbpjwaj.html


<!-- 参考信息 -->