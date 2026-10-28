代发 wailian999

cmd >/dev/null 2>&1
来源：http://hz.zhiwuduotai.top/gtvqfwreyn.html

[R42] 输入重定向
来源：http://hz.xingfuxueyuan.xyz/gtpxwradiv.html

wc -l < a.txt
来源：http://hz.nanxinkj.top/gtdbivenve.html

[R43] 按名字查找文件
来源：http://hz.smart0.xyz/gtqhefshrv.html

find . -name "*.log" -type f
来源：http://hz.feifeiyinyue.top/gtupfuitxj.html

[R44] 按修改时间查找
来源：http://hz.yuanzhike.top/gtnfguddqp.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtspmkecxr.html

[R45] 批量删除
来源：http://hz.tian-w.cn/gtqgilguou.html

find . -name "*.tmp" -delete
来源：http://hz.pycfn.com/gtwnnaheem.html

[R46] 递归替换文件内容
来源：http://hz.chenlongwang.top/gtvrfupctk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zycfv.cn/gtvhjxdzbj.html

[R47] sed 单行替换
来源：http://hz.guannengcc.top/gtqmxpvqtk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtoznxxcdu.html

[R48] awk 取指定列
来源：http://hz.jlsjyb.cn/gtwbnkftfu.html

awk '{print $1, $3}' a.txt
来源：http://hz.yanxiufei.cn/gtvbroxsop.html

[R49] awk 带条件
来源：http://hz.jlsjyb.cn/gttrhdwsqx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jianghu66.top/gtdllkczki.html

[R50] awk 求和
来源：http://hz.pengpengdd.cyou/gtixjvpgip.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtgqxpxdwn.html

[R51] 排序去重取前几
来源：http://hz.kuanghao11.cn/gtjilbgjpo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenzaomai.com/gtpkzrqdmo.html

[R52] 统计行数
来源：http://hz.shuidangran.top/gtmjagpijj.html

wc -l a.txt
来源：http://hz.wangdashe.top/gtohyupiyv.html

[R53] 查看文件头与实时尾
来源：http://hz.yj202588.top/gtnmhycasa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aizwys.cn/gtmuvqigwq.html

[R54] 比较两个文件
来源：http://hz.ppjwa.cn/gtfducuttr.html

diff a.txt b.txt
来源：http://hz.zycfv.cn/gtujgoyxkz.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtfvvjnzjk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jianghu66.top/gtdpsiisgz.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtkpkeqwve.html

scp file user@host:/path/
来源：http://hz.gogol.net.cn/gtsiioafco.html

[R57] 远程执行命令
来源：http://hz.jqgufenzy.top/gtishojhdv.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtguxdasik.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtnyfxadfg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.feifeiyinyue.top/gtzakwwfwh.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtvfukpkvr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.feifeiyinyue.top/gtkgahbfqq.html

[R60] 只看 HTTP 状态码
来源：http://hz.sweek.top/gtevqrcsta.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgufenzy.top/gtheveuzwu.html

[R61] 磁盘占用
来源：http://hz.chenzaomai.com/gtsrsykozu.html

df -h;  du -sh *
来源：http://hz.daria6918.cn/gtxymeswmt.html

[R62] 找最占空间的文件
来源：http://hz.c1oappe.top/gtuwvfagvg.html

du -ah . | sort -rh | head -10
来源：http://hz.ywan-chungtsiang.top/gtjfppjigy.html

[R63] 内存与进程
来源：http://hz.ywan-chungtsiang.top/gthudbcxpq.html

free -h;  ps aux | grep nginx
来源：http://hz.yj202588.top/gtwzjyexsu.html

[R64] 结束进程
来源：http://hz.zhoulong.xyz/gtonbqrjyk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.mhx1999.top/gtryugkcbq.html

[R65] 查看端口占用
来源：http://hz.sxryk.cn/gtnqjernez.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangtech.top/gttzqpmcjm.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtridfvukk.html

crontab -e;  crontab -l
来源：http://hz.yanxiufei.cn/gtegvioedz.html

[R67] 生成随机十六进制串
来源：http://hz.gotoacloud.top/gtluribpjv.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtywdyiacz.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtdguqpkey.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aizwys.cn/gtrmscmthh.html

[R69] 生成随机密码
来源：http://hz.jqgfzy.top/gtjjoiemvg.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigufen.top/gtaiimevdg.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtihagvevn.html

date +%s;  date -d @1700000000
来源：http://hz.mhx1999.top/gtlvqnagcq.html

[R71] 日期格式化
来源：http://hz.smart0.xyz/gtjuvxvlxk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgufenzy.top/gtunjoziyz.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gttxivuafx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.smart0.xyz/gttemuydgm.html

[R73] 分割大日志
来源：http://hz.ydzc1.top/gtbtxnpugl.html

split -l 1000 big.log part_
来源：http://hz.hysaishi.cn/gtiguddkxj.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtlgwzeoav.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtbxikvlue.html

[R75] 导出环境变量
来源：http://hz.sweek.top/gthvhjatus.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gtwxrqyaik.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gtefdzrify.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtlluhrsjd.html

[R77] 读取用户输入
来源：http://hz.cucudq.cn/gtguenkqkp.html

read -rp "请输入: " ans
来源：http://hz.ivvv.top/gtradowqaz.html

[R78] 交互式菜单
来源：http://hz.jqgfzy.top/gtssgsggmf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtlzyzwgyr.html

[R79] 解析命令行选项
来源：http://hz.zdqjudy.top/gtayjgpnlo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hnqzz.top/gtzdkdwxod.html

[R80] 查看脚本执行耗时
来源：http://hz.cashguo.top/gtaxollfhb.html

time ./run.sh
来源：http://hz.zhijiandao.cn/gtyqypbbif.html

================================================================================
来源：http://hz.fengsongda.top/gtufklhzbg.html

S. C / C++ 专题
来源：http://hz.ywan-chungtsiang.top/gtvwpbtisl.html

================================================================================
来源：http://hz.xylfe.cn/gtyoohfqjb.html

[S01] C：Hello World
来源：http://hz.cucudq.cn/gttmbcpqzo.html

#include <stdio.h>
来源：http://hz.jqgfzy.top/gtneegugqn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yueranfly.top/gtxahlhuad.html

[S02] C：变量与格式化输出
来源：http://hz.kuanghao11.cn/gtpjauxvou.html

int a = 10; printf("%d\n", a);
来源：http://hz.yonumen.top/gtdczkfiaz.html

[S03] C：读入整数
来源：http://hz.jinyuanbaomall.cn/gtiqgyrubl.html

int x; scanf("%d", &x);
来源：http://hz.c1oappe.top/gtvqqerzyf.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtqjfovgxb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nwbrower.top/gtzwgxsihg.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtthicvarx.html

strlen(s)
来源：http://hz.xuanzx.com/gtykuxwaun.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtrggqgpeg.html

strcmp(a, b) == 0
来源：http://hz.yueranfly.top/gtksonocvk.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gttotclhel.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gtgzuzqrhz.html

[S08] C：动态内存分配与释放
来源：http://hz.cheryme.top/gtyzpfeqse.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhijiandao.cn/gtkqtoygpw.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtrgskfmhn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuanzx.com/gtcitwxqdd.html

[S10] C：指针与解引用
来源：http://hz.jiagoushi.top/gtwqtkmnro.html

int *p = &a;  *p = 5;
来源：http://hz.dianchejie.cn/gtsiejnpkj.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtnfhqxgog.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gtsnfuayud.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtdtroosez.html

fclose(f);
来源：http://hz.chenzaomai.com/gtiehoqluf.html

[S12] C：写文件
来源：http://hz.redwolf501.top/gtepyfjexy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sufxvd.cn/gtzvpiwcws.html

[S13] C：宏定义
来源：http://hz.tianlin.xyz/gtntgcdotw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tian-w.cn/gtxkbnqrth.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtsathcazk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnqzz.top/gtclrkeyeq.html

[S15] C：类型转换
来源：http://hz.daxiang520.top/gteybcsvuo.html

(double) a / b
来源：http://hz.vqdsnc.cn/gtrpubzbls.html

[S16] C：位操作置位
来源：http://hz.jqgfzy.top/gtawvtzdin.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtsjgztwjm.html

[S17] C：安全拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtqojzubrl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jianghu66.top/gtrygwdsko.html

[S18] C：命令行参数
来源：http://hz.jqgfzy.top/gtyqmszfoh.html

int main(int argc, char **argv)
来源：http://hz.dashuyun.cn/gtkectivdh.html

[S19] C：快速排序
来源：http://hz.cheryme.top/gtnhoqdgtx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtkexsarxd.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtugkazuuv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtqutkzuxg.html

[S21] C：字符类别判断
来源：http://hz.cqqwz.cn/gtxfttupsa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.smart0.xyz/gtunesfvio.html

[S22] C：字符串转数字
来源：http://hz.yuanzhike.top/gtjzrwmlrz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cdnleiting.top/gtkghspggg.html

[S23] C：随机数
来源：http://hz.jqgfzy.top/gtkiqqzzbk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gtjbqyfdxd.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gttwctxwir.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinyuanbaomall.cn/gtbbaeaiml.html

[S25] C：内存拷贝
来源：http://hz.gaohongyu789.top/gtdnefzttm.html

memcpy(dst, src, n);
来源：http://hz.hnqzz.top/gtejgrkkko.html

[S26] C：内存清零
来源：http://hz.tian-w.cn/gtyvpzqlsu.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gtjxwoufsy.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gtjuktktjq.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtpdjnthzo.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtmnmwjbco.html

static int counter = 0;
来源：http://hz.gaohongyu789.top/gtlpvzaryk.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gtcfpkrvgv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnqzz.top/gteujrovvz.html

[S30] C：头文件保护
来源：http://hz.zhixingplan.top/gtuoxdkbwt.html

#ifndef X_H
来源：http://hz.yj20258.top/gtsjlpibwa.html

#define X_H
来源：http://hz.yuxming.cn/gtbedncquf.html

#endif
来源：http://hz.ivvv.top/gtmoajwlzk.html

[S31] C++：Hello World
来源：http://hz.0kj1m.cn/gtljvpnifo.html

#include <iostream>
来源：http://hz.smart0.xyz/gttolzyqam.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hongshengwenyu.top/gtyxsgsgcx.html

[S32] C++：字符串
来源：http://hz.zhoulong.xyz/gtwfwtljdh.html

std::string s = "hi";  s += "!";
来源：http://hz.redwolf501.top/gtpbbplqdf.html

[S33] C++：vector 增删
来源：http://hz.yanxiufei.cn/gtamsuxxmk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yongpay.top/gtlyefilmf.html

[S34] C++：遍历 vector
来源：http://hz.nanxuanxn.top/gtipjlswys.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.iojbl.cn/gtnzprnhqs.html

[S35] C++：map
来源：http://hz.smart0.xyz/gthpkkiqxe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtjzqopeho.html

[S36] C++：unordered_map
来源：http://hz.jinqigfzy.top/gtgpelrorg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtbjaeamby.html

[S37] C++：set
来源：http://hz.yangfankeji.com/gtgbrcssea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtcgupvfgv.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtqlmfkbbq.html

std::sort(v.begin(), v.end());
来源：http://hz.ehwqpu.com/gtvktuufab.html

[S39] C++：自定义比较器排序
来源：http://hz.0kj1m.cn/gtzwbofrde.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.redwolf501.top/gtdfmslerb.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtufigvtjk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuanzx.com/gtdofxduxw.html

[S41] C++：类与构造函数
来源：http://hz.fzhhl.top/gtdaiupohw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gthfjesfwt.html

[S42] C++：继承与虚函数
来源：http://hz.pengpengdd.cyou/gtpnucaqdb.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtxkvdzzyu.html

[S43] C++：智能指针
来源：http://hz.fzhhl.top/gtepsvdtwi.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gtejydnphf.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtwenkqsry.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gtfowpjocg.html

[S45] C++：lambda
来源：http://hz.52xcode.cn/gtrmfvnxbt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj20258888.top/gtzxkezefb.html

[S46] C++：函数模板
来源：http://hz.pycfn.com/gtasiqvkdw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.vqdsnc.cn/gtvhsaypmf.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtavylwdsq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.iojbl.cn/gtjogeqfmx.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtllxjjcsm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sysykeji.top/gteeswkyze.html

while (std::getline(in, line)) { }
来源：http://hz.smart0.xyz/gthvutgfel.html

[S49] C++：写文件
来源：http://hz.wangshuangyany.cn/gtfkwlfszf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sysykeji.top/gtbrynyted.html

[S50] C++：格式化数字
来源：http://hz.52xcode.cn/gtlpjycybk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.mhx1999.top/gttqrhtaku.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtlkkhdwwz.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtvoxzhxvk.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtzykquyha.html

int size() const noexcept { return n_; }
来源：http://hz.havefunace.top/gtzfqnioqb.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gtfexvsbzq.html

std::vector<int> w = std::move(v);
来源：http://hz.havefunace.top/gtodhmyxir.html

[S54] C++：异常处理
来源：http://hz.bjfxy.top/gtbfxjgzfv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gtfonwrjye.html

[S55] C++：结构化绑定
来源：http://hz.tian-w.cn/gtwdiobmjy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigfzy.top/gtxnhqurog.html

[S56] C++：optional
来源：http://hz.smart0.xyz/gtdeenqvtb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cucudq.cn/gtioovgvpr.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtttdxidxh.html

constexpr int N = 10;
来源：http://hz.dashuyun.cn/gtizupuifa.html

[S58] C++：命名空间
来源：http://hz.cdnleiting.top/gthfdfkaex.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gthrppqmdv.html

[S59] C++：静态断言
来源：http://hz.jiagoushi.top/gtfibghnzq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yongpay.top/gtzujbflmj.html

[S60] C++：遍历并删除元素
来源：http://hz.fengsongda.top/gtwfjfovap.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ppjwa.cn/gtooekvufk.html

================================================================================
来源：http://hz.meibo888.top/gtqcrhqrpu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenlongwang.top/gtdpdaetvj.html

================================================================================
来源：http://hz.ydzc1.top/gtqslahwcx.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gtkjhzvhyt.html

println("Hello")
来源：http://hz.andypj.xyz/gtqcrkjgov.html

[T02] Kotlin：变量
来源：http://hz.316326.xyz/gtoxbmbiln.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yvedp.cn/gtkucsgzmn.html

[T03] Kotlin：字符串模板
来源：http://hz.xinyue.icu/gtzftvgixj.html

"值: $b"
来源：http://hz.yongpay.top/gtppgtuvgg.html

[T04] Kotlin：空安全
来源：http://hz.gotoacloud.top/gtagooceql.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtzhqgmwjs.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gtlrxkzump.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtiwicgzqb.html

[T06] Kotlin：集合映射
来源：http://hz.pycfn.com/gtykjzwddr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenjidiqi.icu/gtqpczrxfl.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtcedvwupn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zdqjudy.top/gtixxvdiir.html

[T08] Kotlin：数据类
来源：http://hz.52xcode.cn/gtrnqsvtou.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtuijqykep.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtahyboacf.html

fun String.exclaim() = this + "!"
来源：http://hz.daxiang520.top/gtbrgskzmb.html

[T10] Kotlin：默认参数
来源：http://hz.chenlongwang.top/gtgmhfanjh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtrcpfojjn.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gtsejitcxk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxinkj.top/gtotvtrcce.html

[T12] Kotlin：解构声明
来源：http://hz.jinqigufen.top/gtfwrzdltw.html

val (a, b) = Pair(1, 2)
来源：http://hz.cucudq.cn/gtlipkrpvx.html

[T13] Kotlin：只读 Map
来源：http://hz.cdnleiting.top/gtxgviialy.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gtbelnpmyx.html

[T14] Kotlin：循环
来源：http://hz.smart0.xyz/gtmdxycbpp.html

for (i in 1..10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtmpwfvvba.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gtkmlqcwdm.html

interface Shape { fun area(): Double }
来源：http://hz.jyoumei.cn/gttualsiwe.html

[T16] Swift：Hello World
来源：http://hz.nwbrower.top/gtrowoavvc.html

print("Hello")
来源：http://hz.birdmap.top/gtppyksefr.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gtyarkfmlh.html

var a = 1;  let b = 2
来源：http://hz.hfpthk.cn/gtyxvtcirj.html

[T18] Swift：字符串插值
来源：http://hz.hnxiangtu.top/gtjlqoppbd.html

"值: \(b)"
来源：http://hz.haohaochexian.top/gtvkorvkoa.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gtqhtnbusu.html

if let n = opt { print(n) }
来源：http://hz.pengpengdd.cyou/gtqpbkoqwi.html

[T20] Swift：数组操作
来源：http://hz.tianlin.xyz/gtsjnhrfjo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.kuanghao11.cn/gtnakcscjc.html

[T21] Swift：遍历
来源：http://hz.guowangkeji.top/gtjwmfdeyh.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gtfsefxbxk.html

[T22] Swift：字典
来源：http://hz.kuanghao11.cn/gtkcknepyx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgfzy.top/gtpxtgfyce.html

[T23] Swift：函数
来源：http://hz.gzhubu.top/gtkktpeset.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.havefunace.top/gtnoxxyynw.html

[T24] Swift：闭包
来源：http://hz.yuanzhike.top/gthzsmhoii.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zdqjudy.top/gtjbgniwqt.html

[T25] Swift：结构体
来源：http://hz.zhijiandao.cn/gtnlberbwy.html

struct P { var x: Int }
来源：http://hz.nanxuanxn.top/gtgjtnuruh.html

[T26] Swift：类与重写
来源：http://hz.ehwqpu.com/gtwyoculcl.html

class A: Base { override func f() {} }
来源：http://hz.andypj.xyz/gtliavojjr.html

[T27] Swift：错误处理
来源：http://hz.iojbl.cn/gtldyricgt.html

do { try f() } catch { print(error) }
来源：http://hz.fengsongda.top/gtlgwfvver.html

[T28] Swift：枚举
来源：http://hz.gotoacloud.top/gtalmgkezc.html

enum Color { case red, green }
来源：http://hz.cdnleiting.top/gtyxbvlrzy.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gttpghgtyx.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtyuqtgnpz.html

[T30] Swift：协议
来源：http://hz.shuidangran.top/gtjeoviurx.html

protocol Shape { func area() -> Double }
来源：http://hz.andypj.xyz/gthltxmbou.html

[T31] Lua：Hello World
来源：http://hz.pengpengdd.cyou/gtxsgrngzb.html

print("Hello")
来源：http://hz.cheryme.top/gtanhfvxxd.html

[T32] Lua：局部变量
来源：http://hz.ppjwa.cn/gtknhsddls.html

local a = 1
来源：http://hz.sufxvd.cn/gtiwifhpqa.html

[T33] Lua：表（数组）
来源：http://hz.ehwqpu.com/gtrhdnqfqw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigufen.top/gtaekyccdc.html

[T34] Lua：遍历表
来源：http://hz.0kj1m.cn/gtivavffxz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yanxiufei.cn/gtsiaqlhyf.html

[T35] Lua：字典表
来源：http://hz.0kj1m.cn/gtinfmfoqd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.quarkkingdee.top/gtabmjutxh.html

[T36] Lua：函数
来源：http://hz.daria6918.cn/gtdpyopiqr.html

function add(a, b) return a + b end
来源：http://hz.yj20258.top/gtnfbmkmwy.html

[T37] Lua：字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtandtscdy.html

"a" .. "b"
来源：http://hz.mhx1999.top/gtnomxquhr.html

[T38] Lua：条件
来源：http://hz.shuidangran.top/gtdviubwns.html

if x > 0 then print("正") end
来源：http://hz.jiagoushi.top/gtncvyrapi.html

[T39] Lua：模式匹配
来源：http://hz.daxiang520.top/gtuutmzhtq.html

string.find(s, "%d+")
来源：http://hz.9152youxi.cn/gtzlwjyyqc.html

[T40] Lua：元表
来源：http://hz.cheryme.top/gtzjfqoexn.html

setmetatable({}, { __index = base })
来源：http://hz.gaohongyu789.top/gthfkgxphw.html

[T41] Perl：Hello World
来源：http://hz.iojbl.cn/gtnzilkuee.html

print "Hello\n";
来源：http://hz.pycfn.com/gtslwwbblt.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtnbsrpulm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yueranfly.top/gtvtjwqybp.html

[T43] Perl：字符串插值
来源：http://hz.9152youxi.cn/gtftjbvlpi.html

"值: $a"
来源：http://hz.zycfv.cn/gtkbucacki.html

[T44] Perl：条件
来源：http://hz.wangdashe.top/gtpgqbzzkp.html

if ($a > 0) { print "正"; }
来源：http://hz.redwolf501.top/gtrdvdtvko.html


<!-- 参考信息 -->