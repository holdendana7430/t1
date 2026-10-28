代发 wailian999

find . -name "*.log" -type f
来源：http://hz.zhongyouzk.top/gtjxbqtjlr.html

[R44] 按修改时间查找
来源：http://hz.fengsongda.top/gtvargfhoi.html

find . -mtime -7 -type f
来源：http://hz.jqgufenzy.top/gtmnamtwoj.html

[R45] 批量删除
来源：http://hz.guannengcc.top/gtbfmsthqg.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtkaecmruu.html

[R46] 递归替换文件内容
来源：http://hz.daxiang520.top/gteywyuwrk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gogol.net.cn/gtkcexzcuc.html

[R47] sed 单行替换
来源：http://hz.jinyuanbaomall.cn/gtrykzfpqb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtiqijtkab.html

[R48] awk 取指定列
来源：http://hz.ppjwa.cn/gttdoovofz.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgufenzy.top/gtehxgbqex.html

[R49] awk 带条件
来源：http://hz.yuxming.cn/gtkgnarqcy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.havefunace.top/gtpkqobftm.html

[R50] awk 求和
来源：http://hz.jinqigufen.top/gtzdymadgk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hywenlv.cn/gtxlsllvpp.html

[R51] 排序去重取前几
来源：http://hz.jinyuanbaomall.cn/gtswydidpk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgfzy.top/gtzzkjyzrd.html

[R52] 统计行数
来源：http://hz.zhengqikj.top/gtjgjipqvu.html

wc -l a.txt
来源：http://hz.zhixingplan.top/gtugunhwzm.html

[R53] 查看文件头与实时尾
来源：http://hz.vqdsnc.cn/gtygnvyxop.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtkngxztvg.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtnoaovyco.html

diff a.txt b.txt
来源：http://hz.vqdsnc.cn/gtlhdsckxz.html

[R55] 压缩与解压
来源：http://hz.gzhubu.top/gtsmnhgliq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shuidangran.top/gtbblpjkfy.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtkzjcyoxw.html

scp file user@host:/path/
来源：http://hz.jyoumei.cn/gtzlmzvjaq.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtezxdnfvo.html

ssh user@host 'uptime'
来源：http://hz.ywan-chungtsiang.top/gtqbwptvmq.html

[R58] 下载文件
来源：http://hz.yj20258.top/gteualkmql.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shuidangran.top/gtvptdqjvh.html

[R59] 发 POST JSON
来源：http://hz.bjfxy.top/gtrxenzhqx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daria6918.cn/gtiaegtluj.html

[R60] 只看 HTTP 状态码
来源：http://hz.fzhhl.top/gthuuhuwro.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yvedp.cn/gtmnqsxxld.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtcfyozazi.html

df -h;  du -sh *
来源：http://hz.cucudq.cn/gtwkzzryio.html

[R62] 找最占空间的文件
来源：http://hz.ivvv.top/gtxickvooc.html

du -ah . | sort -rh | head -10
来源：http://hz.ivvv.top/gtdqrtbxag.html

[R63] 内存与进程
来源：http://hz.cucudq.cn/gthlvxofcs.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtjeymotbt.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtbhggzdjy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dianchejie.cn/gtgxqvosdz.html

[R65] 查看端口占用
来源：http://hz.52xcode.cn/gtyqrvlnnh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhijiandao.cn/gtwqojihyt.html

[R66] 定时任务
来源：http://hz.smart0.xyz/gtbdogwqaj.html

crontab -e;  crontab -l
来源：http://hz.sweek.top/gtiptjgyth.html

[R67] 生成随机十六进制串
来源：http://hz.zhijiandao.cn/gtwwnhysvw.html

openssl rand -hex 16
来源：http://hz.havefunace.top/gtlqqsxhxk.html

[R68] 计算文件校验值
来源：http://hz.yueranfly.top/gthjpxwrik.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xinyue.icu/gtsxynruci.html

[R69] 生成随机密码
来源：http://hz.yuxming.cn/gtustfqtgo.html

head -c 16 /dev/urandom | base64
来源：http://hz.haohaochexian.top/gtaudhkktj.html

[R70] 时间戳与互转
来源：http://hz.zhixingplan.top/gtrecuyyjg.html

date +%s;  date -d @1700000000
来源：http://hz.cashguo.top/gtxfmqfaju.html

[R71] 日期格式化
来源：http://hz.chenzaomai.com/gtirpqjjfk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtqsfzsbzj.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtoaclwace.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.smart0.xyz/gtjgizhxvq.html

[R73] 分割大日志
来源：http://hz.hfpthk.cn/gtawipvodu.html

split -l 1000 big.log part_
来源：http://hz.sweek.top/gthuzrbdgp.html

[R74] 批量重命名
来源：http://hz.yongpay.top/gttrirxelk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgfzy.top/gtaqteexvp.html

[R75] 导出环境变量
来源：http://hz.hfpthk.cn/gtutztpmlr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gtfrbgxtkw.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtsuscqizl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtrrzrpfxi.html

[R77] 读取用户输入
来源：http://hz.tianlin.xyz/gtuhhceill.html

read -rp "请输入: " ans
来源：http://hz.zhijiandao.cn/gtdiyinhra.html

[R78] 交互式菜单
来源：http://hz.andypj.xyz/gtmrhylhyh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinghuilouyu.cn/gttqetxmwh.html

[R79] 解析命令行选项
来源：http://hz.hongshengwenyu.top/gtlqnvcmbg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.316326.xyz/gtxxsxosde.html

[R80] 查看脚本执行耗时
来源：http://hz.gzhubu.top/gtbffdntir.html

time ./run.sh
来源：http://hz.guowangkeji.top/gtisdqrppe.html

================================================================================
来源：http://hz.daria6918.cn/gtfrenzktn.html

S. C / C++ 专题
来源：http://hz.tian-w.cn/gthyznphnp.html

================================================================================
来源：http://hz.xinyue.icu/gtldkgrset.html

[S01] C：Hello World
来源：http://hz.cucudq.cn/gtaextcmfa.html

#include <stdio.h>
来源：http://hz.hywenlv.cn/gthtvlnvrr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ybcxt.top/gttteozbyj.html

[S02] C：变量与格式化输出
来源：http://hz.hammf.cn/gtxdyjwjgy.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtprodqltb.html

[S03] C：读入整数
来源：http://hz.yonumen.top/gtmbpssqfm.html

int x; scanf("%d", &x);
来源：http://hz.sweek.top/gtuopfmmvb.html

[S04] C：字符串复制
来源：http://hz.jinghuilouyu.cn/gtckqxvxyb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangdashe.top/gtcfhgtojw.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtbsffatya.html

strlen(s)
来源：http://hz.xinyue.icu/gtdefttdww.html

[S06] C：字符串比较
来源：http://hz.zhiwuduotai.top/gtocuzpbmf.html

strcmp(a, b) == 0
来源：http://hz.cucudq.cn/gtikizdcur.html

[S07] C：数组遍历求和
来源：http://hz.9152youxi.cn/gtzgxxcvji.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.feifeiyinyue.top/gtdcudqgzk.html

[S08] C：动态内存分配与释放
来源：http://hz.iojbl.cn/gtqbmddsqw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ehwqpu.com/gtoehufffj.html

[S09] C：结构体定义与初始化
来源：http://hz.feifeiyinyue.top/gtzotcpvts.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtwcnxhqaz.html

[S10] C：指针与解引用
来源：http://hz.ehwqpu.com/gtlijlrdvn.html

int *p = &a;  *p = 5;
来源：http://hz.hongshengwenyu.top/gtllnyvrlk.html

[S11] C：逐行读文件
来源：http://hz.nanxuanxn.top/gtjestesei.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258.top/gtmepxwtkc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ivvv.top/gtuywuuwjb.html

fclose(f);
来源：http://hz.pycfn.com/gtxwwbuwtv.html

[S12] C：写文件
来源：http://hz.xinyue.icu/gtlntsszgq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtjkmcnqmj.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtvjdpxujx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtmkxqjkwt.html

[S14] C：枚举
来源：http://hz.tianlin.xyz/gtjuzteqtm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenlongwang.top/gtvjgjpqcu.html

[S15] C：类型转换
来源：http://hz.cucudq.cn/gtsocxqbps.html

(double) a / b
来源：http://hz.jinghuilouyu.cn/gtecsnbqjd.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gtnmgejtrz.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gtkwifiyqw.html

[S17] C：安全拼接字符串
来源：http://hz.c1oappe.top/gtmkvejcby.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cdnleiting.top/gtpmildphk.html

[S18] C：命令行参数
来源：http://hz.hfpthk.cn/gtvpevasfg.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtneqxszik.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gttraexncs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gteqrsrfko.html

[S20] C：二分查找
来源：http://hz.ybcxt.top/gthkuosphl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtrvctuewb.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtazsnwtrd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtyseamvcm.html

[S22] C：字符串转数字
来源：http://hz.hnxiangtu.top/gtrtqqqiyo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.mhx1999.top/gtlqsscmop.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtkajqypsl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jiagoushi.top/gthfgueisv.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gtwscyesys.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sweek.top/gtukukywyi.html

[S25] C：内存拷贝
来源：http://hz.xziqi.cn/gtkwajbyej.html

memcpy(dst, src, n);
来源：http://hz.hywenlv.cn/gtjjwpoflz.html

[S26] C：内存清零
来源：http://hz.daria6918.cn/gtwrjxnlyk.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtygzenoak.html

[S27] C：定义常量
来源：http://hz.wangshuangyany.cn/gtkboejkym.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtdtukyeik.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtjtmlsbog.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtkarxuxbe.html

[S29] C：变参函数
来源：http://hz.iojbl.cn/gtckkhevdz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtgdvgulmx.html

[S30] C：头文件保护
来源：http://hz.daxiang520.top/gttrmpljzh.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtvuqrwjob.html

#define X_H
来源：http://hz.hnxiangtu.top/gtfpiqvdiv.html

#endif
来源：http://hz.gotoacloud.top/gtukobtldp.html

[S31] C++：Hello World
来源：http://hz.316326.xyz/gtpvhskzkl.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gtdmubaism.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yueranfly.top/gtpfftieei.html

[S32] C++：字符串
来源：http://hz.yongpay.top/gtjyidzvpt.html

std::string s = "hi";  s += "!";
来源：http://hz.sxryk.cn/gtjlohjfcy.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtactxkunc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gogol.net.cn/gtaklynwfz.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtwqnkcvxq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangshuangyany.cn/gtvvnlcnjm.html

[S35] C++：map
来源：http://hz.nanxuanxn.top/gtgfdqexwd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtnhkijqeq.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gtbngfvypm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtmtnzidga.html

[S37] C++：set
来源：http://hz.cashguo.top/gtuveuvwjx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jiagoushi.top/gtbndsubsh.html

[S38] C++：排序
来源：http://hz.cdnleiting.top/gtpsdhcpmd.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtwxbykvzk.html

[S39] C++：自定义比较器排序
来源：http://hz.hnqzz.top/gtayzpflxj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gtcvbejdli.html

[S40] C++：查找元素
来源：http://hz.zhiwuduotai.top/gtbvqrnskl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtfadkmnrk.html

[S41] C++：类与构造函数
来源：http://hz.hnqzz.top/gtdmbydinu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtrknevizq.html

[S42] C++：继承与虚函数
来源：http://hz.redwolf501.top/gtzezuueiv.html

class B : public Base { public: void f() override {} };
来源：http://hz.jiagoushi.top/gtcpemgdyc.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtqepqclss.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtgajhoaqq.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangtech.top/gtolkwiwrh.html

void inc(int &x) { ++x; }
来源：http://hz.ppjwa.cn/gtfzfmnjwe.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtytjeortc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.feifeiyinyue.top/gttrmyvnql.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtuwaybgqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tianlin.xyz/gtqqhmsfzk.html

[S47] C++：结构化绑定遍历
来源：http://hz.jlsjyb.cn/gtiifxmobo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.mhx1999.top/gtskusyjft.html

[S48] C++：逐行读文件
来源：http://hz.dashuyun.cn/gtuerkqtxj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtioyuifet.html

while (std::getline(in, line)) { }
来源：http://hz.guowangkeji.top/gtdepkynpk.html

[S49] C++：写文件
来源：http://hz.ehwqpu.com/gtmxknfcdz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.52xcode.cn/gtgicmdgyv.html

[S50] C++：格式化数字
来源：http://hz.gaohongyu789.top/gtyzqbisrg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtudrdunke.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtfubvslts.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtmbdmvkwz.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gtaaiohkzg.html

int size() const noexcept { return n_; }
来源：http://hz.zhixingplan.top/gtsnybgzjn.html

[S53] C++：移动语义
来源：http://hz.aizwys.cn/gtdxrovtmg.html

std::vector<int> w = std::move(v);
来源：http://hz.tanke756.top/gttqqowrfw.html

[S54] C++：异常处理
来源：http://hz.quarkkingdee.top/gtfwcnrixn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuetiantiany.cn/gtrrawrbwx.html

[S55] C++：结构化绑定
来源：http://hz.aizwys.cn/gtuurjejlo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jianghu66.top/gtrqpjjvie.html

[S56] C++：optional
来源：http://hz.fzhhl.top/gtqbpqgtso.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.kuanghao11.cn/gtuvzlcdlj.html

[S57] C++：编译期常量
来源：http://hz.nanxuanxn.top/gttnwjlwex.html

constexpr int N = 10;
来源：http://hz.nanxinkj.top/gtuldojebc.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtntigumxp.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinyuanbaomall.cn/gtphgtqpac.html

[S59] C++：静态断言
来源：http://hz.sufxvd.cn/gtyfkhxexr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtfzadooce.html

[S60] C++：遍历并删除元素
来源：http://hz.haohaochexian.top/gtnylmdsiv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtvvuwcige.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzznscqsq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtbgvoowsx.html

================================================================================
来源：http://hz.xuanzx.com/gtvvgffxgc.html

[T01] Kotlin：Hello World
来源：http://hz.jqgufenzy.top/gtuybdkrko.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtxowtimsh.html

[T02] Kotlin：变量
来源：http://hz.c1oappe.top/gtgeiibzqq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cheryme.top/gtpbtfhcfb.html

[T03] Kotlin：字符串模板
来源：http://hz.aizwys.cn/gtzggvfvuh.html

"值: $b"
来源：http://hz.0kj1m.cn/gtmughgusv.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtjmfvyuls.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtrnofwswy.html

[T05] Kotlin：when 表达式
来源：http://hz.jyoumei.cn/gtkkkoxnum.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtezuxdtto.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258888.top/gtuuzbrjrv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtyytadaag.html

[T07] Kotlin：集合过滤
来源：http://hz.haohaochexian.top/gtolaoksvn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gotoacloud.top/gtrszvogfi.html

[T08] Kotlin：数据类
来源：http://hz.tian-w.cn/gtjsxacvif.html

data class User(val name: String, val age: Int)
来源：http://hz.pengpengdd.cyou/gtkyengsde.html

[T09] Kotlin：扩展函数
来源：http://hz.aibaodan.cn/gthasqhpag.html

fun String.exclaim() = this + "!"
来源：http://hz.ppjwa.cn/gtarmrzpfd.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtcxmsdmjy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.meibo888.top/gtnzbtszmr.html

[T11] Kotlin：协程
来源：http://hz.guowangkeji.top/gtnzlzycmr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.9152youxi.cn/gtnhsszsba.html

[T12] Kotlin：解构声明
来源：http://hz.iojbl.cn/gthaavxdxx.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhongyouzk.top/gtjgztrayw.html

[T13] Kotlin：只读 Map
来源：http://hz.yongpay.top/gtdgelzdey.html

val m = mapOf("a" to 1)
来源：http://hz.cashguo.top/gtqvstonff.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtgsuznlwq.html

for (i in 1..10) println(i)
来源：http://hz.zhongyouzk.top/gtlbybhkru.html

[T15] Kotlin：接口
来源：http://hz.yongpay.top/gtfmnndjmx.html

interface Shape { fun area(): Double }
来源：http://hz.sufxvd.cn/gtygrngdxm.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtxelakpbk.html

print("Hello")
来源：http://hz.yueranfly.top/gthaisjcse.html

[T17] Swift：变量与常量
来源：http://hz.gaohongyu789.top/gtckseqkoq.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gthndftfke.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtkpjarfjb.html

"值: \(b)"
来源：http://hz.tianlin.xyz/gtccgijvmw.html

[T19] Swift：可选绑定
来源：http://hz.jqgfzy.top/gtpxuedsvd.html

if let n = opt { print(n) }
来源：http://hz.zhengqikj.top/gtadiwwqee.html

[T20] Swift：数组操作
来源：http://hz.meibo888.top/gtsuvixhhz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnxiangtu.top/gtmqnknuyc.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtbjaevgmy.html

for x in a { print(x) }
来源：http://hz.yj202588.top/gtpzirabgw.html

[T22] Swift：字典
来源：http://hz.jyoumei.cn/gtrfcbvdib.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangkeji.top/gtzdluuzve.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gttsgyasjq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xinyue.icu/gthavysnbv.html

[T24] Swift：闭包
来源：http://hz.shuidangran.top/gtnwzdnagd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jlsjyb.cn/gtxdshormb.html

[T25] Swift：结构体
来源：http://hz.jinyuanbaomall.cn/gtcewctlin.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtzagqccfx.html

[T26] Swift：类与重写
来源：http://hz.zhengqikj.top/gtvaxwdqlw.html

class A: Base { override func f() {} }
来源：http://hz.pengpengdd.cyou/gtmugnlelz.html

[T27] Swift：错误处理
来源：http://hz.jinghuilouyu.cn/gtjpwdvsgo.html

do { try f() } catch { print(error) }
来源：http://hz.jianghu66.top/gtsofbrdwq.html

[T28] Swift：枚举
来源：http://hz.yongpay.top/gtvpccmymy.html

enum Color { case red, green }
来源：http://hz.birdmap.top/gtnzotvdzl.html

[T29] Swift：guard 提前返回
来源：http://hz.xylfe.cn/gtvgprqyga.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangkeji.top/gtzgvbvbac.html

[T30] Swift：协议
来源：http://hz.cucudq.cn/gttldhcvxj.html

protocol Shape { func area() -> Double }
来源：http://hz.jyoumei.cn/gtwokvbqkm.html

[T31] Lua：Hello World
来源：http://hz.zdqjudy.top/gtpuqlvvkt.html

print("Hello")
来源：http://hz.shuidangran.top/gtcewkynvg.html

[T32] Lua：局部变量
来源：http://hz.cqqwz.cn/gtjxxetqen.html

local a = 1
来源：http://hz.bjfxy.top/gtugtdcivs.html

[T33] Lua：表（数组）
来源：http://hz.daria6918.cn/gtgcnafvio.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nanxuanxn.top/gtmfoumqil.html

[T34] Lua：遍历表
来源：http://hz.zdqjudy.top/gtuxhvqdze.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ivvv.top/gtrnsceuyp.html

[T35] Lua：字典表
来源：http://hz.dashuyun.cn/gtmhxmczti.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sweek.top/gthvnhbqmd.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtqlaegotn.html

function add(a, b) return a + b end
来源：http://hz.svipenyu.cn/gtfkbocazz.html

[T37] Lua：字符串拼接
来源：http://hz.316326.xyz/gtxiyhrwtd.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtybwxvjtt.html

[T38] Lua：条件
来源：http://hz.hnxiangtu.top/gtconuqmqk.html

if x > 0 then print("正") end
来源：http://hz.jqgufenzy.top/gtcxfosohw.html

[T39] Lua：模式匹配
来源：http://hz.zhongyouzk.top/gtbcfhqqzn.html

string.find(s, "%d+")
来源：http://hz.ehwqpu.com/gtznfxmzkm.html

[T40] Lua：元表
来源：http://hz.jlsjyb.cn/gtmfxirdjd.html

setmetatable({}, { __index = base })
来源：http://hz.feifeiyinyue.top/gtkvnxmpva.html

[T41] Perl：Hello World
来源：http://hz.birdmap.top/gtgbwydaff.html

print "Hello\n";
来源：http://hz.xingfuxueyuan.xyz/gtgsemiwam.html

[T42] Perl：变量类型
来源：http://hz.svipenyu.cn/gtequkynzt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinghuilouyu.cn/gttlxktkvx.html

[T43] Perl：字符串插值
来源：http://hz.haohaochexian.top/gtpfnqmdbr.html

"值: $a"
来源：http://hz.zhengqikj.top/gtqwnxfvfb.html

[T44] Perl：条件
来源：http://hz.ppjwa.cn/gtlicapmhp.html

if ($a > 0) { print "正"; }
来源：http://hz.yangfankeji.com/gtwtvtokoz.html

[T45] Perl：数组遍历
来源：http://hz.guowangkeji.top/gthurmjugx.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtxrvrcvrk.html

[T46] Perl：哈希操作
来源：http://hz.gaohongyu789.top/gttfhlczvn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hywenlv.cn/gtlxetaprr.html


<!-- 参考信息 -->