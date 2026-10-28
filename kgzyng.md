代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.havefunace.top/gtoiahvwpw.html

[R46] 递归替换文件内容
来源：http://hz.yuxming.cn/gtptsiefsn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhijiandao.cn/gtxavdkpwi.html

[R47] sed 单行替换
来源：http://hz.cheryme.top/gtlkdzwtva.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtwyaybshm.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gtddrcjugh.html

awk '{print $1, $3}' a.txt
来源：http://hz.gzhubu.top/gtornigswg.html

[R49] awk 带条件
来源：http://hz.hammf.cn/gtqfjuujua.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhoulong.xyz/gtjnmopcln.html

[R50] awk 求和
来源：http://hz.zdqjudy.top/gtxttahjty.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtbvyrgsql.html

[R51] 排序去重取前几
来源：http://hz.bjfxy.top/gtedynwovw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sysykeji.top/gtguhfawiq.html

[R52] 统计行数
来源：http://hz.9152youxi.cn/gtfaxakomy.html

wc -l a.txt
来源：http://hz.xuetiantiany.cn/gteweopwht.html

[R53] 查看文件头与实时尾
来源：http://hz.pengpengdd.cyou/gthdmtrmpw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.guowangkeji.top/gtzooodmvi.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gtmgozxvkz.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gthgmiztmi.html

[R55] 压缩与解压
来源：http://hz.wangdashe.top/gtjcdghdzv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgfzy.top/gtwphymgqq.html

[R56] 远程拷贝
来源：http://hz.meibo888.top/gtotcfiltg.html

scp file user@host:/path/
来源：http://hz.yanxiufei.cn/gtonmaqpss.html

[R57] 远程执行命令
来源：http://hz.jqgufenzy.top/gtctqdvimk.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtrvxmdcgr.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtnixssrwu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinyuanbaomall.cn/gtljpycduu.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtlfgalqhn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydjk.org.cn/gtozljpkfs.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtfuycbhaq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtcwvdvyal.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gtdwywtyoo.html

df -h;  du -sh *
来源：http://hz.316326.xyz/gtbwsfkwdh.html

[R62] 找最占空间的文件
来源：http://hz.yongpay.top/gtwfanpxbe.html

du -ah . | sort -rh | head -10
来源：http://hz.zhengqikj.top/gtzexpxkqe.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtruvqicgi.html

free -h;  ps aux | grep nginx
来源：http://hz.xuanzx.com/gtxurruqaj.html

[R64] 结束进程
来源：http://hz.hywenlv.cn/gttbdwasrp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtpqqicahq.html

[R65] 查看端口占用
来源：http://hz.zhongyouzk.top/gtrysntumf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fengsongda.top/gtzaosvomk.html

[R66] 定时任务
来源：http://hz.ehwqpu.com/gtsdhnfzje.html

crontab -e;  crontab -l
来源：http://hz.ivvv.top/gtnrqpudhm.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtjwuxujkd.html

openssl rand -hex 16
来源：http://hz.gogol.net.cn/gtfikujzft.html

[R68] 计算文件校验值
来源：http://hz.gogol.net.cn/gtaciaqihu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aibaodan.cn/gtcdpiblht.html

[R69] 生成随机密码
来源：http://hz.yuxming.cn/gtwfygtkwp.html

head -c 16 /dev/urandom | base64
来源：http://hz.ppjwa.cn/gtnvmqsyxx.html

[R70] 时间戳与互转
来源：http://hz.zhoulong.xyz/gtjsrtmzod.html

date +%s;  date -d @1700000000
来源：http://hz.yuanzhike.top/gtohyffdws.html

[R71] 日期格式化
来源：http://hz.tianlin.xyz/gtezpiynqv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.iojbl.cn/gtfigezcxy.html

[R72] 等待端口就绪
来源：http://hz.svipenyu.cn/gtebguujhb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhixingplan.top/gtygtpgnni.html

[R73] 分割大日志
来源：http://hz.0kj1m.cn/gtpumvrksd.html

split -l 1000 big.log part_
来源：http://hz.zhongyouzk.top/gtfwsodjpx.html

[R74] 批量重命名
来源：http://hz.shanyushiyangtech.top/gtkzmbmqvo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtjhnbzvml.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gteiwoegpr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hfpthk.cn/gttehegnyv.html

[R76] 使用临时文件
来源：http://hz.daxiang520.top/gtwahghdxn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtiubgihbj.html

[R77] 读取用户输入
来源：http://hz.jinghuilouyu.cn/gtjhpvfsmf.html

read -rp "请输入: " ans
来源：http://hz.iojbl.cn/gtqxlzcyen.html

[R78] 交互式菜单
来源：http://hz.kuanghao11.cn/gteuxodwyd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yangfankeji.com/gtvhyoagbm.html

[R79] 解析命令行选项
来源：http://hz.snrcjt.cn/gtsreecnzm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gtvtbagcqv.html

[R80] 查看脚本执行耗时
来源：http://hz.gotoacloud.top/gtaibigqbr.html

time ./run.sh
来源：http://hz.mhx1999.top/gttyxaqbtb.html

================================================================================
来源：http://hz.redwolf501.top/gtuaghdabl.html

S. C / C++ 专题
来源：http://hz.zhijiandao.cn/gtjnyhqkyh.html

================================================================================
来源：http://hz.jinqigufen.top/gtsytmlldt.html

[S01] C：Hello World
来源：http://hz.c1oappe.top/gthpzrzcfd.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gtujvixrdf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.mhx1999.top/gtdtglpnol.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gtyfsyhpze.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtgskvakgk.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gtoibpranx.html

int x; scanf("%d", &x);
来源：http://hz.hnxiangtu.top/gtvctqlzqq.html

[S04] C：字符串复制
来源：http://hz.aizwys.cn/gtkmwmothl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xuanzx.com/gtjkbkdsdm.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtminxikqs.html

strlen(s)
来源：http://hz.fzhhl.top/gtifnpymhd.html

[S06] C：字符串比较
来源：http://hz.iojbl.cn/gtqngyjrsr.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtcxxvkjpa.html

[S07] C：数组遍历求和
来源：http://hz.zhixingplan.top/gttqnbypqr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yuxming.cn/gtuzvptzsi.html

[S08] C：动态内存分配与释放
来源：http://hz.pycfn.com/gtadsndcfh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.svipenyu.cn/gtxpchwook.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtvnspkjgy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.vqdsnc.cn/gtvfrfenuw.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtchcntjpp.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtdfsnkurm.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtdocjbxav.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hywenlv.cn/gtnohhqqka.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sufxvd.cn/gttbhruqdo.html

fclose(f);
来源：http://hz.jinghuilouyu.cn/gtemefeziv.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtkhurbksx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shangyingyoupin.top/gtcqdeullk.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtxywyjucu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.316326.xyz/gtpcvwdtlh.html

[S14] C：枚举
来源：http://hz.ppjwa.cn/gtkthabgeo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtptorlmhe.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtrvrvzthv.html

(double) a / b
来源：http://hz.yanxiufei.cn/gtfpkuyiho.html

[S16] C：位操作置位
来源：http://hz.xylfe.cn/gtbvjjymxs.html

x |= (1 << 3);
来源：http://hz.wangshuangyany.cn/gtnzqiryko.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtfyoklxwg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gtzmirtwfn.html

[S18] C：命令行参数
来源：http://hz.hnqzz.top/gtsfnlttiz.html

int main(int argc, char **argv)
来源：http://hz.ydjk.org.cn/gtubvkfcdp.html

[S19] C：快速排序
来源：http://hz.zhijiandao.cn/gtksyuusjq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtknjfquyk.html

[S20] C：二分查找
来源：http://hz.tianlin.xyz/gtbqlnyakc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtjsqqfbgg.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtevuwsjff.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtdgxbsxkr.html

[S22] C：字符串转数字
来源：http://hz.zhoulong.xyz/gtvobpaoea.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.52xcode.cn/gtnlfhhqpz.html

[S23] C：随机数
来源：http://hz.yueranfly.top/gteeorjohj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtqpnvxxlo.html

[S24] C：获取本地时间
来源：http://hz.pengpengdd.cyou/gtsubpcsfn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yonumen.top/gtqamtfoxt.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtbmpdnobh.html

memcpy(dst, src, n);
来源：http://hz.jinqigufen.top/gtgwzirwtr.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtexiqccig.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gtlqjkzpxu.html

[S27] C：定义常量
来源：http://hz.cashguo.top/gtyppupdiy.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtzphaiwco.html

[S28] C：静态变量
来源：http://hz.yangfankeji.com/gtvddebxlk.html

static int counter = 0;
来源：http://hz.mhx1999.top/gtxpbwhtxp.html

[S29] C：变参函数
来源：http://hz.dianchejie.cn/gtzobibltu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtzjxuerbh.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gtwlbpvjgx.html

#ifndef X_H
来源：http://hz.ybcxt.top/gtxlocmuuq.html

#define X_H
来源：http://hz.xylfe.cn/gtkufgvzfu.html

#endif
来源：http://hz.52xcode.cn/gtwwkbrehu.html

[S31] C++：Hello World
来源：http://hz.havefunace.top/gtzngsbikn.html

#include <iostream>
来源：http://hz.yuanzhike.top/gtazetfoqk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dianchejie.cn/gtpkyynqov.html

[S32] C++：字符串
来源：http://hz.redwolf501.top/gtcwskmmvv.html

std::string s = "hi";  s += "!";
来源：http://hz.zhaomingkeji.xyz/gtxdyyngig.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtyvkhydda.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ywan-chungtsiang.top/gtpijdvpnc.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtkicjzlcl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gttfcicsbw.html

[S35] C++：map
来源：http://hz.jqgufenzy.top/gtlimgwaxp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtdgcxgbhs.html

[S36] C++：unordered_map
来源：http://hz.yj20258.top/gtptrfaies.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtmbfjlzdj.html

[S37] C++：set
来源：http://hz.zhijiandao.cn/gtudrvuwqb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tanke756.top/gtvxryvtqp.html

[S38] C++：排序
来源：http://hz.shuidangran.top/gtmijqbyug.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtljtjbhrw.html

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtbuohmowr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hongshengwenyu.top/gtlwgdncxb.html

[S40] C++：查找元素
来源：http://hz.jianghu66.top/gtaeiwzuml.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gtagrldryp.html

[S41] C++：类与构造函数
来源：http://hz.gogol.net.cn/gthmvessij.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gtnyodcass.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtzaqyoypf.html

class B : public Base { public: void f() override {} };
来源：http://hz.yangfankeji.com/gtpixkjbtl.html

[S43] C++：智能指针
来源：http://hz.snrcjt.cn/gthsajqrax.html

auto p = std::make_unique<int>(5);
来源：http://hz.yvedp.cn/gtyzriwphz.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtxerrcjyr.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtioxrltni.html

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gtpijwifuf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.52xcode.cn/gtabajelsc.html

[S46] C++：函数模板
来源：http://hz.ybcxt.top/gtvvnlcrng.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shzxlz.cn/gtydxjrdwb.html

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtmmiiheni.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gtzvjyfxbh.html

[S48] C++：逐行读文件
来源：http://hz.yongpay.top/gtfalplitu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxuanxn.top/gtytfohpbv.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtffzuttzo.html

[S49] C++：写文件
来源：http://hz.chenlongwang.top/gteundwndn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gthyxwwfdo.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gtpbwngbkx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.redwolf501.top/gtzdvtumuu.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtwufyxcnt.html

static_cast<double>(a) / b
来源：http://hz.cqqwz.cn/gtmucwtivl.html

[S52] C++：const 与 noexcept
来源：http://hz.zhijiandao.cn/gtcibhdhbw.html

int size() const noexcept { return n_; }
来源：http://hz.vqdsnc.cn/gtgnojpzfr.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtcrvxqeix.html

std::vector<int> w = std::move(v);
来源：http://hz.kuanghao11.cn/gthzzgfhit.html

[S54] C++：异常处理
来源：http://hz.dashuyun.cn/gtwgvfdhkk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hongshengwenyu.top/gtlrqsaqhd.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtqxvisiut.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtywobjxtn.html

[S56] C++：optional
来源：http://hz.daxiang520.top/gtnxxswhui.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gtlmipaiwe.html

[S57] C++：编译期常量
来源：http://hz.tianlin.xyz/gtanlpkdwg.html

constexpr int N = 10;
来源：http://hz.pengpengdd.cyou/gtjvdpandx.html

[S58] C++：命名空间
来源：http://hz.yueranfly.top/gtjmfydohi.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangkeji.top/gtybuplaow.html

[S59] C++：静态断言
来源：http://hz.ybcxt.top/gtdxgecvic.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtrmaivhfg.html

[S60] C++：遍历并删除元素
来源：http://hz.yuanzhike.top/gtxhudioux.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtzdrsiyhf.html

================================================================================
来源：http://hz.fzhhl.top/gtevfygdsb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtxgjedgdk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbelkbvvt.html

[T01] Kotlin：Hello World
来源：http://hz.nwbrower.top/gtndgyfzrs.html

println("Hello")
来源：http://hz.hysaishi.cn/gtbwjddhie.html

[T02] Kotlin：变量
来源：http://hz.smart0.xyz/gtvgjuazoe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.mhx1999.top/gtkybtsizn.html

[T03] Kotlin：字符串模板
来源：http://hz.jiagoushi.top/gtdrgrzcsg.html

"值: $b"
来源：http://hz.9152youxi.cn/gtpcgdfnwy.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gtallyyuas.html

val n: String? = null;  n?.length
来源：http://hz.hammf.cn/gtmqldprgh.html

[T05] Kotlin：when 表达式
来源：http://hz.gotoacloud.top/gtlsiulxfq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.9152youxi.cn/gtncxtpynq.html

[T06] Kotlin：集合映射
来源：http://hz.aibaodan.cn/gtagudlcfj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.kuanghao11.cn/gtzalnivpe.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtxldimxkx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangtech.top/gtvyvdlymz.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtsggblgrn.html

data class User(val name: String, val age: Int)
来源：http://hz.tanke756.top/gtatcayncu.html

[T09] Kotlin：扩展函数
来源：http://hz.xingfuxueyuan.xyz/gtyyovlulf.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtjiggmibu.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtmchrbpba.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtmowwybtp.html

[T11] Kotlin：协程
来源：http://hz.sweek.top/gtjpfajvuc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenlongwang.top/gtzuxnvesi.html

[T12] Kotlin：解构声明
来源：http://hz.zhengqikj.top/gtfvcisdou.html

val (a, b) = Pair(1, 2)
来源：http://hz.cheryme.top/gtkfwlcdao.html

[T13] Kotlin：只读 Map
来源：http://hz.shanyushiyangkeji.top/gtpmoyfupg.html

val m = mapOf("a" to 1)
来源：http://hz.jianghu66.top/gtpmvizmax.html

[T14] Kotlin：循环
来源：http://hz.quarkkingdee.top/gtzvbpsdbo.html

for (i in 1..10) println(i)
来源：http://hz.nwbrower.top/gtuhmdxres.html

[T15] Kotlin：接口
来源：http://hz.hongshengwenyu.top/gtmeiwonrz.html

interface Shape { fun area(): Double }
来源：http://hz.zhijiandao.cn/gtpexybqtw.html

[T16] Swift：Hello World
来源：http://hz.sweek.top/gthacvvwtb.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtmyfnjbij.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gtlsiaqphr.html

var a = 1;  let b = 2
来源：http://hz.ivvv.top/gtfhkczaex.html

[T18] Swift：字符串插值
来源：http://hz.cqqwz.cn/gtpxcpybhx.html

"值: \(b)"
来源：http://hz.wangdashe.top/gtacidmjpe.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtnhlgygoh.html

if let n = opt { print(n) }
来源：http://hz.yj20258.top/gtmjiqxhpg.html

[T20] Swift：数组操作
来源：http://hz.0kj1m.cn/gtipzpghpb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yanxiufei.cn/gtixromupc.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtltrmwhmt.html

for x in a { print(x) }
来源：http://hz.zhongyouzk.top/gtaemfokst.html

[T22] Swift：字典
来源：http://hz.guowangkeji.top/gtesnhlxja.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shuidangran.top/gtqameuhke.html

[T23] Swift：函数
来源：http://hz.xuanzx.com/gtlnzcozkx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sxryk.cn/gtyqghehxm.html

[T24] Swift：闭包
来源：http://hz.aibaodan.cn/gtiviivdjp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guowangkeji.top/gtwvieknxy.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtqplbrslr.html

struct P { var x: Int }
来源：http://hz.ybcxt.top/gtnjzlynbu.html

[T26] Swift：类与重写
来源：http://hz.sweek.top/gtwhhrhscr.html

class A: Base { override func f() {} }
来源：http://hz.yj202588.top/gtovqmagyr.html

[T27] Swift：错误处理
来源：http://hz.andypj.xyz/gtpfryosyi.html

do { try f() } catch { print(error) }
来源：http://hz.hywenlv.cn/gtcmzhaykz.html

[T28] Swift：枚举
来源：http://hz.jiagoushi.top/gteajqsvdy.html

enum Color { case red, green }
来源：http://hz.shanyushiyangtech.top/gtwracireu.html

[T29] Swift：guard 提前返回
来源：http://hz.haohaochexian.top/gtavevsqel.html

guard let x = opt else { return }
来源：http://hz.cashguo.top/gtaauxhvmx.html

[T30] Swift：协议
来源：http://hz.chenlongwang.top/gtvoiczkhz.html

protocol Shape { func area() -> Double }
来源：http://hz.hywenlv.cn/gtnynvkbmg.html

[T31] Lua：Hello World
来源：http://hz.yj202588.top/gtmkoggjda.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtmfjrukso.html

[T32] Lua：局部变量
来源：http://hz.hnxiangtu.top/gtwxzeggaf.html

local a = 1
来源：http://hz.hongshengwenyu.top/gtigknrjcn.html

[T33] Lua：表（数组）
来源：http://hz.hnxiangtu.top/gtmjgnocbr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.chenzaomai.com/gtpiwylich.html

[T34] Lua：遍历表
来源：http://hz.jlsjyb.cn/gtalmksdae.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xuanzx.com/gthwbttdup.html

[T35] Lua：字典表
来源：http://hz.52xcode.cn/gtoaclfaux.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hfpthk.cn/gtxybrlitd.html

[T36] Lua：函数
来源：http://hz.wangshuangyany.cn/gtrhhbcwub.html

function add(a, b) return a + b end
来源：http://hz.hongshengwenyu.top/gtdxgowevd.html

[T37] Lua：字符串拼接
来源：http://hz.yueranfly.top/gtgdwwourg.html

"a" .. "b"
来源：http://hz.quarkkingdee.top/gtvybytgtc.html

[T38] Lua：条件
来源：http://hz.xingfuxueyuan.xyz/gtbfyiffem.html

if x > 0 then print("正") end
来源：http://hz.gogol.net.cn/gtixslddmk.html

[T39] Lua：模式匹配
来源：http://hz.shangyingyoupin.top/gtrurjjcge.html

string.find(s, "%d+")
来源：http://hz.yj20258888.top/gtbzmrhuvu.html

[T40] Lua：元表
来源：http://hz.sxryk.cn/gtxsexvroj.html

setmetatable({}, { __index = base })
来源：http://hz.nanxuanxn.top/gtabijgosu.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtmkplnejr.html

print "Hello\n";
来源：http://hz.havefunace.top/gtvxqjgnmh.html

[T42] Perl：变量类型
来源：http://hz.sysykeji.top/gtfhzayran.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.svipenyu.cn/gtgvdivlmk.html

[T43] Perl：字符串插值
来源：http://hz.ybcxt.top/gtojbggdic.html

"值: $a"
来源：http://hz.bjfxy.top/gtzxbewgdb.html

[T44] Perl：条件
来源：http://hz.fzhhl.top/gtpeizkzda.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtbeqhchwo.html

[T45] Perl：数组遍历
来源：http://hz.sufxvd.cn/gtxxxjrvbb.html

for my $x (@arr) { print $x; }
来源：http://hz.9152youxi.cn/gtglblpfeq.html

[T46] Perl：哈希操作
来源：http://hz.9152youxi.cn/gtfhnuzxak.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hfpthk.cn/gtfbpuokfk.html

[T47] Perl：正则捕获
来源：http://hz.yuanzhike.top/gtkvgnuhpo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yonumen.top/gtjisbuuri.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtnizpcqou.html

$s =~ s/old/new/g;
来源：http://hz.yonumen.top/gtfombddiq.html


<!-- 参考信息 -->