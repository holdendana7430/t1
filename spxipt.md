代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.guannengcc.top/gtwzvhxhth.html

[R46] 递归替换文件内容
来源：http://hz.pycfn.com/gtmfifikjm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gogol.net.cn/gtoejinthx.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gthkdeidwb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pycfn.com/gtermktkjx.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gtlrxlkowk.html

awk '{print $1, $3}' a.txt
来源：http://hz.shangyingyoupin.top/gtqzzuqwsp.html

[R49] awk 带条件
来源：http://hz.tian-w.cn/gtisrsibnz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yueranfly.top/gtepsfhiaj.html

[R50] awk 求和
来源：http://hz.guowangkeji.top/gtiwskcwfs.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtykxfqznx.html

[R51] 排序去重取前几
来源：http://hz.shanyushiyangtech.top/gtlaqtvpho.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sufxvd.cn/gtrijkamsf.html

[R52] 统计行数
来源：http://hz.wangdashe.top/gtofruslrs.html

wc -l a.txt
来源：http://hz.zhaomingkeji.xyz/gthagrdiip.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtjswfmdwl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtmucfmbyz.html

[R54] 比较两个文件
来源：http://hz.cheryme.top/gtijatskcr.html

diff a.txt b.txt
来源：http://hz.hysaishi.cn/gtlhbhjcya.html

[R55] 压缩与解压
来源：http://hz.52xcode.cn/gtptkiaisn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenjidiqi.icu/gtmkfsrvlh.html

[R56] 远程拷贝
来源：http://hz.gaohongyu789.top/gtsdyabvmy.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gtokbrxegz.html

[R57] 远程执行命令
来源：http://hz.fengsongda.top/gtjsqpcjct.html

ssh user@host 'uptime'
来源：http://hz.yj20258.top/gttdpmwmzy.html

[R58] 下载文件
来源：http://hz.yuanzhike.top/gtjcugzmhg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtlwwfluui.html

[R59] 发 POST JSON
来源：http://hz.pengpengdd.cyou/gtfhinfvwy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aizwys.cn/gtxrphvbwa.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtfllixzsw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tian-w.cn/gtkbduozmm.html

[R61] 磁盘占用
来源：http://hz.0kj1m.cn/gtyexpracl.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtezyklbgj.html

[R62] 找最占空间的文件
来源：http://hz.zhongyouzk.top/gtqrgnznbl.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gtmhurzouv.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtwbadkwcb.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtcvtotude.html

[R64] 结束进程
来源：http://hz.ivvv.top/gtddzkzgsd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinyuanbaomall.cn/gtmmujpslc.html

[R65] 查看端口占用
来源：http://hz.svipenyu.cn/gtgjkxwnbu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.svipenyu.cn/gttplzxdbd.html

[R66] 定时任务
来源：http://hz.pengpengdd.cyou/gtjpqdubra.html

crontab -e;  crontab -l
来源：http://hz.jqgfzy.top/gtzmxablds.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtktiypzmt.html

openssl rand -hex 16
来源：http://hz.zhaomingkeji.xyz/gtgqiyjhme.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtgdgfamud.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hfpthk.cn/gtmwsrqvia.html

[R69] 生成随机密码
来源：http://hz.jinqigfzy.top/gtbzpqqaut.html

head -c 16 /dev/urandom | base64
来源：http://hz.cqqwz.cn/gtyhcjezfu.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtxwtfigwb.html

date +%s;  date -d @1700000000
来源：http://hz.feifeiyinyue.top/gtuqgpcygg.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtakwyecgy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daxiang520.top/gtqemqjytk.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtecylvwfz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gttttwwtds.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gtvwyrqvto.html

split -l 1000 big.log part_
来源：http://hz.nwbrower.top/gtvbupawwd.html

[R74] 批量重命名
来源：http://hz.52xcode.cn/gtjxojjyrx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtqroxvhlx.html

[R75] 导出环境变量
来源：http://hz.daxiang520.top/gtywbgallu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhaomingkeji.xyz/gtlumnnegk.html

[R76] 使用临时文件
来源：http://hz.zhiwuduotai.top/gtewjcdnob.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtmqsqjavz.html

[R77] 读取用户输入
来源：http://hz.cheryme.top/gtpeutwmqr.html

read -rp "请输入: " ans
来源：http://hz.jinqigfzy.top/gtgcapaoxo.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtibqphzrv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhijiandao.cn/gtqkkifoil.html

[R79] 解析命令行选项
来源：http://hz.snrcjt.cn/gthyggwzfs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtfctuyipn.html

[R80] 查看脚本执行耗时
来源：http://hz.yangfankeji.com/gtrxaxaakx.html

time ./run.sh
来源：http://hz.chenjidiqi.icu/gtagdvafrp.html

================================================================================
来源：http://hz.ivvv.top/gtwoionvdy.html

S. C / C++ 专题
来源：http://hz.ppjwa.cn/gtutjvgdgu.html

================================================================================
来源：http://hz.tianlin.xyz/gtqujgjwti.html

[S01] C：Hello World
来源：http://hz.52xcode.cn/gtgthomlzs.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtxhdnnixv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dianchejie.cn/gtqtqskjgo.html

[S02] C：变量与格式化输出
来源：http://hz.shzxlz.cn/gtnuqujflt.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnxiangtu.top/gtorbvkdfb.html

[S03] C：读入整数
来源：http://hz.xingfuxueyuan.xyz/gtdpdmvqgo.html

int x; scanf("%d", &x);
来源：http://hz.bjfxy.top/gtowhdtova.html

[S04] C：字符串复制
来源：http://hz.yuanzhike.top/gtsmorenkj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenjidiqi.icu/gtdmjarmns.html

[S05] C：字符串长度
来源：http://hz.bjfxy.top/gtelufdcgz.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtyyddqhtt.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gtujxycbmw.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtdbrouqlv.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtjoakueeo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtpqxdeyjr.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtsfkhxwxp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gtzenakomq.html

[S09] C：结构体定义与初始化
来源：http://hz.andypj.xyz/gtqsjplkgg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgufenzy.top/gtscteaqkb.html

[S10] C：指针与解引用
来源：http://hz.ybcxt.top/gtqthsujum.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtxaauozdd.html

[S11] C：逐行读文件
来源：http://hz.52xcode.cn/gtysvfwafs.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtqdubghch.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hywenlv.cn/gtfscxgscr.html

fclose(f);
来源：http://hz.xylfe.cn/gtqnncusfs.html

[S12] C：写文件
来源：http://hz.hysaishi.cn/gtvzrefbhu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nwbrower.top/gtzqipnozh.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtsvkqxxlt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.bjfxy.top/gtffjobano.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtpyxcdcdc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yonumen.top/gtjmcrmlob.html

[S15] C：类型转换
来源：http://hz.nwbrower.top/gtbpvsdbps.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtcvsmfjrf.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gtfajohpju.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gtkruytbfl.html

[S17] C：安全拼接字符串
来源：http://hz.pengpengdd.cyou/gtwsmodgtv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtcyjlvrvg.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gtpsjtrpty.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtnaqjzgok.html

[S19] C：快速排序
来源：http://hz.cashguo.top/gtgctfusnv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtlpilezxn.html

[S20] C：二分查找
来源：http://hz.sufxvd.cn/gtcyrgcrmz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gtjrcifbfy.html

[S21] C：字符类别判断
来源：http://hz.ydzc1.top/gtiwxprdrb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtaoyyccuu.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtzjtbbvyx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtwuakardu.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtzlviqbnd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigfzy.top/gtiluibasn.html

[S24] C：获取本地时间
来源：http://hz.havefunace.top/gtupgmhwgr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigufen.top/gtezcedfek.html

[S25] C：内存拷贝
来源：http://hz.zhaomingkeji.xyz/gtpibartun.html

memcpy(dst, src, n);
来源：http://hz.cqqwz.cn/gtdecprlap.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gtpnomzhcy.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtjufuqgyk.html

[S27] C：定义常量
来源：http://hz.chenjidiqi.icu/gtwipldppd.html

const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtoqpcfhei.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtwyyevzbs.html

static int counter = 0;
来源：http://hz.andypj.xyz/gtajawvdhv.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtvlaqzoyg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daxiang520.top/gtgkvbcrvu.html

[S30] C：头文件保护
来源：http://hz.mhx1999.top/gtrdkhocjq.html

#ifndef X_H
来源：http://hz.redwolf501.top/gteljbiefj.html

#define X_H
来源：http://hz.cashguo.top/gtticiqgly.html

#endif
来源：http://hz.cucudq.cn/gtirxgfgtc.html

[S31] C++：Hello World
来源：http://hz.yonumen.top/gtzlkudnty.html

#include <iostream>
来源：http://hz.andypj.xyz/gtsgsfctfc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gtvctscjzk.html

[S32] C++：字符串
来源：http://hz.andypj.xyz/gtgwerzwrs.html

std::string s = "hi";  s += "!";
来源：http://hz.ydjk.org.cn/gttncjnryg.html

[S33] C++：vector 增删
来源：http://hz.hywenlv.cn/gthhjcboyp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtirwysetu.html

[S34] C++：遍历 vector
来源：http://hz.birdmap.top/gtkworncmq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtdlqkluqt.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtloxagzpw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtnmwscuqd.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtcpfzmdzx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtbtzqcabg.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtudragyzg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shuidangran.top/gtggfmyrdz.html

[S38] C++：排序
来源：http://hz.hnqzz.top/gtgabznual.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtedodshqr.html

[S39] C++：自定义比较器排序
来源：http://hz.feifeiyinyue.top/gtdocygtvi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinyuanbaomall.cn/gtbvyyzkfe.html

[S40] C++：查找元素
来源：http://hz.jianghu66.top/gtviwbunoq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xylfe.cn/gtextlhzeo.html

[S41] C++：类与构造函数
来源：http://hz.hnqzz.top/gtjoytrzhd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtetssfscw.html

[S42] C++：继承与虚函数
来源：http://hz.zhiwuduotai.top/gtslmcpxsf.html

class B : public Base { public: void f() override {} };
来源：http://hz.gaohongyu789.top/gthgmusrdc.html

[S43] C++：智能指针
来源：http://hz.tianlin.xyz/gttyrszhtl.html

auto p = std::make_unique<int>(5);
来源：http://hz.hfpthk.cn/gtbkwndljt.html

[S44] C++：引用传参
来源：http://hz.gogol.net.cn/gtcstgtcfj.html

void inc(int &x) { ++x; }
来源：http://hz.havefunace.top/gtezhgqgsi.html

[S45] C++：lambda
来源：http://hz.tian-w.cn/gtpxfdqhpj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigfzy.top/gtpvyghpbo.html

[S46] C++：函数模板
来源：http://hz.jyoumei.cn/gtfyhucvsd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtwfldtpbg.html

[S47] C++：结构化绑定遍历
来源：http://hz.hongshengwenyu.top/gtcjmkpvrj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.kuanghao11.cn/gtibauqwlx.html

[S48] C++：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtxsqmxnfl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtqzchzsex.html

while (std::getline(in, line)) { }
来源：http://hz.jqgfzy.top/gtlpluqffp.html

[S49] C++：写文件
来源：http://hz.nanxinkj.top/gtubjtvqli.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cucudq.cn/gtqxgsqdul.html

[S50] C++：格式化数字
来源：http://hz.yj20258888.top/gthqonyowf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgfzy.top/gtyyzarycm.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtberubwtu.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtlikoyjbc.html

[S52] C++：const 与 noexcept
来源：http://hz.jiagoushi.top/gtyldpwqpr.html

int size() const noexcept { return n_; }
来源：http://hz.tianlin.xyz/gtabczipsj.html

[S53] C++：移动语义
来源：http://hz.snrcjt.cn/gtlksrlxbl.html

std::vector<int> w = std::move(v);
来源：http://hz.jianghu66.top/gtparpdean.html

[S54] C++：异常处理
来源：http://hz.iojbl.cn/gtcgqcbtwx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tian-w.cn/gtuolwtbxi.html

[S55] C++：结构化绑定
来源：http://hz.iojbl.cn/gtvnexfyhr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jiagoushi.top/gtpnvcwyhl.html

[S56] C++：optional
来源：http://hz.yongpay.top/gtrgtcbqzg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jianghu66.top/gtujhkxnjg.html

[S57] C++：编译期常量
来源：http://hz.ehwqpu.com/gttgdqrpyj.html

constexpr int N = 10;
来源：http://hz.c1oappe.top/gtdzrwrdzh.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gttuoossbs.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtnlngkhan.html

[S59] C++：静态断言
来源：http://hz.svipenyu.cn/gtxmzcnqgp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtfebguenx.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtqehvfjkl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtalrjkfwz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttrocqngw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtvmmqclmu.html

================================================================================
来源：http://hz.zhengqikj.top/gtwwkeucth.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gtbbjohaae.html

println("Hello")
来源：http://hz.wangdashe.top/gtiwxenxkb.html

[T02] Kotlin：变量
来源：http://hz.chenlongwang.top/gtjpsswvcd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.quarkkingdee.top/gtlaxdlffk.html

[T03] Kotlin：字符串模板
来源：http://hz.52xcode.cn/gtmqeatwzi.html

"值: $b"
来源：http://hz.cdnleiting.top/gtfataswxy.html

[T04] Kotlin：空安全
来源：http://hz.fengsongda.top/gtwinnpscg.html

val n: String? = null;  n?.length
来源：http://hz.ydjk.org.cn/gttapiuuey.html

[T05] Kotlin：when 表达式
来源：http://hz.sufxvd.cn/gtvkalpnvn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gthikzarue.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gthoeybfbn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtrlkkdvio.html

[T07] Kotlin：集合过滤
来源：http://hz.meibo888.top/gtgiwqgujg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtwarkbyod.html

[T08] Kotlin：数据类
来源：http://hz.zhixingplan.top/gtzjuhotia.html

data class User(val name: String, val age: Int)
来源：http://hz.yj202588.top/gtogqvtamb.html

[T09] Kotlin：扩展函数
来源：http://hz.chenlongwang.top/gtkqjnjrng.html

fun String.exclaim() = this + "!"
来源：http://hz.kuanghao11.cn/gtbfvcehko.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtidmaxgxf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinyuanbaomall.cn/gthocaclcm.html

[T11] Kotlin：协程
来源：http://hz.sufxvd.cn/gtriuiydog.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gtcwyugwxg.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtpyaamhnf.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtfrvnuonb.html

[T13] Kotlin：只读 Map
来源：http://hz.0kj1m.cn/gtxtnzmfac.html

val m = mapOf("a" to 1)
来源：http://hz.wangdashe.top/gtnfojwsup.html

[T14] Kotlin：循环
来源：http://hz.yuanzhike.top/gtbkltgttq.html

for (i in 1..10) println(i)
来源：http://hz.pengpengdd.cyou/gtueiezeqi.html

[T15] Kotlin：接口
来源：http://hz.sxryk.cn/gttorznqua.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtzyhmsnbi.html

[T16] Swift：Hello World
来源：http://hz.zhengqikj.top/gtqcadguwd.html

print("Hello")
来源：http://hz.guannengcc.top/gthxomcovj.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gtwfngabvt.html

var a = 1;  let b = 2
来源：http://hz.yuanzhike.top/gttyyqzvhz.html

[T18] Swift：字符串插值
来源：http://hz.316326.xyz/gtjyglnstl.html

"值: \(b)"
来源：http://hz.mhx1999.top/gtrzycweuv.html

[T19] Swift：可选绑定
来源：http://hz.zhiwuduotai.top/gtsrcdpwhz.html

if let n = opt { print(n) }
来源：http://hz.dashuyun.cn/gtbfbdiday.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gtzogslgwl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtlboilxqg.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gtxvznswum.html

for x in a { print(x) }
来源：http://hz.yonumen.top/gtrnotkkwv.html

[T22] Swift：字典
来源：http://hz.gaohongyu789.top/gtsxiadrod.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gtvfiojigc.html

[T23] Swift：函数
来源：http://hz.tanke756.top/gtflelhoar.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtwsspunki.html

[T24] Swift：闭包
来源：http://hz.chenzaomai.com/gtehmkwmtd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shzxlz.cn/gtagvqcqsc.html

[T25] Swift：结构体
来源：http://hz.cashguo.top/gtzisqxrmo.html

struct P { var x: Int }
来源：http://hz.iojbl.cn/gtqmtrvugy.html

[T26] Swift：类与重写
来源：http://hz.shzxlz.cn/gtxhvuyhkq.html

class A: Base { override func f() {} }
来源：http://hz.aibaodan.cn/gtxwnodrep.html

[T27] Swift：错误处理
来源：http://hz.shangyingyoupin.top/gtvyemgxwq.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gtsqfdvmws.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtprgkbyid.html

enum Color { case red, green }
来源：http://hz.wangshuangyany.cn/gtfwphlsur.html

[T29] Swift：guard 提前返回
来源：http://hz.jlsjyb.cn/gtmxpsnifo.html

guard let x = opt else { return }
来源：http://hz.cdnleiting.top/gtygihiieg.html

[T30] Swift：协议
来源：http://hz.ybcxt.top/gtcimzdvrv.html

protocol Shape { func area() -> Double }
来源：http://hz.iojbl.cn/gtfmpdeodj.html

[T31] Lua：Hello World
来源：http://hz.birdmap.top/gtxyalamhi.html

print("Hello")
来源：http://hz.guannengcc.top/gtdpjgnyro.html

[T32] Lua：局部变量
来源：http://hz.shuidangran.top/gtkfupbmqm.html

local a = 1
来源：http://hz.shanyushiyangkeji.top/gtqmnbpjjf.html

[T33] Lua：表（数组）
来源：http://hz.sufxvd.cn/gtkidqiwpc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cqqwz.cn/gtjfbnmbep.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtwrnaroxe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.316326.xyz/gtwdntuyzm.html

[T35] Lua：字典表
来源：http://hz.aizwys.cn/gtkuyhxrnn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hywenlv.cn/gtuswerxkr.html

[T36] Lua：函数
来源：http://hz.chenzaomai.com/gtxkhjwszf.html

function add(a, b) return a + b end
来源：http://hz.meibo888.top/gtpvhsxldb.html

[T37] Lua：字符串拼接
来源：http://hz.bjfxy.top/gtvuehecez.html

"a" .. "b"
来源：http://hz.nanxuanxn.top/gtnjnomeie.html

[T38] Lua：条件
来源：http://hz.pengpengdd.cyou/gtkptejqyh.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gtiovfrceg.html

[T39] Lua：模式匹配
来源：http://hz.mhx1999.top/gtfwwaixia.html

string.find(s, "%d+")
来源：http://hz.mhx1999.top/gtgclgeuja.html

[T40] Lua：元表
来源：http://hz.nanxuanxn.top/gtnvhnvket.html

setmetatable({}, { __index = base })
来源：http://hz.aizwys.cn/gtalhdqleq.html

[T41] Perl：Hello World
来源：http://hz.smart0.xyz/gtgpnqrtrd.html

print "Hello\n";
来源：http://hz.ppjwa.cn/gtauhocvlz.html

[T42] Perl：变量类型
来源：http://hz.shanyushiyangkeji.top/gtdcxpwxrj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.vqdsnc.cn/gtmpkaylfr.html

[T43] Perl：字符串插值
来源：http://hz.mhx1999.top/gtsvkzabql.html

"值: $a"
来源：http://hz.svipenyu.cn/gtcxhmaadn.html

[T44] Perl：条件
来源：http://hz.yueranfly.top/gtxsobocpu.html

if ($a > 0) { print "正"; }
来源：http://hz.jinqigfzy.top/gtltdupqak.html

[T45] Perl：数组遍历
来源：http://hz.yj20258.top/gtlcjecqyc.html

for my $x (@arr) { print $x; }
来源：http://hz.sweek.top/gtgjrpcdvw.html

[T46] Perl：哈希操作
来源：http://hz.hywenlv.cn/gtomsejxcg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigufen.top/gtgseafnju.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtilrfrqhs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hnqzz.top/gtqdicipnq.html

[T48] Perl：正则替换
来源：http://hz.sweek.top/gtehjxsrvj.html

$s =~ s/old/new/g;
来源：http://hz.pengpengdd.cyou/gtwcuneovh.html


<!-- 参考信息 -->