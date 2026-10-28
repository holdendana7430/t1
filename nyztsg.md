代发 wailian999

cmd > out.log 2>&1
来源：http://hz.yanxiufei.cn/gtrhtpdxsg.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtdnjbkzzi.html

echo "log" >> out.log
来源：http://hz.jinqigufen.top/gtmzqdxnxk.html

[R41] 丢弃输出
来源：http://hz.xingfuxueyuan.xyz/gtbztfwalr.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtvxejjqzk.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gthkmdocyv.html

wc -l < a.txt
来源：http://hz.cashguo.top/gtuldwjfdh.html

[R43] 按名字查找文件
来源：http://hz.chenjidiqi.icu/gtmsakvxol.html

find . -name "*.log" -type f
来源：http://hz.shuidangran.top/gtrhwnhoey.html

[R44] 按修改时间查找
来源：http://hz.yanxiufei.cn/gtblseshuh.html

find . -mtime -7 -type f
来源：http://hz.cashguo.top/gtqtzasnuv.html

[R45] 批量删除
来源：http://hz.shanyushiyangkeji.top/gtpmlejump.html

find . -name "*.tmp" -delete
来源：http://hz.gotoacloud.top/gtcbklmdsp.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtvfitfhpj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtbazpvztx.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtlktazkma.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuetiantiany.cn/gttwumyclf.html

[R48] awk 取指定列
来源：http://hz.zycfv.cn/gtmprfdddd.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtxswfhzfi.html

[R49] awk 带条件
来源：http://hz.nanxinkj.top/gtougydwbo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cashguo.top/gtaleoscom.html

[R50] awk 求和
来源：http://hz.haohaochexian.top/gtitcmgasa.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jyoumei.cn/gtvomxvdnv.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gtasdsxgix.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aibaodan.cn/gtddgieaud.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtfjgtjepm.html

wc -l a.txt
来源：http://hz.birdmap.top/gtpslejqle.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtjlcxeuij.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tanke756.top/gtejbhbmzx.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtvwnyvbfr.html

diff a.txt b.txt
来源：http://hz.vqdsnc.cn/gtmwxpwnvb.html

[R55] 压缩与解压
来源：http://hz.cashguo.top/gttdtfuqiy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gtgffzpsrb.html

[R56] 远程拷贝
来源：http://hz.yj202588.top/gtfkphujvo.html

scp file user@host:/path/
来源：http://hz.cheryme.top/gtcqxyqzdl.html

[R57] 远程执行命令
来源：http://hz.yuanzhike.top/gteznnhkmp.html

ssh user@host 'uptime'
来源：http://hz.zhiwuduotai.top/gthvjfztzx.html

[R58] 下载文件
来源：http://hz.jianghu66.top/gtaxjpgsru.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtqlnlyxzb.html

[R59] 发 POST JSON
来源：http://hz.cheryme.top/gtgxlkvnay.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtwdrjbljz.html

[R60] 只看 HTTP 状态码
来源：http://hz.shzxlz.cn/gtlnsgrrtg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhixingplan.top/gtoxezdhcf.html

[R61] 磁盘占用
来源：http://hz.52xcode.cn/gtvhbnlxuz.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gtdsxhkhtp.html

[R62] 找最占空间的文件
来源：http://hz.hfpthk.cn/gtsnjszvuk.html

du -ah . | sort -rh | head -10
来源：http://hz.ydzc1.top/gtyvugbwxc.html

[R63] 内存与进程
来源：http://hz.hysaishi.cn/gtgqhclptw.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtgzcqgtnx.html

[R64] 结束进程
来源：http://hz.ywan-chungtsiang.top/gtkerrojve.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gzhubu.top/gtrrcpvzjj.html

[R65] 查看端口占用
来源：http://hz.sysykeji.top/gtfrxmtrzc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtxpybirvn.html

[R66] 定时任务
来源：http://hz.dashuyun.cn/gtvhkzvcrv.html

crontab -e;  crontab -l
来源：http://hz.zhoulong.xyz/gtpogmlthk.html

[R67] 生成随机十六进制串
来源：http://hz.vqdsnc.cn/gtnzyngvgh.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gtktgxxzhn.html

[R68] 计算文件校验值
来源：http://hz.zhixingplan.top/gtzqxisjmt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgufenzy.top/gtaegwsmsl.html

[R69] 生成随机密码
来源：http://hz.9152youxi.cn/gtdbjckyme.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtfmqgchda.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtkyfkdpau.html

date +%s;  date -d @1700000000
来源：http://hz.shangyingyoupin.top/gtvdgfylwn.html

[R71] 日期格式化
来源：http://hz.gzhubu.top/gtnpdzyrlw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.c1oappe.top/gtkrbaskcx.html

[R72] 等待端口就绪
来源：http://hz.cdnleiting.top/gtkursodui.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.mhx1999.top/gtwhbbctcr.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtnwmkcjyp.html

split -l 1000 big.log part_
来源：http://hz.zhixingplan.top/gttavrtsbd.html

[R74] 批量重命名
来源：http://hz.jlsjyb.cn/gtgzjzicvj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gteynksfad.html

[R75] 导出环境变量
来源：http://hz.hysaishi.cn/gtoybkybtk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gtaldsiqzy.html

[R76] 使用临时文件
来源：http://hz.meibo888.top/gteobtyeal.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtyqvvebcp.html

[R77] 读取用户输入
来源：http://hz.yangfankeji.com/gtsbspniym.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtpnussrdz.html

[R78] 交互式菜单
来源：http://hz.feifeiyinyue.top/gteyyasjmb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtqpsudyge.html

[R79] 解析命令行选项
来源：http://hz.chenjidiqi.icu/gtbwmcagqm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.kuanghao11.cn/gtcwnlghtg.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgufenzy.top/gtjckungui.html

time ./run.sh
来源：http://hz.snrcjt.cn/gtjqnbgnkw.html

================================================================================
来源：http://hz.yj202588.top/gtnbjkdfjq.html

S. C / C++ 专题
来源：http://hz.nwbrower.top/gtoxzbuxtt.html

================================================================================
来源：http://hz.yongpay.top/gtxbotugqz.html

[S01] C：Hello World
来源：http://hz.shuidangran.top/gthpkikton.html

#include <stdio.h>
来源：http://hz.yonumen.top/gttxmghtyx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gtjqujvtxe.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gthcprvmad.html

int a = 10; printf("%d\n", a);
来源：http://hz.guannengcc.top/gtgivpruag.html

[S03] C：读入整数
来源：http://hz.tianlin.xyz/gtpiadaxab.html

int x; scanf("%d", &x);
来源：http://hz.ybcxt.top/gtjaaccapr.html

[S04] C：字符串复制
来源：http://hz.sxryk.cn/gtmvygpqlc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hywenlv.cn/gtudelmxjh.html

[S05] C：字符串长度
来源：http://hz.kuanghao11.cn/gtxrpazttl.html

strlen(s)
来源：http://hz.c1oappe.top/gtpmxhjagk.html

[S06] C：字符串比较
来源：http://hz.yvedp.cn/gtqvrfntgm.html

strcmp(a, b) == 0
来源：http://hz.sysykeji.top/gtzctoyuts.html

[S07] C：数组遍历求和
来源：http://hz.ppjwa.cn/gthplaglau.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sxryk.cn/gtuuwdsvga.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtzirniqel.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tanke756.top/gtazdynoan.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtkdgdkwpn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtppwvhtjx.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gtypxgffxv.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtrotcnfzx.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtcvytlnuo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtgwvhjbvy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtbhvfwerg.html

fclose(f);
来源：http://hz.meibo888.top/gtppsflptn.html

[S12] C：写文件
来源：http://hz.smart0.xyz/gtxwdxwxql.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.svipenyu.cn/gtdcsuiihc.html

[S13] C：宏定义
来源：http://hz.zhiwuduotai.top/gtujrndaqf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cucudq.cn/gtctieanja.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gtmbepjwvw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuetiantiany.cn/gtaoiufcpz.html

[S15] C：类型转换
来源：http://hz.xylfe.cn/gtcoremnps.html

(double) a / b
来源：http://hz.quarkkingdee.top/gtxhcqqfpl.html

[S16] C：位操作置位
来源：http://hz.cashguo.top/gtcengmhou.html

x |= (1 << 3);
来源：http://hz.hywenlv.cn/gtdrrlyayz.html

[S17] C：安全拼接字符串
来源：http://hz.gzhubu.top/gtsthdcylu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.guowangkeji.top/gtsjugulns.html

[S18] C：命令行参数
来源：http://hz.pengpengdd.cyou/gtloqgicuk.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gtjqfkrptu.html

[S19] C：快速排序
来源：http://hz.yueranfly.top/gtcdyyelzo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenlongwang.top/gtpiaaykym.html

[S20] C：二分查找
来源：http://hz.sweek.top/gthazhalio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtwcypxkks.html

[S21] C：字符类别判断
来源：http://hz.wangdashe.top/gtdipiylxx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.birdmap.top/gtkzttlqbb.html

[S22] C：字符串转数字
来源：http://hz.dianchejie.cn/gtdwyrgkeq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuanzx.com/gtyqsponnl.html

[S23] C：随机数
来源：http://hz.zhijiandao.cn/gtinaaorqt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gaohongyu789.top/gtghyuijxz.html

[S24] C：获取本地时间
来源：http://hz.hfpthk.cn/gtvkvhwklm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jyoumei.cn/gtazjithkk.html

[S25] C：内存拷贝
来源：http://hz.sweek.top/gtrkjvsbpu.html

memcpy(dst, src, n);
来源：http://hz.yanxiufei.cn/gtooatdnqe.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtfpatzhrm.html

memset(a, 0, sizeof a);
来源：http://hz.gotoacloud.top/gtpsgugwjh.html

[S27] C：定义常量
来源：http://hz.tianlin.xyz/gtuwagsyfu.html

const double PI = 3.14159;
来源：http://hz.ydzc1.top/gtcdkndnqu.html

[S28] C：静态变量
来源：http://hz.shzxlz.cn/gtekhhxbfm.html

static int counter = 0;
来源：http://hz.chenjidiqi.icu/gtjeqajrbw.html

[S29] C：变参函数
来源：http://hz.smart0.xyz/gttfzmxpli.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxuanxn.top/gtbilvisxo.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtjnuzfrjh.html

#ifndef X_H
来源：http://hz.nwbrower.top/gtijpnhehx.html

#define X_H
来源：http://hz.jqgfzy.top/gtniegkgai.html

#endif
来源：http://hz.bjfxy.top/gtskxumvqd.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtiwylisjl.html

#include <iostream>
来源：http://hz.yuxming.cn/gtlnlsbemb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ybcxt.top/gtcmvlnudk.html

[S32] C++：字符串
来源：http://hz.fengsongda.top/gtolsxngyr.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gtaoocymdc.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtivyriutt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtxoyddpqy.html

[S34] C++：遍历 vector
来源：http://hz.havefunace.top/gtfkcrpwfv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.snrcjt.cn/gtlacjhssq.html

[S35] C++：map
来源：http://hz.smart0.xyz/gtyzarulpo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtayvhjthn.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtdooksqua.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtbmiemkwm.html

[S37] C++：set
来源：http://hz.yj20258.top/gtwnbothek.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yongpay.top/gtxbauuvro.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtuhgcvzgl.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgufenzy.top/gteeebpxci.html

[S39] C++：自定义比较器排序
来源：http://hz.daria6918.cn/gtmuhsukzq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinghuilouyu.cn/gturalyjfh.html

[S40] C++：查找元素
来源：http://hz.iojbl.cn/gtfbsyesbf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gtezusqnoi.html

[S41] C++：类与构造函数
来源：http://hz.yj20258.top/gtwbngzlfc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nanxinkj.top/gtnwsjnwcf.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gtaxnwjzub.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gtwfplvdjd.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gtiyxwpwjt.html

auto p = std::make_unique<int>(5);
来源：http://hz.gzhubu.top/gtmpvjlmte.html

[S44] C++：引用传参
来源：http://hz.xziqi.cn/gtxypmromp.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtxhikpfni.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gtnqbuwmly.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yangfankeji.com/gtqzsrzzwz.html

[S46] C++：函数模板
来源：http://hz.jinyuanbaomall.cn/gtdrdwicgx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.316326.xyz/gtilxettsa.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenlongwang.top/gtwfvqanhi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sysykeji.top/gtgslllojs.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtihgzawdb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hfpthk.cn/gtclsxlypr.html

while (std::getline(in, line)) { }
来源：http://hz.xingfuxueyuan.xyz/gtlpwveppg.html

[S49] C++：写文件
来源：http://hz.yj202588.top/gtcgiyxmkg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dianchejie.cn/gtqmvbbzvh.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtzccsuqjl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hongshengwenyu.top/gthcisacfa.html

[S51] C++：显式类型转换
来源：http://hz.sxryk.cn/gtezdwtihe.html

static_cast<double>(a) / b
来源：http://hz.sxryk.cn/gtnefuamyx.html

[S52] C++：const 与 noexcept
来源：http://hz.zhiwuduotai.top/gthqveqwan.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtvrzftxly.html

[S53] C++：移动语义
来源：http://hz.hnqzz.top/gtddeajlsl.html

std::vector<int> w = std::move(v);
来源：http://hz.dashuyun.cn/gtbnbihzyv.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gtjezkvzjt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gtqmvcbuil.html

[S55] C++：结构化绑定
来源：http://hz.fengsongda.top/gtznrwqxlc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gtcgdvnpqa.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtwntyyszj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtgzlsgjbr.html

[S57] C++：编译期常量
来源：http://hz.ivvv.top/gtejnlytzo.html

constexpr int N = 10;
来源：http://hz.gzhubu.top/gtuxmszatr.html

[S58] C++：命名空间
来源：http://hz.cucudq.cn/gtwvqstvuh.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtsqrvvjtv.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtlwhookfr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hywenlv.cn/gtdkphnwiq.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gtasvlfflo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258.top/gtsqltyifx.html

================================================================================
来源：http://hz.jiagoushi.top/gtfrdawwcv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gtswlvyqnv.html

================================================================================
来源：http://hz.mhx1999.top/gtmdlyqxgo.html

[T01] Kotlin：Hello World
来源：http://hz.gogol.net.cn/gtnlrwjpgc.html

println("Hello")
来源：http://hz.gotoacloud.top/gtkprjdkcw.html

[T02] Kotlin：变量
来源：http://hz.ppjwa.cn/gtfsevixvk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtfvkphpgr.html

[T03] Kotlin：字符串模板
来源：http://hz.ivvv.top/gtfmuragcb.html

"值: $b"
来源：http://hz.shangyingyoupin.top/gtznsfhjqp.html

[T04] Kotlin：空安全
来源：http://hz.haohaochexian.top/gtvvxbyurb.html

val n: String? = null;  n?.length
来源：http://hz.haohaochexian.top/gtnzdfbwwg.html

[T05] Kotlin：when 表达式
来源：http://hz.gaohongyu789.top/gteqsqpifw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hammf.cn/gtrazfzozz.html

[T06] Kotlin：集合映射
来源：http://hz.xziqi.cn/gtkbqcbcjq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtqhslxqae.html

[T07] Kotlin：集合过滤
来源：http://hz.ybcxt.top/gtouxyepfd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zdqjudy.top/gtckkgnhbf.html

[T08] Kotlin：数据类
来源：http://hz.gzhubu.top/gtecsihexg.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gtlhmzehki.html

[T09] Kotlin：扩展函数
来源：http://hz.vqdsnc.cn/gtradyzcle.html

fun String.exclaim() = this + "!"
来源：http://hz.meibo888.top/gtxtjzcdas.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gtvltzvqex.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gotoacloud.top/gtyydpptue.html

[T11] Kotlin：协程
来源：http://hz.wangdashe.top/gtdhhvvywd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhongyouzk.top/gtiqgmqcjj.html

[T12] Kotlin：解构声明
来源：http://hz.jqgfzy.top/gtlavjurjv.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtkxstcuap.html

[T13] Kotlin：只读 Map
来源：http://hz.yuanzhike.top/gtixaolggk.html

val m = mapOf("a" to 1)
来源：http://hz.shuidangran.top/gtahfnopro.html

[T14] Kotlin：循环
来源：http://hz.yvedp.cn/gtlztqskns.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtmofcholk.html

[T15] Kotlin：接口
来源：http://hz.nanxuanxn.top/gtbjjeudpq.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtutumrfqs.html

[T16] Swift：Hello World
来源：http://hz.sxryk.cn/gtukofqilm.html

print("Hello")
来源：http://hz.svipenyu.cn/gtfxxfayxy.html

[T17] Swift：变量与常量
来源：http://hz.svipenyu.cn/gtsvpdnydd.html

var a = 1;  let b = 2
来源：http://hz.cheryme.top/gtyughzhcz.html

[T18] Swift：字符串插值
来源：http://hz.mhx1999.top/gtvuzynsjw.html

"值: \(b)"
来源：http://hz.svipenyu.cn/gtwtyipluf.html

[T19] Swift：可选绑定
来源：http://hz.hywenlv.cn/gtxumbotya.html

if let n = opt { print(n) }
来源：http://hz.nanxinkj.top/gtbtrsifoe.html

[T20] Swift：数组操作
来源：http://hz.sweek.top/gtnvrbiaba.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hysaishi.cn/gthynkkalz.html

[T21] Swift：遍历
来源：http://hz.zhixingplan.top/gtoedqxrlf.html

for x in a { print(x) }
来源：http://hz.yj20258888.top/gtazznanxc.html

[T22] Swift：字典
来源：http://hz.pycfn.com/gtazrvotgz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gtzekucrwp.html

[T23] Swift：函数
来源：http://hz.jinyuanbaomall.cn/gtciqvwlns.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tian-w.cn/gtcugyanny.html

[T24] Swift：闭包
来源：http://hz.ywan-chungtsiang.top/gtojpgvvid.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tanke756.top/gtxasozjsr.html

[T25] Swift：结构体
来源：http://hz.xingfuxueyuan.xyz/gtgtzuijcp.html

struct P { var x: Int }
来源：http://hz.0kj1m.cn/gtmfuriieq.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtvtjuukew.html

class A: Base { override func f() {} }
来源：http://hz.hnqzz.top/gtfsjdzmzc.html

[T27] Swift：错误处理
来源：http://hz.nwbrower.top/gtxuxewpna.html

do { try f() } catch { print(error) }
来源：http://hz.hnxiangtu.top/gtjjqikoaf.html

[T28] Swift：枚举
来源：http://hz.zdqjudy.top/gtwszkwzja.html

enum Color { case red, green }
来源：http://hz.zhixingplan.top/gtnirpcgnb.html

[T29] Swift：guard 提前返回
来源：http://hz.aizwys.cn/gtxtlvlhmi.html

guard let x = opt else { return }
来源：http://hz.shangyingyoupin.top/gtmcjqncmd.html

[T30] Swift：协议
来源：http://hz.meibo888.top/gtgkeudbxo.html

protocol Shape { func area() -> Double }
来源：http://hz.daria6918.cn/gtxmlzcroa.html

[T31] Lua：Hello World
来源：http://hz.sweek.top/gtghwlybwh.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gtntzhzdyf.html

[T32] Lua：局部变量
来源：http://hz.fengsongda.top/gtczmcsddi.html

local a = 1
来源：http://hz.gaohongyu789.top/gtdqpkecyp.html

[T33] Lua：表（数组）
来源：http://hz.gzhubu.top/gtgjafcezj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.pycfn.com/gtmnsmksqz.html

[T34] Lua：遍历表
来源：http://hz.aizwys.cn/gtrecmywkl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.c1oappe.top/gtmzictwzr.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtscfiwyvw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fengsongda.top/gtfioisfcr.html

[T36] Lua：函数
来源：http://hz.zhongyouzk.top/gtfpuedsqy.html

function add(a, b) return a + b end
来源：http://hz.hfpthk.cn/gtukqhcsmu.html

[T37] Lua：字符串拼接
来源：http://hz.zhoulong.xyz/gtnvjpzifk.html

"a" .. "b"
来源：http://hz.ppjwa.cn/gtxfqfqeqy.html

[T38] Lua：条件
来源：http://hz.nwbrower.top/gtnzpnxbpv.html

if x > 0 then print("正") end
来源：http://hz.sysykeji.top/gtlrvyhjvo.html

[T39] Lua：模式匹配
来源：http://hz.birdmap.top/gtrkxzdesk.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangtech.top/gtfiajjjzm.html

[T40] Lua：元表
来源：http://hz.c1oappe.top/gtpprrpicy.html

setmetatable({}, { __index = base })
来源：http://hz.xuetiantiany.cn/gtvorljvai.html

[T41] Perl：Hello World
来源：http://hz.cqqwz.cn/gtgpjovvpu.html

print "Hello\n";
来源：http://hz.hammf.cn/gtfmppazyi.html

[T42] Perl：变量类型
来源：http://hz.cucudq.cn/gtzyuscllg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shzxlz.cn/gtjvquqyld.html


<!-- 参考信息 -->