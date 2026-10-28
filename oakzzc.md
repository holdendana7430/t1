代发 wailian999

find . -name "*.log" -type f
来源：http://hz.zhixingplan.top/gthwsasmxr.html

[R44] 按修改时间查找
来源：http://hz.ywan-chungtsiang.top/gthlmliomx.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gteuxoagyd.html

[R45] 批量删除
来源：http://hz.zycfv.cn/gtalivaxra.html

find . -name "*.tmp" -delete
来源：http://hz.yuanzhike.top/gtowqiduks.html

[R46] 递归替换文件内容
来源：http://hz.gotoacloud.top/gtcjugndph.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.smart0.xyz/gtjkzzwoou.html

[R47] sed 单行替换
来源：http://hz.cashguo.top/gtcizsvyhr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtrqnkqmnc.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtbufojtzj.html

awk '{print $1, $3}' a.txt
来源：http://hz.quarkkingdee.top/gtnyqafads.html

[R49] awk 带条件
来源：http://hz.yuxming.cn/gtpshnseqy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pengpengdd.cyou/gtzzodrumi.html

[R50] awk 求和
来源：http://hz.316326.xyz/gtxoozritc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj202588.top/gthliilitf.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gtlcmsoplj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shangyingyoupin.top/gtbyewxpzo.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gtxrhzcrzh.html

wc -l a.txt
来源：http://hz.quarkkingdee.top/gtzarfwupt.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtrlfwzzzw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhoulong.xyz/gtewqgqaem.html

[R54] 比较两个文件
来源：http://hz.xinyue.icu/gthggmjnwm.html

diff a.txt b.txt
来源：http://hz.hnxiangtu.top/gteqrxwhty.html

[R55] 压缩与解压
来源：http://hz.hongshengwenyu.top/gtcjnqoxhc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tanke756.top/gtoyeueblv.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtnzxspboo.html

scp file user@host:/path/
来源：http://hz.0kj1m.cn/gtbnslkykp.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gtxooxwrdz.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangkeji.top/gtqsfejcgo.html

[R58] 下载文件
来源：http://hz.sweek.top/gtipolgoya.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guowangkeji.top/gtdqwaoons.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtconxrmsd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ivvv.top/gtyrhtihmo.html

[R60] 只看 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtpaxyjqll.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.9152youxi.cn/gtarykzhng.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtciomisnt.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtrmkojjqb.html

[R62] 找最占空间的文件
来源：http://hz.nanxinkj.top/gteimoxwye.html

du -ah . | sort -rh | head -10
来源：http://hz.ybcxt.top/gtwruxnjvr.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtlpxewtxs.html

free -h;  ps aux | grep nginx
来源：http://hz.gogol.net.cn/gtsfwjxnrk.html

[R64] 结束进程
来源：http://hz.fzhhl.top/gtxrdsdsav.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtjunrzmmv.html

[R65] 查看端口占用
来源：http://hz.ywan-chungtsiang.top/gtzvgaxcle.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sysykeji.top/gtpfbztjxn.html

[R66] 定时任务
来源：http://hz.dashuyun.cn/gtmxhwocqv.html

crontab -e;  crontab -l
来源：http://hz.daxiang520.top/gtrybnrdev.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtarajbgyg.html

openssl rand -hex 16
来源：http://hz.wangdashe.top/gtsxpulvqx.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtfijcpvcn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.quarkkingdee.top/gtzhmuizhb.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gtipsphewb.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtgasfgcfo.html

[R70] 时间戳与互转
来源：http://hz.shuidangran.top/gtycmgcbbo.html

date +%s;  date -d @1700000000
来源：http://hz.xuanzx.com/gtqyqyjesz.html

[R71] 日期格式化
来源：http://hz.kuanghao11.cn/gtngrsfoqg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtugnqqhve.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtcpxnahct.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gtyzipthjs.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtijitxklg.html

split -l 1000 big.log part_
来源：http://hz.daria6918.cn/gtgafwjool.html

[R74] 批量重命名
来源：http://hz.guowangkeji.top/gtpihfcmhz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guowangkeji.top/gtrsjjhffr.html

[R75] 导出环境变量
来源：http://hz.yuanzhike.top/gtuvmwlhma.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuetiantiany.cn/gtplbdmyue.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtzuvjjuuj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtjrorprvn.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gttwmjvlgx.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gtyyneomlk.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtyxtabqoj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sxryk.cn/gtshpgsbfm.html

[R79] 解析命令行选项
来源：http://hz.hnqzz.top/gtpokedqgm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xziqi.cn/gtuoehzcvt.html

[R80] 查看脚本执行耗时
来源：http://hz.quarkkingdee.top/gtjdiubvyv.html

time ./run.sh
来源：http://hz.nanxuanxn.top/gtywxntkwm.html

================================================================================
来源：http://hz.hywenlv.cn/gtfqnryqpp.html

S. C / C++ 专题
来源：http://hz.52xcode.cn/gtttxnnxls.html

================================================================================
来源：http://hz.zhixingplan.top/gtuoymxrjx.html

[S01] C：Hello World
来源：http://hz.hfpthk.cn/gtrysamchv.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtugndwdli.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shanyushiyangkeji.top/gtxycswsen.html

[S02] C：变量与格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtwadoxlif.html

int a = 10; printf("%d\n", a);
来源：http://hz.daria6918.cn/gtlwbnfuzq.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gteogjnvrc.html

int x; scanf("%d", &x);
来源：http://hz.haohaochexian.top/gtmujircbd.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtvxwbqwjt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gaohongyu789.top/gtalpbpbfu.html

[S05] C：字符串长度
来源：http://hz.aizwys.cn/gtfpwnznol.html

strlen(s)
来源：http://hz.shuidangran.top/gtipplmalu.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gtwfmtrjpb.html

strcmp(a, b) == 0
来源：http://hz.sysykeji.top/gtbrqrdsgu.html

[S07] C：数组遍历求和
来源：http://hz.sweek.top/gtagovoawe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.c1oappe.top/gtfeknvkfz.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtbgbwrtuo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhongyouzk.top/gtxgqmvdte.html

[S09] C：结构体定义与初始化
来源：http://hz.fengsongda.top/gtojzorxsa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yueranfly.top/gtnjfsehmt.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtkuechjyy.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtgprvbthx.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gtauyracpp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.iojbl.cn/gtvgqawsxj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xingfuxueyuan.xyz/gttzjrhxks.html

fclose(f);
来源：http://hz.dashuyun.cn/gtprdnudkn.html

[S12] C：写文件
来源：http://hz.0kj1m.cn/gtxaeplskq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ehwqpu.com/gtnsizhcrg.html

[S13] C：宏定义
来源：http://hz.hnxiangtu.top/gtcckosgvw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtnuiwtbqd.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gtmcnmxank.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangkeji.top/gtcbmpmgtu.html

[S15] C：类型转换
来源：http://hz.jqgfzy.top/gtkkizzznc.html

(double) a / b
来源：http://hz.zdqjudy.top/gtowojsstt.html

[S16] C：位操作置位
来源：http://hz.haohaochexian.top/gtmoymdiuv.html

x |= (1 << 3);
来源：http://hz.jinyuanbaomall.cn/gtwdxmdrzu.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gtrmibdinr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dianchejie.cn/gtkdghicqz.html

[S18] C：命令行参数
来源：http://hz.shuidangran.top/gtvmjmgrol.html

int main(int argc, char **argv)
来源：http://hz.zhengqikj.top/gtewlxpvzu.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gthoxjeffz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtjoqxkrfp.html

[S20] C：二分查找
来源：http://hz.yangfankeji.com/gtodvshzbm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gthxszbuhu.html

[S21] C：字符类别判断
来源：http://hz.redwolf501.top/gtpnujrxcy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gtroulxhhz.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gtczdzvmbv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangdashe.top/gtwjwpxoif.html

[S23] C：随机数
来源：http://hz.yuanzhike.top/gtwexamhgs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gtwalfvutw.html

[S24] C：获取本地时间
来源：http://hz.shangyingyoupin.top/gtbsbatpzx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yonumen.top/gtvqcizuap.html

[S25] C：内存拷贝
来源：http://hz.cheryme.top/gtrakoakwu.html

memcpy(dst, src, n);
来源：http://hz.sxryk.cn/gtexxsulnb.html

[S26] C：内存清零
来源：http://hz.tian-w.cn/gtsizqmfzt.html

memset(a, 0, sizeof a);
来源：http://hz.yanxiufei.cn/gtzaelgbrj.html

[S27] C：定义常量
来源：http://hz.tianlin.xyz/gtgvgbkxdx.html

const double PI = 3.14159;
来源：http://hz.yonumen.top/gtamrbsxrw.html

[S28] C：静态变量
来源：http://hz.9152youxi.cn/gtlnrwgvtk.html

static int counter = 0;
来源：http://hz.andypj.xyz/gtytkajvpn.html

[S29] C：变参函数
来源：http://hz.yvedp.cn/gtfbtmseqz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hysaishi.cn/gtenzjdbsg.html

[S30] C：头文件保护
来源：http://hz.meibo888.top/gtoeuuguie.html

#ifndef X_H
来源：http://hz.yangfankeji.com/gtoalccynr.html

#define X_H
来源：http://hz.jqgufenzy.top/gtcjitlqhp.html

#endif
来源：http://hz.tianlin.xyz/gtfgbxnjha.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtlnyzzqel.html

#include <iostream>
来源：http://hz.gaohongyu789.top/gtiucgbtsj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigfzy.top/gtviiwcieh.html

[S32] C++：字符串
来源：http://hz.tianlin.xyz/gtfangvupj.html

std::string s = "hi";  s += "!";
来源：http://hz.yueranfly.top/gtjwgigitn.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtdeqlsiut.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuetiantiany.cn/gtainzoorm.html

[S34] C++：遍历 vector
来源：http://hz.9152youxi.cn/gtnjmrhszs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xziqi.cn/gtqldplkmn.html

[S35] C++：map
来源：http://hz.vqdsnc.cn/gtprbnahof.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gttfefwfnl.html

[S36] C++：unordered_map
来源：http://hz.ydjk.org.cn/gtnyehvsnv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gteyqkvoee.html

[S37] C++：set
来源：http://hz.yj202588.top/gtyjrlzrrt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.redwolf501.top/gtcitmscat.html

[S38] C++：排序
来源：http://hz.yj202588.top/gtdaozcxrp.html

std::sort(v.begin(), v.end());
来源：http://hz.yj202588.top/gthldikrji.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtuilgspeo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ehwqpu.com/gtddtvvmfm.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtkbzxqxzk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj20258888.top/gtwpgbstjs.html

[S41] C++：类与构造函数
来源：http://hz.ywan-chungtsiang.top/gtvdbsdotj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ywan-chungtsiang.top/gtgjwidhyk.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gtovznkayy.html

class B : public Base { public: void f() override {} };
来源：http://hz.shuidangran.top/gtafdabmrk.html

[S43] C++：智能指针
来源：http://hz.gogol.net.cn/gtfoibovht.html

auto p = std::make_unique<int>(5);
来源：http://hz.ywan-chungtsiang.top/gtgfosyjbv.html

[S44] C++：引用传参
来源：http://hz.yongpay.top/gtsjmwwygl.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtqzmmpplv.html

[S45] C++：lambda
来源：http://hz.yuxming.cn/gtcbvdaboq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xinyue.icu/gtofsespqf.html

[S46] C++：函数模板
来源：http://hz.jiagoushi.top/gtvvvtpwrr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtttkwdvqc.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gturkmdivh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.meibo888.top/gtnbdbmleh.html

[S48] C++：逐行读文件
来源：http://hz.yangfankeji.com/gtecvlidnd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtxnrlcuea.html

while (std::getline(in, line)) { }
来源：http://hz.xinyue.icu/gtqiygjtvu.html

[S49] C++：写文件
来源：http://hz.zdqjudy.top/gtbdohgicx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jianghu66.top/gtbgaebome.html

[S50] C++：格式化数字
来源：http://hz.shzxlz.cn/gtsdulqlnk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuetiantiany.cn/gtobxxbnlg.html

[S51] C++：显式类型转换
来源：http://hz.quarkkingdee.top/gtyjglxmhj.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtzleowikk.html

[S52] C++：const 与 noexcept
来源：http://hz.sufxvd.cn/gtdcdyoevf.html

int size() const noexcept { return n_; }
来源：http://hz.yonumen.top/gtmplemray.html

[S53] C++：移动语义
来源：http://hz.tian-w.cn/gtvgvozuxl.html

std::vector<int> w = std::move(v);
来源：http://hz.tian-w.cn/gtdgizlbxh.html

[S54] C++：异常处理
来源：http://hz.gaohongyu789.top/gtdselqgxw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pengpengdd.cyou/gtkeijjbkr.html

[S55] C++：结构化绑定
来源：http://hz.gogol.net.cn/gtwbejvott.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hammf.cn/gtmkpgvvsr.html

[S56] C++：optional
来源：http://hz.zhengqikj.top/gtyrcuouvc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.kuanghao11.cn/gtyopslusj.html

[S57] C++：编译期常量
来源：http://hz.yj202588.top/gtpsmdztpj.html

constexpr int N = 10;
来源：http://hz.jqgufenzy.top/gtpiiugact.html

[S58] C++：命名空间
来源：http://hz.zhongyouzk.top/gtemtrzecy.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtpimasodh.html

[S59] C++：静态断言
来源：http://hz.jinqigufen.top/gtnaalkami.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnxiangtu.top/gtdinemchr.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gtmcwpyrja.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangdashe.top/gtgjsxhgwu.html

================================================================================
来源：http://hz.havefunace.top/gtxeugrwzo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gttxgvysyl.html

================================================================================
来源：http://hz.mhx1999.top/gtudiilpgo.html

[T01] Kotlin：Hello World
来源：http://hz.xuanzx.com/gtshjcfxbn.html

println("Hello")
来源：http://hz.gogol.net.cn/gtbnnhgyzf.html

[T02] Kotlin：变量
来源：http://hz.iojbl.cn/gtucxnvuqc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnqzz.top/gtvvwpycqf.html

[T03] Kotlin：字符串模板
来源：http://hz.ydjk.org.cn/gtjpveflmf.html

"值: $b"
来源：http://hz.yj20258888.top/gtmgwazoon.html

[T04] Kotlin：空安全
来源：http://hz.iojbl.cn/gtkhtwzbvt.html

val n: String? = null;  n?.length
来源：http://hz.tanke756.top/gtkxkhlnyw.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gthrfugdts.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sysykeji.top/gtsulayljr.html

[T06] Kotlin：集合映射
来源：http://hz.jlsjyb.cn/gtuqtyvqnt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuanzhike.top/gtiecugngi.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtkqmglcvx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtkoleztgq.html

[T08] Kotlin：数据类
来源：http://hz.jinqigfzy.top/gtjqvrujee.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtxoymbwsy.html

[T09] Kotlin：扩展函数
来源：http://hz.tianlin.xyz/gttatsrsng.html

fun String.exclaim() = this + "!"
来源：http://hz.316326.xyz/gtzopsnack.html

[T10] Kotlin：默认参数
来源：http://hz.kuanghao11.cn/gtghraxkak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtcbeffvsl.html

[T11] Kotlin：协程
来源：http://hz.yj202588.top/gtepyzpgkm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yonumen.top/gtnhlqfgks.html

[T12] Kotlin：解构声明
来源：http://hz.smart0.xyz/gtyzmcgwiq.html

val (a, b) = Pair(1, 2)
来源：http://hz.hysaishi.cn/gtkvdgenez.html

[T13] Kotlin：只读 Map
来源：http://hz.xuetiantiany.cn/gtqqmfvwdf.html

val m = mapOf("a" to 1)
来源：http://hz.snrcjt.cn/gtxyuoxjzf.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtzbecspio.html

for (i in 1..10) println(i)
来源：http://hz.birdmap.top/gtuonyitgu.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gtzlmjnvwq.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258.top/gtokdymfdw.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gthyepuhih.html

print("Hello")
来源：http://hz.sufxvd.cn/gtzywzcqhw.html

[T17] Swift：变量与常量
来源：http://hz.aizwys.cn/gtuwxobrts.html

var a = 1;  let b = 2
来源：http://hz.gaohongyu789.top/gtbxhkbtfl.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtgjatbyvi.html

"值: \(b)"
来源：http://hz.fengsongda.top/gtccmqbshp.html

[T19] Swift：可选绑定
来源：http://hz.snrcjt.cn/gttzfqakhm.html

if let n = opt { print(n) }
来源：http://hz.pengpengdd.cyou/gtnxbtnofg.html

[T20] Swift：数组操作
来源：http://hz.52xcode.cn/gtfowerhti.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jlsjyb.cn/gtbxsqfhjl.html

[T21] Swift：遍历
来源：http://hz.jlsjyb.cn/gtktclmzgi.html

for x in a { print(x) }
来源：http://hz.meibo888.top/gtfqaykabm.html

[T22] Swift：字典
来源：http://hz.fengsongda.top/gtbbgzzpoh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zdqjudy.top/gtunnkwbui.html

[T23] Swift：函数
来源：http://hz.hammf.cn/gtvaddncgv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtmobdlfry.html

[T24] Swift：闭包
来源：http://hz.c1oappe.top/gtreaytzye.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xziqi.cn/gtpmfvdmez.html

[T25] Swift：结构体
来源：http://hz.meibo888.top/gtvnkcjjnp.html

struct P { var x: Int }
来源：http://hz.mhx1999.top/gtnmgezjcd.html

[T26] Swift：类与重写
来源：http://hz.aizwys.cn/gtyjgsxmbp.html

class A: Base { override func f() {} }
来源：http://hz.hfpthk.cn/gtoepwkfcf.html

[T27] Swift：错误处理
来源：http://hz.52xcode.cn/gttmybkjzc.html

do { try f() } catch { print(error) }
来源：http://hz.guowangkeji.top/gtjoipbwut.html

[T28] Swift：枚举
来源：http://hz.cdnleiting.top/gtrvgiclhs.html

enum Color { case red, green }
来源：http://hz.cucudq.cn/gtkagbnssw.html

[T29] Swift：guard 提前返回
来源：http://hz.ivvv.top/gtnxlvnhud.html

guard let x = opt else { return }
来源：http://hz.cashguo.top/gtqncutvko.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtodqqursg.html

protocol Shape { func area() -> Double }
来源：http://hz.xziqi.cn/gtsaomwnnh.html

[T31] Lua：Hello World
来源：http://hz.zhixingplan.top/gtseyguxzj.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtpwwiiner.html

[T32] Lua：局部变量
来源：http://hz.quarkkingdee.top/gtmrxvdquu.html

local a = 1
来源：http://hz.haohaochexian.top/gtdiktraat.html

[T33] Lua：表（数组）
来源：http://hz.dianchejie.cn/gtzhiayvow.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhoulong.xyz/gtiolpmgsi.html

[T34] Lua：遍历表
来源：http://hz.zhijiandao.cn/gtphgobqtm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxinkj.top/gtafdjaclh.html

[T35] Lua：字典表
来源：http://hz.xuetiantiany.cn/gtrbvokqni.html

local d = { a = 1 };  d.b = 2
来源：http://hz.9152youxi.cn/gtnmggxxrh.html

[T36] Lua：函数
来源：http://hz.shanyushiyangtech.top/gtbrgotsfr.html

function add(a, b) return a + b end
来源：http://hz.zycfv.cn/gtghnbckow.html

[T37] Lua：字符串拼接
来源：http://hz.xuanzx.com/gtcjupayxw.html

"a" .. "b"
来源：http://hz.nanxuanxn.top/gthoowpftm.html

[T38] Lua：条件
来源：http://hz.fzhhl.top/gtroehzxge.html

if x > 0 then print("正") end
来源：http://hz.jinghuilouyu.cn/gtfgrayyui.html

[T39] Lua：模式匹配
来源：http://hz.wangshuangyany.cn/gtcfqzmxax.html

string.find(s, "%d+")
来源：http://hz.jinyuanbaomall.cn/gtvomwuszi.html

[T40] Lua：元表
来源：http://hz.dashuyun.cn/gtcadgaryu.html

setmetatable({}, { __index = base })
来源：http://hz.52xcode.cn/gtudsccivs.html

[T41] Perl：Hello World
来源：http://hz.yvedp.cn/gtelxsjatk.html

print "Hello\n";
来源：http://hz.sufxvd.cn/gtmmdwgwzc.html

[T42] Perl：变量类型
来源：http://hz.tian-w.cn/gtvxsdmaks.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ybcxt.top/gtdtwmudek.html

[T43] Perl：字符串插值
来源：http://hz.wangshuangyany.cn/gtcrqpcdey.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gtzggrbztd.html

[T44] Perl：条件
来源：http://hz.jlsjyb.cn/gtuplhhtsh.html

if ($a > 0) { print "正"; }
来源：http://hz.xuetiantiany.cn/gtgsikllur.html

[T45] Perl：数组遍历
来源：http://hz.hywenlv.cn/gttvcbbrle.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgufenzy.top/gtlolhbeuy.html

[T46] Perl：哈希操作
来源：http://hz.shanyushiyangtech.top/gtyccaspje.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.smart0.xyz/gtiijoenaw.html


<!-- 参考信息 -->