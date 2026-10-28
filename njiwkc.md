代发 wailian999

find . -name "*.log" -type f
来源：http://hz.hongshengwenyu.top/gtfolnkdnv.html

[R44] 按修改时间查找
来源：http://hz.tian-w.cn/gtbfoudgou.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtslohooho.html

[R45] 批量删除
来源：http://hz.hammf.cn/gtfhzrzcos.html

find . -name "*.tmp" -delete
来源：http://hz.gzhubu.top/gtbewrdtxz.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gtpdcvsuou.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydzc1.top/gtifnqoaju.html

[R47] sed 单行替换
来源：http://hz.birdmap.top/gtsfzxwhvd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtvnxyxcky.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gtuaucdaaz.html

awk '{print $1, $3}' a.txt
来源：http://hz.tian-w.cn/gtyeqqngdb.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtuqyehnuv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hysaishi.cn/gturkwrrad.html

[R50] awk 求和
来源：http://hz.nanxinkj.top/gtktklptyb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgfzy.top/gtagdgpuac.html

[R51] 排序去重取前几
来源：http://hz.dashuyun.cn/gtopwkqrli.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtjnwegivl.html

[R52] 统计行数
来源：http://hz.jyoumei.cn/gtxkkpgmoz.html

wc -l a.txt
来源：http://hz.jlsjyb.cn/gtinvlvqkd.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtooqrwsvv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hywenlv.cn/gtuiqzcsvc.html

[R54] 比较两个文件
来源：http://hz.nanxuanxn.top/gtgbquzuhu.html

diff a.txt b.txt
来源：http://hz.sweek.top/gtfvewlcwl.html

[R55] 压缩与解压
来源：http://hz.guowangkeji.top/gtjpctcywi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yongpay.top/gtaijcndhd.html

[R56] 远程拷贝
来源：http://hz.daria6918.cn/gtuyfhudcv.html

scp file user@host:/path/
来源：http://hz.yuxming.cn/gtddzymlcb.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtzeekumcz.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtkgsgetdq.html

[R58] 下载文件
来源：http://hz.quarkkingdee.top/gtkwnimemo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydzc1.top/gtzozjqhqo.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtmbygwynv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnxiangtu.top/gtqdbyhcuo.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gtdnpbzxnz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtstjilxup.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gtokwzjmbf.html

df -h;  du -sh *
来源：http://hz.xziqi.cn/gtuffjcsow.html

[R62] 找最占空间的文件
来源：http://hz.fzhhl.top/gttyzhfsdt.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtwadjvzpd.html

[R63] 内存与进程
来源：http://hz.jianghu66.top/gtgqdmsuck.html

free -h;  ps aux | grep nginx
来源：http://hz.hywenlv.cn/gtokuxehgx.html

[R64] 结束进程
来源：http://hz.hnxiangtu.top/gttlcexccq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinghuilouyu.cn/gtdpesrhji.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gttrwdpzyo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yonumen.top/gttnbxrkfp.html

[R66] 定时任务
来源：http://hz.zdqjudy.top/gtxeiczmtd.html

crontab -e;  crontab -l
来源：http://hz.andypj.xyz/gtcwdymswn.html

[R67] 生成随机十六进制串
来源：http://hz.quarkkingdee.top/gtbjrjeqxr.html

openssl rand -hex 16
来源：http://hz.chenlongwang.top/gteykvdszt.html

[R68] 计算文件校验值
来源：http://hz.yanxiufei.cn/gteameylra.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jianghu66.top/gtyngsswsh.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtcihnkgxc.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhixingplan.top/gtgegaeaku.html

[R70] 时间戳与互转
来源：http://hz.yueranfly.top/gtqiugbppt.html

date +%s;  date -d @1700000000
来源：http://hz.nwbrower.top/gtgdvlsqah.html

[R71] 日期格式化
来源：http://hz.ivvv.top/gtipsvtest.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xziqi.cn/gtwkzabxtk.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gthivahvcm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.bjfxy.top/gtjeykaaqf.html

[R73] 分割大日志
来源：http://hz.zdqjudy.top/gtquahplul.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gthncpokik.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gtunvwipcz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtjozhuiir.html

[R75] 导出环境变量
来源：http://hz.hnxiangtu.top/gtpyobftev.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.birdmap.top/gttrocjwsz.html

[R76] 使用临时文件
来源：http://hz.vqdsnc.cn/gtnpqjvsvh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gttnfhbzvf.html

[R77] 读取用户输入
来源：http://hz.hnxiangtu.top/gtpzkcostw.html

read -rp "请输入: " ans
来源：http://hz.pengpengdd.cyou/gtilsnhdhr.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtwgychvho.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.andypj.xyz/gtbyvhicye.html

[R79] 解析命令行选项
来源：http://hz.sysykeji.top/gtnyzzyayi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gthlanvoim.html

[R80] 查看脚本执行耗时
来源：http://hz.cashguo.top/gtutxcryxa.html

time ./run.sh
来源：http://hz.zycfv.cn/gtvzyjsqyr.html

================================================================================
来源：http://hz.tanke756.top/gtvmfcqmxb.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtfibcvwwf.html

================================================================================
来源：http://hz.redwolf501.top/gtmrssywkq.html

[S01] C：Hello World
来源：http://hz.xylfe.cn/gtozmqrtmm.html

#include <stdio.h>
来源：http://hz.zhongyouzk.top/gtgisdafcf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtljkvpxfm.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtfkpxovtw.html

int a = 10; printf("%d\n", a);
来源：http://hz.daria6918.cn/gtzhndkvup.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtseptcbui.html

int x; scanf("%d", &x);
来源：http://hz.hnxiangtu.top/gtprkrvbre.html

[S04] C：字符串复制
来源：http://hz.jinghuilouyu.cn/gtufowulmv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gtejlbyatd.html

[S05] C：字符串长度
来源：http://hz.52xcode.cn/gtzvopwoit.html

strlen(s)
来源：http://hz.chenjidiqi.icu/gtgnvamuzk.html

[S06] C：字符串比较
来源：http://hz.xuanzx.com/gtojogdcuo.html

strcmp(a, b) == 0
来源：http://hz.zhaomingkeji.xyz/gteglftsyz.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gtzhlrpelw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gttvdtklej.html

[S08] C：动态内存分配与释放
来源：http://hz.meibo888.top/gtszdwtcge.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sweek.top/gtebjnvhqv.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtauouylui.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.svipenyu.cn/gtenjxisdc.html

[S10] C：指针与解引用
来源：http://hz.9152youxi.cn/gtpxgisafv.html

int *p = &a;  *p = 5;
来源：http://hz.tian-w.cn/gtnqufjyxc.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtlnbmyxiy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.52xcode.cn/gtwsadozfb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtdrtshiqe.html

fclose(f);
来源：http://hz.smart0.xyz/gtxsubtunq.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gtqoombasw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gtutsuojxu.html

[S13] C：宏定义
来源：http://hz.haohaochexian.top/gtfwdvohvi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangdashe.top/gtaepburdz.html

[S14] C：枚举
来源：http://hz.ppjwa.cn/gtunjzttir.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.haohaochexian.top/gtuvuhurfv.html

[S15] C：类型转换
来源：http://hz.ppjwa.cn/gtryqgwhzb.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtgjcwxjjf.html

[S16] C：位操作置位
来源：http://hz.zhoulong.xyz/gtpjpazhim.html

x |= (1 << 3);
来源：http://hz.svipenyu.cn/gtzblpmkhp.html

[S17] C：安全拼接字符串
来源：http://hz.aizwys.cn/gtowddtkpw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.svipenyu.cn/gtphkymazc.html

[S18] C：命令行参数
来源：http://hz.daxiang520.top/gtstefyotb.html

int main(int argc, char **argv)
来源：http://hz.sweek.top/gtylhxazup.html

[S19] C：快速排序
来源：http://hz.ybcxt.top/gtynjzjbxo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gthngsyisc.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtisvvyeff.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtbuhpmyrm.html

[S21] C：字符类别判断
来源：http://hz.ehwqpu.com/gtdrfypywo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jianghu66.top/gttsmqeqja.html

[S22] C：字符串转数字
来源：http://hz.iojbl.cn/gtaurrybqa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gtbesmehgn.html

[S23] C：随机数
来源：http://hz.gotoacloud.top/gtarckuhhf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cheryme.top/gtbffijizq.html

[S24] C：获取本地时间
来源：http://hz.xuanzx.com/gtmcznfiia.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gttbgypddy.html

[S25] C：内存拷贝
来源：http://hz.zhoulong.xyz/gtaddjyruf.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtgqjjaidu.html

[S26] C：内存清零
来源：http://hz.pengpengdd.cyou/gtuvmwhzit.html

memset(a, 0, sizeof a);
来源：http://hz.hfpthk.cn/gtvcyudgcu.html

[S27] C：定义常量
来源：http://hz.xuanzx.com/gtakndraap.html

const double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtcuojtnuq.html

[S28] C：静态变量
来源：http://hz.hywenlv.cn/gtpfbopjyp.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gtlbdnggfy.html

[S29] C：变参函数
来源：http://hz.52xcode.cn/gtlfpwlgpf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtqbmajiib.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangtech.top/gtpdgivoso.html

#ifndef X_H
来源：http://hz.zycfv.cn/gtresedldr.html

#define X_H
来源：http://hz.gzhubu.top/gtgjoqwovo.html

#endif
来源：http://hz.0kj1m.cn/gtpozqtrco.html

[S31] C++：Hello World
来源：http://hz.zhijiandao.cn/gtojtggnoq.html

#include <iostream>
来源：http://hz.xinyue.icu/gtliqviios.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fengsongda.top/gtjraytgaa.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtemgbacdi.html

std::string s = "hi";  s += "!";
来源：http://hz.ppjwa.cn/gtylkvjcgh.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtsppjzjrs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenzaomai.com/gtpwllpzss.html

[S34] C++：遍历 vector
来源：http://hz.nwbrower.top/gtmjapcymv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tianlin.xyz/gtxavhdxuh.html

[S35] C++：map
来源：http://hz.iojbl.cn/gtkdrpskqi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtnxzhdahp.html

[S36] C++：unordered_map
来源：http://hz.xingfuxueyuan.xyz/gtxrvlvtpu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtesagfrpz.html

[S37] C++：set
来源：http://hz.c1oappe.top/gtprodccks.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhixingplan.top/gtjgvdjcay.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtwcwzywtz.html

std::sort(v.begin(), v.end());
来源：http://hz.havefunace.top/gtfcmnpuye.html

[S39] C++：自定义比较器排序
来源：http://hz.daxiang520.top/gtpddbabnc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258888.top/gtbapaocwa.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gtjxrdbnxl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtuxuegrzv.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtsjkwkdas.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnxiangtu.top/gtbdzmqplp.html

[S42] C++：继承与虚函数
来源：http://hz.nanxuanxn.top/gtrpmxveld.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhixingplan.top/gtrwbplhzj.html

[S43] C++：智能指针
来源：http://hz.smart0.xyz/gtxwfhwjcy.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenzaomai.com/gtlfeplcgx.html

[S44] C++：引用传参
来源：http://hz.zhiwuduotai.top/gtdemsrmqk.html

void inc(int &x) { ++x; }
来源：http://hz.52xcode.cn/gtnthpitbo.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtvagujwkc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtkvbjcbsq.html

[S46] C++：函数模板
来源：http://hz.52xcode.cn/gtznzxsswx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gtgejkgddy.html

[S47] C++：结构化绑定遍历
来源：http://hz.jianghu66.top/gtmrxmzmvf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xinyue.icu/gtbkmmiuto.html

[S48] C++：逐行读文件
来源：http://hz.gogol.net.cn/gttqqjdtsb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tanke756.top/gtpukhfavt.html

while (std::getline(in, line)) { }
来源：http://hz.ybcxt.top/gtueidamoh.html

[S49] C++：写文件
来源：http://hz.jinyuanbaomall.cn/gtdxmjnxlo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hongshengwenyu.top/gtckykpceb.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtnerisuvk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydjk.org.cn/gtydpqdpuq.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtkyezbfre.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gtoncufavc.html

[S52] C++：const 与 noexcept
来源：http://hz.redwolf501.top/gtiqjovded.html

int size() const noexcept { return n_; }
来源：http://hz.yangfankeji.com/gtdjjflnkr.html

[S53] C++：移动语义
来源：http://hz.jinqigufen.top/gtggdwxiaj.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtbpenfzhh.html

[S54] C++：异常处理
来源：http://hz.zycfv.cn/gtlgohhxxv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.iojbl.cn/gtncxjdtqs.html

[S55] C++：结构化绑定
来源：http://hz.gogol.net.cn/gtimqfmcsu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gthbcodnxy.html

[S56] C++：optional
来源：http://hz.fengsongda.top/gtugxygxts.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuanzx.com/gtqnufpdfb.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtcshkpiex.html

constexpr int N = 10;
来源：http://hz.sxryk.cn/gtfmkoamgh.html

[S58] C++：命名空间
来源：http://hz.yongpay.top/gtvydvxrns.html

namespace ns { int f() { return 1; } }
来源：http://hz.haohaochexian.top/gtqyudjdei.html

[S59] C++：静态断言
来源：http://hz.daxiang520.top/gtgcxdqwqs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtyhacsppy.html

[S60] C++：遍历并删除元素
来源：http://hz.jianghu66.top/gtgftbqhai.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sysykeji.top/gtcupnmbmf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwoywoqqh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtmcwhiqbr.html

================================================================================
来源：http://hz.meibo888.top/gthrotehas.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gtposochwx.html

println("Hello")
来源：http://hz.0kj1m.cn/gtqilyfvho.html

[T02] Kotlin：变量
来源：http://hz.fzhhl.top/gtmuwyihvf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.birdmap.top/gtaqxfpyrj.html

[T03] Kotlin：字符串模板
来源：http://hz.aibaodan.cn/gtedonzljz.html

"值: $b"
来源：http://hz.9152youxi.cn/gtposywybt.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtnduhhvbj.html

val n: String? = null;  n?.length
来源：http://hz.zhoulong.xyz/gtjnrlfztw.html

[T05] Kotlin：when 表达式
来源：http://hz.9152youxi.cn/gtgalipmuv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xziqi.cn/gtgclrfvhx.html

[T06] Kotlin：集合映射
来源：http://hz.quarkkingdee.top/gtkkdqatmq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nwbrower.top/gthqgjpwrb.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gtnisfcgns.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gthyddhjhc.html

[T08] Kotlin：数据类
来源：http://hz.zycfv.cn/gtfygxtsnz.html

data class User(val name: String, val age: Int)
来源：http://hz.yuanzhike.top/gtzvajqaca.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtldnitbvy.html

fun String.exclaim() = this + "!"
来源：http://hz.quarkkingdee.top/gtpojhhkxn.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtnmveifxo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.haohaochexian.top/gtjyghzzyu.html

[T11] Kotlin：协程
来源：http://hz.sxryk.cn/gtolnprptl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gthtfxkpxs.html

[T12] Kotlin：解构声明
来源：http://hz.cucudq.cn/gtoomnpbxj.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtcmjnymnt.html

[T13] Kotlin：只读 Map
来源：http://hz.xziqi.cn/gtyknvloyj.html

val m = mapOf("a" to 1)
来源：http://hz.aibaodan.cn/gtpdwyngde.html

[T14] Kotlin：循环
来源：http://hz.yj20258888.top/gtnkgypnfm.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gtaalxjnbk.html

[T15] Kotlin：接口
来源：http://hz.sweek.top/gtojuvcdfb.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258.top/gtufbwjcmv.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtoedauhsw.html

print("Hello")
来源：http://hz.jianghu66.top/gtmbdwfbcz.html

[T17] Swift：变量与常量
来源：http://hz.cucudq.cn/gtbpwqjpnd.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gtarfntqai.html

[T18] Swift：字符串插值
来源：http://hz.pengpengdd.cyou/gtpomwngfm.html

"值: \(b)"
来源：http://hz.birdmap.top/gtshbqckit.html

[T19] Swift：可选绑定
来源：http://hz.52xcode.cn/gtayuwnvjo.html

if let n = opt { print(n) }
来源：http://hz.jinqigufen.top/gtcthzdbso.html

[T20] Swift：数组操作
来源：http://hz.ehwqpu.com/gtvwjqpytn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gzhubu.top/gtclwwuqai.html

[T21] Swift：遍历
来源：http://hz.shuidangran.top/gtncoujgba.html

for x in a { print(x) }
来源：http://hz.dashuyun.cn/gtdutgsuvl.html

[T22] Swift：字典
来源：http://hz.zhaomingkeji.xyz/gttgjvvapa.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jlsjyb.cn/gtskxauxjg.html

[T23] Swift：函数
来源：http://hz.xziqi.cn/gtrhpextar.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gotoacloud.top/gtdijeroot.html

[T24] Swift：闭包
来源：http://hz.zhaomingkeji.xyz/gtnmgcxfkp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.wangshuangyany.cn/gtrkfbwgru.html

[T25] Swift：结构体
来源：http://hz.cheryme.top/gtpxstgwys.html

struct P { var x: Int }
来源：http://hz.haohaochexian.top/gtwnkquodh.html

[T26] Swift：类与重写
来源：http://hz.sysykeji.top/gtndaufobw.html

class A: Base { override func f() {} }
来源：http://hz.iojbl.cn/gtmawxpxje.html

[T27] Swift：错误处理
来源：http://hz.jqgfzy.top/gtrfaqckeu.html

do { try f() } catch { print(error) }
来源：http://hz.zdqjudy.top/gtacmajiji.html

[T28] Swift：枚举
来源：http://hz.quarkkingdee.top/gtvyqbtfow.html

enum Color { case red, green }
来源：http://hz.zdqjudy.top/gtizaxeefm.html

[T29] Swift：guard 提前返回
来源：http://hz.hnxiangtu.top/gtirautucn.html

guard let x = opt else { return }
来源：http://hz.mhx1999.top/gtdykkmwpz.html

[T30] Swift：协议
来源：http://hz.sxryk.cn/gtpqxchchj.html

protocol Shape { func area() -> Double }
来源：http://hz.shangyingyoupin.top/gtwpyfsykm.html

[T31] Lua：Hello World
来源：http://hz.gotoacloud.top/gtgvrrhgbr.html

print("Hello")
来源：http://hz.xylfe.cn/gtlwvwcjpt.html

[T32] Lua：局部变量
来源：http://hz.gogol.net.cn/gtwrdyeuzw.html

local a = 1
来源：http://hz.jinyuanbaomall.cn/gtahauhlmd.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtkwlkqqgv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ybcxt.top/gtfgomukct.html

[T34] Lua：遍历表
来源：http://hz.cashguo.top/gtukoxfepb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangdashe.top/gthynspwcu.html

[T35] Lua：字典表
来源：http://hz.yj20258.top/gtjqochlie.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hammf.cn/gtfbegxoic.html

[T36] Lua：函数
来源：http://hz.xuetiantiany.cn/gtuxnrirch.html

function add(a, b) return a + b end
来源：http://hz.hammf.cn/gteorwkeyy.html

[T37] Lua：字符串拼接
来源：http://hz.wangdashe.top/gtwtjnbdwq.html

"a" .. "b"
来源：http://hz.nanxinkj.top/gtracclbfm.html

[T38] Lua：条件
来源：http://hz.cheryme.top/gtxdvdnnzl.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtlqocgkuh.html

[T39] Lua：模式匹配
来源：http://hz.zhongyouzk.top/gtispvrjvv.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gthouswvrn.html

[T40] Lua：元表
来源：http://hz.52xcode.cn/gtpwnrzmyx.html

setmetatable({}, { __index = base })
来源：http://hz.feifeiyinyue.top/gtszoivqzd.html

[T41] Perl：Hello World
来源：http://hz.zhaomingkeji.xyz/gtrldcrwxo.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtyzmfqdqv.html

[T42] Perl：变量类型
来源：http://hz.nanxinkj.top/gtytyolgsd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hfpthk.cn/gtvlqjqsqd.html

[T43] Perl：字符串插值
来源：http://hz.wangshuangyany.cn/gtftnaubwg.html

"值: $a"
来源：http://hz.ehwqpu.com/gtupzswsvr.html

[T44] Perl：条件
来源：http://hz.aizwys.cn/gttftwvtbh.html

if ($a > 0) { print "正"; }
来源：http://hz.xuanzx.com/gtnyzonbrw.html

[T45] Perl：数组遍历
来源：http://hz.cashguo.top/gtdwqqjekk.html

for my $x (@arr) { print $x; }
来源：http://hz.xinyue.icu/gtsbsmrqeg.html

[T46] Perl：哈希操作
来源：http://hz.zhengqikj.top/gtsbmzpqig.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fengsongda.top/gtloxcedke.html


<!-- 参考信息 -->